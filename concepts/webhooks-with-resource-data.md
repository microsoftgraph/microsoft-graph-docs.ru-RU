---
title: Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)
description: Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Уведомления могут включать свойства ресурсов.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: a0db70d65b919033f6c371b8bf704ed7e2c77b5b
ms.sourcegitcommit: 8a84ee922acd2946a3ffae9f8f7f7b485567bc05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2020
ms.locfileid: "42618653"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a>Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)

Microsoft Graph позволяет приложениям подписываться на уведомления об изменениях ресурсов с использованием [веб-перехватчиков](webhooks.md). Теперь можно настроить подписки таким образом, чтобы в уведомления включались данные измененных ресурсов (например, содержимое сообщения чата из Microsoft Teams). Затем приложение сможет запустить свою бизнес-логику без отдельного вызова API для получения измененного ресурса. В результате приложение работает эффективнее, выполняя меньше вызовов API, что полезно в крупномасштабных сценариях.

Добавление данных ресурса в уведомления требует реализации следующей дополнительной логики, чтобы выполнить требования по доступу к данным и их безопасности. 

- [Применяйте](#subscription-life-cycle-notifications) специальные уведомления _жизненного цикла_ подписки, чтобы обеспечить непрерывный поток данных. Microsoft Graph периодически отправляет уведомления жизненного цикла, требуя от приложения повторной авторизации, чтобы обеспечить отсутствие неожиданных проблем с доступом при включении данных ресурсов в уведомления.
- [Проверяйте](#validating-the-authenticity-of-notifications) подлинность уведомлений, подтверждая что их источником является Microsoft Graph.
- [Предоставьте](#decrypting-resource-data-from-change-notifications) открытый ключ шифрования и используйте закрытый ключ для расшифровки данных ресурсов, полученных в уведомлениях.

## <a name="resource-data-in-notification-payload"></a>Сведения ресурсов в полезных данных уведомлений

Обычно этот тип уведомлений об изменениях содержит следующие сведения ресурсов в полезных данных.

- Идентификатор и тип измененного экземпляра ресурса, возвращаемые в свойстве **resourceData**.
- Все значения свойств экземпляра ресурса, зашифрованные в соответствии с подпиской и возвращаемые в свойстве **encryptedContent**.
- Или зависимые от ресурса определенные свойства, возвращаемые в свойстве **resourceData**. Чтобы получить только определенные свойства, их нужно указать в URL-адресе объекта **resource** в подписке, используя параметр `$select`.  


## <a name="supported-resources"></a>Поддерживаемые ресурсы

В настоящее время ресурс [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (предварительная версия) в Microsoft Teams поддерживает уведомления об изменениях, включающие данные ресурсов. В частности, вы можете настроить подписку, относящуюся к одному из следующих элементов:

- Новые или измененные сообщения в определенном канале Teams: `/teams/{id}/channels/{id}/messages`
- Новые или измененные сообщения в определенном чате Teams: `/chats/{id}/messages`

Ресурс **chatMessage** поддерживает включение в уведомление всех свойств измененного экземпляра. Он не поддерживает возвращение только выбранных свойств экземпляра. 

В этой статье рассматривается пример подписки на уведомления об изменениях в канале Teams. При этом каждое уведомление содержит все данные ресурсов измененного экземпляра **chatMessage**.

## <a name="creating-a-subscription"></a>Создание подписки

Чтобы включить данные ресурсов в уведомления об изменениях, **требуется** указать следующие свойства в дополнение к обычно указываемым при [создании подписки](webhooks.md#creating-a-subscription):

- **includeResourceData**, которому следует присвоить значение `true`, чтобы явно запросить данные ресурса.
- **lifecycleNotificationUrl**, являющееся конечной точкой, в которую доставляются [уведомления жизненного цикла](#subscription-life-cycle-notifications). Оно может совпадать с **notificationUrl**.
- **encryptionCertificate**, содержащее только открытый ключ, используемый Microsoft Graph для шифрования данных ресурса. Сохраняйте соответствующий закрытый ключ для [расшифровки контента](#decrypting-resource-data-from-change-notifications).
- **encryptionCertificateId**, являющееся вашим собственным идентификатором для сертификата. Используйте этот идентификатор для определения в каждом уведомлении сертификата, используемого для расшифровки.

Учитывайте следующее:

- Используйте одинаковое имя узла для обеих конечных точек уведомлений (**notificationUrl** и **lifecycleNotificationUrl**).
- Проверьте обе конечные точки уведомлений, как описано [здесь](webhooks.md#notification-endpoint-validation). Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.
- Вы не сможете обновить (`PATCH`) существующую подписку, чтобы добавить свойство **lifecycleNotificationUrl**. Следует удалить существующую подписку и создать новую, чтобы указать свойство **lifecycleNotificationUrl**.

### <a name="subscription-request-example"></a>Пример запроса на подписку

В примере ниже выполняется подписка на два типа уведомлений: 

- Изменения ресурсов — создание или обновление сообщений каналов в Microsoft Teams
- События жизненного цикла подписки, которые могут влиять на поток уведомлений об изменениях. Дополнительные сведения об уведомлениях жизненного цикла см. в [следующем разделе](#subscription-life-cycle-notifications).

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a>Отклик подписки
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "encryptionCertificateThumbprint": "{thumbprint from the certificate}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-life-cycle-notifications"></a>Уведомления жизненного цикла подписки

Некоторые события могут воздействовать на стандартный потоку уведомлений в существующей подписке. _Уведомления жизненного цикла_ подписки указывают необходимые действия для обеспечения непрерывного потока. В отличие от уведомления об изменении ресурса, информирующем об изменении экземпляра ресурса, уведомление жизненного цикла относится к самой подписке и ее текущему состоянию в жизненном цикле. 

Уведомления жизненного цикла доставляются в объект **lifecycleNotificationUrl**. 

Содержание

- [Уведомление жизненного цикла, запрашивающее авторизацию подписки](#life-cycle-notification-that-challenges-subscription-authorization)
- [Поток запроса авторизации](#authorization-challenge-flow)
- [Пример запроса авторизации](#example-authorization-challenge)
- [Ответ на запрос авторизации](#responding-to-an-authorization-challenge)
- [Советы](#tips)
- [Подготовка к изменениям кода для обработки других типов уведомлений жизненного цикла](#future-proof-your-code-to-handle-other-types-of-life-cycle-notifications)

### <a name="life-cycle-notification-that-challenges-subscription-authorization"></a>Уведомление жизненного цикла, запрашивающее авторизацию подписки

Один из типов уведомлений жизненного цикла запрашивает авторизованное состояние активной подписки. Если в свойстве **lifecycleEvent** уведомления указано значение `reauthorizationRequired`, требуется повторно авторизовать подписку, чтобы поток данных не прерывался.

При создании долгосрочной подписки (например, длительностью 3 дня) уведомления о данных ресурсов направляются в расположение, указанное в свойстве **notificationUrl**. Однако в любой момент Microsoft Graph может потребовать повторную авторизацию подписки, чтобы подтвердить наличие у вас доступа к данным ресурсов в случае изменения условий доступа с момента создания подписки. Ниже приведены примеры изменений, влияющих на доступ к данным.

- Администратор клиента может отозвать разрешения приложения на чтение ресурса.
- В интерактивном сценарии к пользователю, предоставляющему маркер проверки подлинности для вашего приложения, могут применяться динамические политики на основе различных факторов, например их расположения, состояния устройства или оценки риска. Например, если пользователь изменяет свое физическое расположение, ему может быть запрещен доступ к данным, и ваше приложение не сможет повторно авторизовать подписку. Дополнительные сведения о динамических политиках, управляющих доступом, см. в статье [Политики условного доступа Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview). 

### <a name="authorization-challenge-flow"></a>Поток запроса авторизации

Поток запроса авторизации для активной подписки с неистекшим сроком действия выглядит следующим образом:

1. Microsoft Graph требует повторной авторизации подписки
    
    Причины этого могут отличаться для разных ресурсов и меняться со временем. Независимо от причины события повторной авторизации вам потребуется отреагировать на него.

2. Microsoft Graph отправляет уведомление о запросе авторизации в **lifecycleNotificationUrl**

    Обратите внимание, что поток уведомлений о ресурсе может некоторое время продолжаться, предоставляя вам дополнительное время для ответа. Однако в конечном итоге доставка уведомлений о ресурсе будет приостановлена, пока вы не выполните требуемое действие.

3. Ответьте на это уведомление одним из двух способов:
    1. Повторная авторизация подписки. Это не продлевает срок действия подписки.
    2. Возобновление подписки. Это повторно авторизует подписку и продлевает срок ее действия.

    Примечание. Оба действия требуют предоставление действительного маркера проверки подлинности по аналогии с [созданием новой подписки](webhooks.md#creating-a-subscription) или [продлением подписки до истечения срока ее действия](webhooks.md#renewing-a-subscription).

4. Если вы успешно выполнили повторную авторизацию или возобновление подписки, уведомления о ресурсах продолжать поступать. В противном случае уведомления о ресурсах не будут возобновлены.
    
### <a name="example-authorization-challenge"></a>Пример запроса авторизации

Ниже представлен пример уведомления жизненного цикла, запрашивающего повторную авторизацию подписки. 

Обратите внимание на следующее:

- Поле `"lifecycleEvent": "reauthorizationRequired"` определяет это уведомление как запрос авторизации.
- Это уведомление не содержит никаких сведений о конкретном ресурсе, так как оно связано не с изменением ресурса, а с изменением состояния подписки.
- Как и уведомления о ресурсах, уведомления жизненного цикла можно объединять (в коллекции **value**), каждое с возможно разными значениями **lifecycleEvent**. Обрабатывайте каждое уведомление в пакете соответствующим образом.

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

### <a name="responding-to-an-authorization-challenge"></a>Ответ на запрос авторизации

Чтобы обработать уведомление жизненного цикла с запросом авторизации, выполните следующие действия. Первые два действия по подтверждению и проверке уведомления жизненного цикла аналогичны [ответу на уведомление об изменении ресурса](webhooks.md#processing-the-notification).

1. Подтвердите получение уведомления, ответив на вызов POST с помощью `HTTP 202 Accepted`.
2. Проверьте подлинность уведомления. Дополнительные сведения см. [ниже](#validating-the-authenticity-of-notifications).
3. Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия. 

    Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), библиотека сделает это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, попросив пользователя повторно войти с помощью нового пароля. Однако получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и пользователю больше недоступны данные ресурсов.

4. Вызовите один из двух следующих API. Если вызов API выполняется успешно, поток уведомлений о ресурсе возобновляется.

    - Чтобы повторно авторизовать подписку без продления ее срока, вызовите действие `/reauthorize`:
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - Чтобы одновременно возобновить и повторно авторизовать подписку, выполните обычное действие возобновления:
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      Возобновление может завершиться сбоем, так как проверки авторизации, выполняемые системой, могут отказать приложению или пользователю в доступе к ресурсу. Приложению может потребоваться получение нового маркера доступа от пользователя для повторной авторизации подписки. 
      
      Вы может повторить эти действия позднее в любое время и успешно выполнить их, если изменяются условия доступа. Все уведомления об изменении ресурсов с момента отправки уведомления жизненного цикла до успешного воссоздания подписки приложением будут потеряны. В таких случаях приложению нужно отдельно получить эти изменения.

### <a name="tips"></a>Советы 

Учитывайте следующее:

1. Запросы авторизации не отменяют необходимость возобновления подписки на изменения ресурса до истечения ее срока действия. 

    Хотя вы можете возобновить подписку при получении запроса авторизации, Microsoft Graph может не выполнять запрос для всех ваших подписок. Например, подписка без действий и уведомлений о ресурсах, ожидающих доставки, может не создавать для приложения запросы на повторную авторизацию. Обязательно [возобновите подписки](webhooks.md#renewing-a-subscription) до истечения их сроков действия.

2. Частота запросов авторизации может изменяться.

    Не делайте предположений о частоте запросов авторизации. Эти уведомления сообщают, когда нужно принимать действия, избавляя от отслеживания подписок, которым требуется повторная авторизация. Будьте готовы обрабатывать запросы авторизации каждые несколько минут для всех подписок или в редких случаях лишь для некоторых подписок.

### <a name="future-proof-your-code-to-handle-other-types-of-life-cycle-notifications"></a>Подготовка к изменениям кода для обработки других типов уведомлений жизненного цикла

Ожидайте публикацию уведомлений жизненного цикла подписки в конечной точке, указанной в **lifecycleNotificationUrl**. Они отличаются свойством **lifecycleEvent** и могут содержать немного другую схему и свойства для обслуживания своих сценариев.

Применяйте свой код, предполагая новые типы уведомлений жизненного цикла:

1. Используйте свойство **lifecycleEvent**, чтобы указать тип уведомления для определения соответствующего ответа. Например, найдите свойство `"lifecycleEvent": "reauthorizationRequired"` для определения конкретного события и обработайте его.

1. Регистрируйте все события жизненного цикла, не распознанные вашим приложением, чтобы получить сведения о них.

1. Подпишитесь на [блог разработчика Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы следить за объявлениями об уведомлениях жизненного цикла для новых сценариев.

1. Просматривайте соответствующую документацию о новых уведомлениях жизненного цикла и реализуйте для них нужную поддержку.

## <a name="validating-the-authenticity-of-notifications"></a>Проверка подлинности уведомлений

Приложения часто выполняют бизнес-логику на основе данных ресурсов, включенных в уведомления. Важно сначала проверить подлинность каждого уведомления. В противном случае посторонние смогут обмануть ваше приложение с помощью ложных уведомлений, заставить его неправильно выполнять бизнес-логику и привести к нарушению безопасности.

Для основных уведомлений, не содержащих данные ресурсов, просто проверьте их на основе значения **clientState**, как описано [здесь](webhooks.md#processing-the-notification). Это приемлемо, так как вы можете выполнять последующие надежные вызовы Microsoft Graph, чтобы получить доступ к данным ресурсов и, следовательно, влияние любых попыток подмены ограничено. 

Для уведомлений, доставляющих данные ресурсов, проведите более тщательную проверку перед обработкой данных.

Содержание

- [Маркеры проверки в уведомлении](#validation-tokens-in-the-notification)
- [Способ проверки](#how-to-validate)
- [Пример маркера JWT](#example-jwt-token)

### <a name="validation-tokens-in-the-notification"></a>Маркеры проверки в уведомлении

Уведомление с данными ресурсов содержит дополнительное свойство **validationTokens**, содержащее массив маркеров JWT, созданных Microsoft Graph. Microsoft Graph создает один маркер для каждой отдельной пары приложения и клиента, для которой существует элемент в массиве **value**. Учитывайте, что уведомления могут содержать разные элементы для различных приложений и клиентов, подписанных с помощью одинакового значения **notificationUrl**.

В следующем примере уведомление содержит два элемента для одного приложения и двух разных клиентов, поэтому массив **validationTokens** содержит два маркера, требующие проверки.

```json
{
    "value": [
          {
            "subscriptionId": "76619225-ff6b-4489-96ca-4ef547e78b22",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
            "changeType": "created",
            ...
          },
      {
            "subscriptionId": "e990d58f-fd93-40af-acf7-a7c907c5d8ea",
      "tenantId": "46d9e3bd-6309-4177-a016-b256a411e30f",
            "changeType": "created",
            ...
            }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhb...",
    "cGlkYWNyIjoiMiIsImlkc..."
    ]
}
```
### <a name="how-to-validate"></a>Способ проверки

Если вы незнакомы с проверкой маркеров, см. [статью в блоге](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) с полезным обзором. Используйте пакет SDK, например библиотеку [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) Майкрософт для .NET или стороннюю библиотеку для другой платформы.

Следует учитывать следующее: 

- Всегда отправляйте код состояния `HTTP 202 Accepted` в ответе на уведомление. 
- Делайте это перед проверкой уведомления (например, если вы храните уведомления в очередях для последующей обработки) или после нее (если они обрабатываются на ходу), даже если проверка завершилась сбоем.
- Принятие уведомления позволяет избежать ненужных повторений доставки, а также мешает любым возможным злоумышленникам выяснить, прошли ли они проверку. Вы всегда можете игнорировать неверное уведомление после его принятия.

В частности, выполняйте проверку каждого маркера JWT в коллекции **validationTokens**. Если любой из маркеров не прошел проверку, считайте уведомление подозрительным и выполните дальнейшее исследование. 

Для проверки маркеров и приложений, создающих маркеры, выполните следующие действия.

1. Убедитесь, что срок действия маркера не истек.

2. Проверьте, что маркер не был подделан и был выдан ожидаемым центром авторизации (Microsoft Azure Active Directory):

    - Получите ключи подписи от общей конечной точки конфигурации: `https://login.microsoftonline.com/common/.well-known/openid-configuration`. Эта конфигурация кэшируется приложением на определенный период времени. Имейте в виду, что конфигурация часто обновляется, так как ключи входа ежедневно меняются.
    - Проверьте подпись маркера JWT, использующего эти ключи.

    Не принимайте маркеры, выпущенные любыми другими центрами.

3. Проверьте, что маркер выпущен для вашего приложения, подписавшегося на уведомления об изменениях.

    Следующие действия являются частью стандартной логики проверки в библиотеках маркеров JWT, и обычно их можно выполнять в виде вызова одной функции. 
    - Убедитесь, что "аудитория" в маркере совпадает с идентификатором вашего приложения.
    - Если уведомления получают несколько приложений, выполните проверку по нескольким идентификаторам.


4. **Важно**. Убедитесь, что приложение, создавшее маркер, представляет издателя уведомления об изменениях Microsoft Graph. 

    - Проверьте, что свойство **appid** в маркере соответствует ожидаемому значению `0bf30f3b-4a52-48df-9a82-234910c4a086`.
    - Это гарантирует, что уведомления не отправляются другим приложением, отличным от Microsoft Graph.


### <a name="example-jwt-token"></a>Пример маркера JWT

Ниже приведен пример свойств, входящих в маркер JWT, которые требуется проверить:

```json
{
  // aud is your app's id 
  "aud": "8e460676-ae3f-4b1e-8790-ee0fb5d6148f",                           
  "iss": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "iat": 1565046813,
  "nbf": 1565046813,
  // Expiration date 
  "exp": 1565075913,                                                        
  "aio": "42FgYKhZ+uOZrHa7p+7tfruauq1HAA==",
  // appid represents the notification publisher and must always be the same value of 0bf30f3b-4a52-48df-9a82-234910c4a086 
  "appid": "0bf30f3b-4a52-48df-9a82-234910c4a086",                          
  "appidacr": "2",
  "idp": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "tid": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
  "uti": "-KoJHevhgEGnN4kwuixpAA",
  "ver": "1.0"
}
```

### <a name="example-verifying-validation-tokens"></a>Пример: подтверждение маркеров проверки

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
    var openIdConfig = await configurationManager.GetConfigurationAsync();
    var handler = new JwtSecurityTokenHandler();
    try
    {
    handler.ValidateToken(token, new TokenValidationParameters
    {
        ValidateIssuer = true,
        ValidateAudience = true,
        ValidateIssuerSigningKey = true,
        ValidateLifetime = true,
        ValidIssuer = $"https://sts.windows.net/{tenantId}/",
        ValidAudiences = appIds,
        IssuerSigningKeys = openIdConfig.SigningKeys
    }, out _);
    return true;
    }
    catch (Exception ex)
    {
    Trace.TraceError($"{ex.Message}:{ex.StackTrace}");
    return false;
    }
}
```

## <a name="decrypting-resource-data-from-change-notifications"></a>Расшифровка данных ресурсов из уведомлений об изменениях

Свойство **resourceData** уведомления содержит только основной идентификатор и сведения о типе экземпляра ресурса. Свойство **encryptedData** содержит полные данные о ресурсе, зашифрованные Microsoft Graph с использованием открытого ключа, указанного в подписке. Это свойство также содержит значения, необходимые для проверки и расшифровки. Это выполняется для повышения безопасности пользовательских данных, к которым получен доступ с помощью уведомлений. Вы отвечаете за защиту закрытого ключа, чтобы гарантировать невозможность расшифровки пользовательских данных посторонними, даже если они смогли перехватить исходные уведомления.

Содержание

- [Управление ключами шифрования](#managing-encryption-keys)
- [Расшифровка данных ресурсов](#decrypting-resource-data)
- [Пример: расшифровка уведомления с зашифрованными данными ресурсов](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a>Управление ключами шифрования

1. Получите сертификат с парой асимметричных ключей.

    - Вы можете самостоятельно подписать сертификат, так как Microsoft Graph не проверяет поставщика сертификата и использует открытый ключ только для шифрования. 
    - В качестве решения для создания и ротации сертификатов, а также безопасного управления ими используйте [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis). Убедитесь, что ключи удовлетворяют следующим условиям:

        - Ключ должен быть типа `RSA`
        - Размер ключа должен находиться в диапазоне от 2048 до 4096 бит

2. Экспортируйте сертификат в формате X.509 с кодировкой base64 и **добавьте только открытый ключ**. 

3. При создании подписки:

    - Укажите сертификат в свойстве **encryptionCertificate**, используя контент в кодировке base64, в которой сертификат был экспортирован.
    - Укажите ваш собственный идентификатор в свойстве **encryptionCertificateId**. 
  
        Этот идентификатор позволяет сопоставлять сертификаты с получаемыми уведомлениями, а также получать сертификаты из хранилища сертификатов. Длина идентификатора не должна превышать 128 символов.

4. Обеспечьте защиту закрытого ключа, чтобы ваш код обработки уведомлений мог обращаться к закрытому ключу для расшифровки данных ресурсов.

#### <a name="rotating-keys"></a>Ротация ключей

Чтобы уменьшить риск компрометации закрытого ключа, периодически изменяйте ассиметричные ключи. Чтобы добавить новую пару ключей, выполните следующие действия:

1. Получите новый сертификат с новой парой асимметричных ключей. Используйте его для всех создаваемых подписок.

2. Обновите существующие подписки с использованием нового ключа сертификата.

    - Выполняйте это в рамках регулярного возобновления подписки. 
    - Или перечислите все подписки и укажите ключ. Используйте [операцию PATCH для подписки](/graph/api/subscription-update?view=graph-rest-1.0) и обновите свойства **encryptionCertificate** и **encryptionCertificateId**.

3. Учитывайте следующее:
    - В течение некоторого периода времени старый сертификат по-прежнему можно использовать для шифрования. Чтобы расшифровать контент, у вашего приложения должен быть доступ как к старым, так и к новым сертификатам.
    - Используйте свойство **encryptionCertificateId** в каждом уведомлении, чтобы определить правильный ключ для использования.
    - Удалите старый сертификат, только когда он перестает указываться в последних уведомлениях.

### <a name="decrypting-resource-data"></a>Расшифровка данных ресурсов

Microsoft Graph использует двухэтапный процесс шифрования с целью оптимизации работы:
  - Создается симметричный ключ однократного применения, который используется для шифрования данных ресурсов.
  - Используется открытый асимметричный ключ (указанный при подписке), чтобы зашифровать симметричный ключ и добавить его в каждое уведомление этой подписки.

Всегда предполагайте, что для каждого элемента в уведомлении используется разный симметричный ключ.

Чтобы расшифровать данные ресурсов, приложение должно выполнить обратные действия, используя свойства в разделе **encryptedContent** в каждом уведомлении:

1. Используйте свойство **encryptionCertificateId**, чтобы определить сертификат для использования.

2. Инициализируйте криптографический компонент RSA (например, .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) с помощью закрытого ключа.

3. Расшифруйте симметричный ключ, указанный в свойстве **dataKey** каждого элемента в уведомлении.

    Используйте оптимальное асимметричное шифрование с дополнением (OAEP) в качестве алгоритма расшифровки.

4. Используйте симметричный ключ, чтобы вычислить подпись HMAC-SHA256 значения в объекте **data**.
  
    Сравните его со значением в объекте **dataSignature**. Если они не совпадают, считайте, что полезные данные были подменены, и не расшифровывайте их.

5. Используйте симметричный ключ с AES (например, .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) для расшифровки содержимого в объекте **data**.

    - Используйте следующие параметры расшифровки для алгоритма AES:

        - Дополнение: PKCS7
        - Режим шифрования: CBC
    - Настройте "вектор инициализации", скопировав первые 16 байт симметричного ключа, использованного для расшифровки.

6. Расшифрованное значение — это строка JSON, представляющая экземпляр ресурса в уведомлении.


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a>Пример: расшифровка уведомления с зашифрованными данными ресурсов

Ниже приведен пример уведомления, включающего зашифрованные значения свойств экземпляра **chatMessage** в сообщении канала. Экземпляр задается значением `@odata.id`.

```json
{
    "value": [
        {
            "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
            "changeType": "created",
            // Other properties typical in a resource change notification
            "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
            "resourceData": {
                "id": "1565293727947",
                "@odata.type": "#Microsoft.Graph.ChatMessage",
                "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
            },
            "encryptedContent": {
                "data": "{encrypted data that produces a full resource}",
        "dataSignature": "<HMAC-SHA256 hash>",
                "dataKey": "{encrypted symmetric key from Microsoft Graph}",
                "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
                "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
            }
        }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
    ]
}
```

В этом разделе содержатся некоторые полезные фрагменты кода, использующие C# и .NET для каждого этапа расшифровки.

#### <a name="decrypt-the-symmetric-key"></a>Расшифровка симметричного ключа

```csharp
// Initialize with the private key that matches the encryptionCertificateId.
RSACryptoServiceProvider rsaProvider = ...;        
byte[] encryptedSymmetricKey = Convert.FromBase64String(<value from dataKey property>);

// Decrypt using OAEP padding.
byte[] decryptedSymmetricKey = rsaProvider.Decrypt(encryptedSymmetricKey, fOAEP: true);

// Can now use decryptedSymmetricKey with the AES algorithm.
```
```Java
String storename = ""; //name/path of the jks store
String storepass = ""; //password used to open the jks store
String alias = ""; //alias of the certificate when store in the jks store, should be passed as encryptionCertificateId when subscribing and retrieved from the notification
KeyStore ks = KeyStore.getInstance("JKS");
ks.load(new FileInputStream(storename), storepass.toCharArray());
Key asymmetricKey = ks.getKey(alias, storepass.toCharArray());
byte[] encryptedSymetricKey = Base64.decodeBase64("<value from dataKey property>");
Cipher cipher = Cipher.getInstance("RSA/ECB/OAEPWithSHA1AndMGF1Padding");
cipher.init(Cipher.DECRYPT_MODE, asymmetricKey);
byte[] decryptedSymmetricKey = cipher.doFinal(encryptedSymetricKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```

#### <a name="compare-data-signature-using-hmac-sha256"></a>Сравнение подписи данных с помощью HMAC-SHA256

```csharp
byte[] decryptedSymmetricKey = <the aes key decrypted in the previous step>;
byte[] encryptedPayload = <the value from the data property, still encrypted>;
byte[] expectedSignature = <the value from the dataSignature property>;
byte[] actualSignature;

using (HMACSHA256 hmac = new HMACSHA256(decryptedSymmetricKey))
{
    actualSignature = hmac.ComputeHash(encryptedPayload);
}
if (actualSignature.SequenceEqual(expectedSignature))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```Java
byte[] decryptedSymmetricKey = "<the aes key decrypted in the previous step>";
byte[] decodedEncryptedData = Base64.decodeBase64("data property from encryptedContent object");
Mac mac = Mac.getInstance("HMACSHA256");
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "HMACSHA256");
mac.init(skey);
byte[] hashedData = mac.doFinal(decodedEncryptedData);
String encodedHashedData = new String(Base64.encodeBase64(hashedData));
if (comparisonSignature.equals(encodedHashedData);)
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a>Расшифровка содержимого данных ресурсов

```csharp
AesCryptoServiceProvider aesProvider = new AesCryptoServiceProvider();
aesProvider.Key = decryptedSymmetricKey;
aesProvider.Padding = PaddingMode.PKCS7;
aesProvider.Mode = CipherMode.CBC;

// Obtain the intialization vector from the symmetric key itself.
int vectorSize = 16;
byte[] iv = new byte[vectorSize];
Array.Copy(decryptedSymmetricKey, iv, vectorSize);
aesProvider.IV = iv;

byte[] encryptedPayload = Convert.FromBase64String(<value from dataKey property>);

string decryptedResourceData;
// Decrypt the resource data content.
using (var decryptor = aesProvider.CreateDecryptor())
{
  using (MemoryStream msDecrypt = new MemoryStream(encryptedPayload))
  {
      using (CryptoStream csDecrypt = new CryptoStream(msDecrypt, decryptor, CryptoStreamMode.Read))
      {
          using (StreamReader srDecrypt = new StreamReader(csDecrypt))
          {
              decryptedResourceData = srDecrypt.ReadToEnd();
          }
      }
  }
}

// decryptedResourceData now contains a JSON string that represents the resource.
```
```Java
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "AES");
IvParameterSpec ivspec = new IvParameterSpec(Arrays.copyOf(decryptedSymmetricKey, 16));
Cipher cipher = Cipher.getInstance("AES/CBC/PKCS5PADDING");
cipher.init(Cipher.DECRYPT_MODE, skey, ivspec);
String decryptedResourceData = new String(cipher.doFinal(Base64.decodeBase64(encryptedData)));
```

## <a name="see-also"></a>См. также

- [Настройка уведомлений об изменениях в пользовательских данных](webhooks.md)
- [Тип ресурса subscription](/graph/api/resources/subscription?view=graph-rest-beta)
- [Получение подписки](/graph/api/subscription-get?view=graph-rest-1.0)
- [Создание подписки](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [Обновление подписки](/graph/api/subscription-update?view=graph-rest-1.0)
