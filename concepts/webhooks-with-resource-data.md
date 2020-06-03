---
title: Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)
description: Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений об изменениях клиентам. Уведомления об изменениях могут включать в себя свойства ресурса.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 9135a50f8dfa631ed85a23a12e2a146893b9994f
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429560"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a>Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)

Microsoft Graph позволяет приложениям подписываться на уведомления об изменениях ресурсов с использованием [веб-перехватчиков](webhooks.md). Теперь вы можете настроить подписки, включив в уведомления об изменениях сведения об измененных ресурсах (например, о содержимом сообщения Chat Microsoft Teams). Затем приложение сможет запустить свою бизнес-логику без отдельного вызова API для получения измененного ресурса. В результате приложение работает эффективнее, выполняя меньше вызовов API, что полезно в крупномасштабных сценариях.

Включение данных ресурсов в состав уведомлений об изменениях требует реализации следующей дополнительной логики для обеспечения доступа к данным и безопасности. 

- [Обработка](#subscription-lifecycle-notifications) уведомлений о жизненном цикле подписки для поддержания непрерывного процесса передачи данных. Microsoft Graph отправляет уведомления жизненного цикла от времени к времени, чтобы приложение могло повторно авторизоваться, чтобы убедиться в том, что проблемы Access не были неожиданно обрезаны для включения данных ресурсов в уведомлениях об изменениях.
- [Проверка](#validating-the-authenticity-of-notifications) подлинности уведомлений об изменениях, поступающих от Microsoft Graph.
- [Предоставьте](#decrypting-resource-data-from-change-notifications) открытый ключ шифрования и используйте закрытый ключ для расшифровки данных ресурсов, полученных через уведомления об изменениях.

## <a name="resource-data-in-notification-payload"></a>Сведения ресурсов в полезных данных уведомлений

Обычно этот тип уведомлений об изменениях содержит следующие сведения ресурсов в полезных данных.

- Идентификатор и тип измененного экземпляра ресурса, возвращаемые в свойстве **resourceData**.
- Все значения свойств экземпляра ресурса, зашифрованные в соответствии с подпиской и возвращаемые в свойстве **encryptedContent**.
- Или зависимые от ресурса определенные свойства, возвращаемые в свойстве **resourceData**. Чтобы получить только определенные свойства, их нужно указать в URL-адресе объекта **resource** в подписке, используя параметр `$select`.  


## <a name="supported-resources"></a>Поддерживаемые ресурсы

В настоящее время ресурс [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (предварительная версия) в Microsoft Teams поддерживает уведомления об изменениях, включающие данные ресурсов. В частности, вы можете настроить подписку, относящуюся к одному из следующих элементов:

- Новые или измененные сообщения в определенном канале Teams: `/teams/{id}/channels/{id}/messages`
- Новые или измененные сообщения в определенном чате Teams: `/chats/{id}/messages`

Ресурс **chatMessage** поддерживает все свойства измененного экземпляра в уведомлении об изменении. Он не поддерживает возвращение только выбранных свойств экземпляра. 

В этой статье рассматривается пример подписки на изменение уведомлений о сообщениях в канале Teams с каждым уведомлением об изменении, включая полные данные ресурса измененного экземпляра **chatMessage** .

## <a name="creating-a-subscription"></a>Создание подписки

Чтобы включить данные ресурсов в уведомления об изменениях, **требуется** указать следующие свойства в дополнение к обычно указываемым при [создании подписки](webhooks.md#creating-a-subscription):

- **includeResourceData**, которому следует присвоить значение `true`, чтобы явно запросить данные ресурса.
- **лифецикленотификатионурл** — конечная точка, в которой доставляются [уведомления о жизненном цикле](#subscription-lifecycle-notifications) . Оно может совпадать с **notificationUrl**.
- **encryptionCertificate**, содержащее только открытый ключ, используемый Microsoft Graph для шифрования данных ресурса. Сохраняйте соответствующий закрытый ключ для [расшифровки контента](#decrypting-resource-data-from-change-notifications).
- **encryptionCertificateId**, являющееся вашим собственным идентификатором для сертификата. Используйте этот идентификатор для согласования в каждом уведомлении об изменении, который используется для расшифровки.

Учитывайте следующее:

- Используйте одно и то же имя узла для обеих конечных точек уведомлений об изменении (**notificationUrl** и **лифецикленотификатионурл**).
- Проверяйте обе конечные точки, как описано [ниже](webhooks.md#notification-endpoint-validation). Если вы решили использовать один URL-адрес для обеих конечных точек, вы получите два запроса на проверку с необходимостью ответа на них.
- Вы не сможете обновить (`PATCH`) существующую подписку, чтобы добавить свойство **lifecycleNotificationUrl**. Следует удалить существующую подписку и создать новую, чтобы указать свойство **lifecycleNotificationUrl**.

### <a name="subscription-request-example"></a>Пример запроса на подписку

В примере ниже выполняется подписка на два типа уведомлений: 

- Изменения ресурсов — создание или обновление сообщений каналов в Microsoft Teams
- События жизненного цикла подписки, которые могут влиять на процесс отправки уведомлений об изменениях. В [следующем разделе](#subscription-lifecycle-notifications)приведены дополнительные сведения об уведомлениях о жизненном цикле.

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
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications"></a>Уведомления о жизненном цикле подписки

Некоторые события могут повлиять на потоки уведомлений об изменении в существующей подписке. Уведомления жизненного цикла подписки информируют о действиях, которые необходимо выполнить для поддержания непрерывного движения. В отличие от уведомления об изменении ресурсов, которое информирует об изменении экземпляра ресурса, уведомление о жизненном цикле относится к самой подписке и ее текущему состоянию в жизненном цикле. 

Уведомления о жизненном цикле доставляются в **лифецикленотификатионурл**. 

Содержание

- [Уведомление о жизненном цикле, которое является трудной авторизацией](#lifecycle-notification-that-challenges-subscription-authorization)
- [Поток запроса авторизации](#authorization-challenge-flow)
- [Пример запроса авторизации](#example-authorization-challenge)
- [Ответ на запрос авторизации](#responding-to-an-authorization-challenge)
- [Советы](#tips)
- [Будущий код для обработки других типов уведомлений о жизненном цикле](#future-proof-your-code-to-handle-other-types-of-lifecycle-notifications)

### <a name="lifecycle-notification-that-challenges-subscription-authorization"></a>Уведомление о жизненном цикле, которое является трудной авторизацией

Один из типов уведомлений о жизненном цикле проблемы авторизованного состояния активной подписки. Если в свойстве **lifecycleEvent** уведомления указано значение `reauthorizationRequired`, требуется повторно авторизовать подписку, чтобы поток данных не прерывался.

При создании подписки с длительным сроком действия (например, в течение 3 дней) уведомления об изменениях передаются в расположение, указанное в **notificationUrl**. Однако в любой момент Microsoft Graph может потребовать повторную авторизацию подписки, чтобы подтвердить наличие у вас доступа к данным ресурсов в случае изменения условий доступа с момента создания подписки. Ниже приведены примеры изменений, влияющих на доступ к данным.

- Администратор клиента может отозвать разрешения приложения на чтение ресурса.
- В интерактивном сценарии к пользователю, предоставляющему маркер проверки подлинности для вашего приложения, могут применяться динамические политики на основе различных факторов, например их расположения, состояния устройства или оценки риска. Например, если пользователь изменяет свое физическое расположение, ему может быть запрещен доступ к данным, и ваше приложение не сможет повторно авторизовать подписку. Дополнительные сведения о динамических политиках, управляющих доступом, см. в статье [Политики условного доступа Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview). 

### <a name="authorization-challenge-flow"></a>Поток запроса авторизации

Поток запроса авторизации для активной подписки с неистекшим сроком действия выглядит следующим образом:

1. Microsoft Graph требует повторной авторизации подписки
    
    Причины этого могут отличаться для разных ресурсов и меняться со временем. Независимо от причины события повторной авторизации вам потребуется отреагировать на него.

2. Microsoft Graph отправляет уведомление о запросе авторизации в **lifecycleNotificationUrl**

    Обратите внимание на то, что процесс уведомлений об изменениях может продолжаться в течение определенного времени, что дает дополнительное время для ответа. Однако в конечном итоге Доставка уведомлений об изменениях приостанавливается до тех пор, пока не будет выполнено необходимое действие.

3. Ответьте на это уведомление о жизненном цикле одним из двух способов:
    1. Повторная авторизация подписки. Это не продлевает срок действия подписки.
    2. Возобновление подписки. Это повторно авторизует подписку и продлевает срок ее действия.

    Примечание. Оба действия требуют предоставление действительного маркера проверки подлинности по аналогии с [созданием новой подписки](webhooks.md#creating-a-subscription) или [продлением подписки до истечения срока ее действия](webhooks.md#renewing-a-subscription).

4. Если вы успешно выполнили повторную авторизацию или продление подписки, уведомления об изменениях продолжатся. В противном случае уведомления об изменениях остаются приостановленными.
    
### <a name="example-authorization-challenge"></a>Пример запроса авторизации

Ниже приведен пример уведомления жизненного цикла, запрашивающего повторную авторизацию подписки. 

Обратите внимание на следующее:

- Поле `"lifecycleEvent": "reauthorizationRequired"` определяет это уведомление как запрос авторизации.
- В уведомлении о жизненном цикле не содержатся сведения об определенном ресурсе, так как он не связан с изменением ресурса, но с изменением состояния подписки.
- Аналогично уведомлениям об изменениях можно пакетно получать уведомления о жизненном цикле (в коллекции **значений** ), в каждом из которых может быть другое значение **лифецикливент** . Соответствующим образом обработайте каждое уведомление о жизненном цикле в пакете.

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

> **Примечание:** полное описание данных, отправленных при доставке уведомлений об изменении, приведено в разделе [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection).

### <a name="responding-to-an-authorization-challenge"></a>Ответ на запрос авторизации

Выполните указанные ниже действия, чтобы обработать уведомление о жизненном цикле запроса на авторизацию. Первые два этапа подтверждения и проверки уведомления о жизненном цикле аналогичны [отклику на уведомления об изменении ресурсов](webhooks.md#processing-the-change-notification).

1. Подтвердите получение уведомления о жизненном цикле, выполнив ответ на вызов POST `HTTP 202 Accepted` .
2. Проверка подлинности уведомления о жизненном цикле. Дополнительные сведения см. [ниже](#validating-the-authenticity-of-notifications).
3. Убедитесь, что у приложения есть допустимый маркер доступа для выполнения следующего действия. 

    Если вы используете одну из [библиотек проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), библиотека сделает это за вас, повторно использовав допустимый кэшированный маркер или получив новый маркер, попросив пользователя повторно войти с помощью нового пароля. Однако получение нового маркера может завершиться сбоем, так как условия доступа могли измениться, и пользователю больше недоступны данные ресурсов.

4. Вызовите один из двух следующих API. При успешном вызове API процесс уведомления об изменении возобновляется.

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
      
      Вы может повторить эти действия позднее в любое время и успешно выполнить их, если изменяются условия доступа. Любые уведомления об изменениях ресурсов, происходящих между временем отправки уведомления о жизненном цикле и время, когда приложение в конечном итоге повторно создает подписку, будут потеряны. В таких случаях приложению нужно отдельно получить эти изменения.

### <a name="tips"></a>Советы 

Учитывайте следующее:

1. Запросы авторизации не отменяют необходимость возобновления подписки на изменения ресурса до истечения ее срока действия. 

    Хотя вы можете возобновить подписку при получении запроса авторизации, Microsoft Graph может не выполнять запрос для всех ваших подписок. Например, подписка, которая не имеет действий и не имеет уведомлений об изменениях, ожидающих доставки, может не сообщить о проблемах при повторной проверке подлинности в вашем приложении. Обязательно [возобновите подписки](webhooks.md#renewing-a-subscription) до истечения их сроков действия.

2. Частота запросов авторизации может изменяться.

    Не делайте предположений о частоте запросов авторизации. Эти уведомления о жизненном цикле указывают, когда следует выполнять действия, сохраняя, что вам нужно отслеживать, какие подписки требуют повторной проверки подлинности. Будьте готовы обрабатывать запросы авторизации каждые несколько минут для всех подписок или в редких случаях лишь для некоторых подписок.

### <a name="future-proof-your-code-to-handle-other-types-of-lifecycle-notifications"></a>Будущий код для обработки других типов уведомлений о жизненном цикле

Ожидается, что уведомления жизненного цикла подписки будут отправлены в ту же конечную точку, что и параметр **лифецикленотификатионурл**. Они отличаются свойством **lifecycleEvent** и могут содержать немного другую схему и свойства для обслуживания своих сценариев.

Реализуйте свой код в предполагали новых типов уведомлений о жизненном цикле:

1. Используйте свойство **lifecycleEvent**, чтобы указать тип уведомления для определения соответствующего ответа. Например, найдите свойство `"lifecycleEvent": "reauthorizationRequired"` для определения конкретного события и обработайте его.

1. Заносить в журнал все события жизненного цикла, не распознаваемые приложением для получения сведений о состоянии.

1. Подпишитесь на [блог разработчика Microsoft Graph](https://developer.microsoft.com/graph/blogs/) , чтобы просмотреть объявления об уведомлениях жизненного цикла для новых сценариев.

1. Просмотрите сопутствующую документацию по новым уведомлениям жизненного цикла и реализуйте соответствующие средства поддержки.

## <a name="validating-the-authenticity-of-notifications"></a>Проверка подлинности уведомлений

Приложения часто выполняют бизнес-логику на основе данных ресурса, включенных в уведомления об изменениях. Сначала необходимо проверить подлинность каждого уведомления об изменении. В противном случае третья сторона может подменить ваше приложение с уведомлениями об изменении значения false, сделать его бизнес-логику некорректной и привести к инциденту безопасности.

Для базовых уведомлений об изменениях, которые не содержат данные ресурса, просто проверяйте их на основе значения **clientState** , как описано в [этом разделе](webhooks.md#processing-the-change-notification). Это приемлемо, так как вы можете выполнять последующие надежные вызовы Microsoft Graph, чтобы получить доступ к данным ресурсов и, следовательно, влияние любых попыток подмены ограничено. 

Для уведомлений об изменениях, которые доставлять данные ресурсов, выполните более тщательную проверку перед обработкой данных.

Содержание

- [Маркеры проверки в уведомлении об изменении](#validation-tokens-in-the-change-notification)
- [Способ проверки](#how-to-validate)
- [Пример маркера JWT](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a>Маркеры проверки в уведомлении об изменении

Уведомление об изменении с данными ресурса содержит дополнительное свойство **валидатионтокенс**, которое содержит массив маркеров JWT, созданных Microsoft Graph. Microsoft Graph создает один маркер для каждой отдельной пары приложения и клиента, для которой существует элемент в массиве **value**. Имейте в виду, что уведомления об изменениях могут содержать смесь элементов для различных приложений и клиентов, подписанных с помощью одного и того же **notificationUrl**.

В следующем примере уведомление об изменении содержит два элемента для одного и того же приложения и для двух различных клиентов, поэтому массив **валидатионтокенс** содержит два токена, которые необходимо проверить.

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

> **Примечание:** полное описание данных, отправленных при доставке уведомлений об изменении, приведено в разделе [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection).

### <a name="how-to-validate"></a>Способ проверки

Если вы не знакомы с проверкой маркеров, ознакомьтесь со статьями, посведениями о том, как выполнять [проверку маркеров](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) . Используйте пакет SDK, например библиотеку [System. IdentityModel. tokens. JWT](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) для .NET, или библиотеку стороннего производителя для другой платформы.

Следует учитывать следующее: 

- Обязательно отправьте `HTTP 202 Accepted` код состояния в ответ на уведомление об изменении. 
- Выполните эти действия перед проверкой уведомления об изменении (например, если вы храните уведомления об изменениях в очередях для дальнейшей обработки) или после (если вы обрабатываете их на лету), даже если проверка завершилась неудачно.
- Принятие уведомления об изменении предотвращает ненужные попытки доставки, а также предотвращает возможность поиска ненужных фиктивных субъектов, если они прошли проверку или прошли проверку. Вы всегда можете игнорировать неправильное уведомление об изменении после того, как вы его приняли.

В частности, выполняйте проверку каждого маркера JWT в коллекции **validationTokens**. При неисправности маркеров рассмотрите уведомление об изменениях подозрительный и проанализируйте дальнейшие сведения. 

Для проверки маркеров и приложений, создающих маркеры, выполните следующие действия.

1. Убедитесь, что срок действия маркера не истек.

2. Проверьте, что маркер не был подделан и был выдан ожидаемым центром авторизации (Microsoft Azure Active Directory):

    - Получите ключи подписи от общей конечной точки конфигурации: `https://login.microsoftonline.com/common/.well-known/openid-configuration`. Эта конфигурация кэшируется приложением на определенный период времени. Имейте в виду, что конфигурация часто обновляется, так как ключи входа ежедневно меняются.
    - Проверьте подпись маркера JWT, использующего эти ключи.

    Не принимайте маркеры, выпущенные любыми другими центрами.

3. Проверьте, что маркер выпущен для вашего приложения, подписавшегося на уведомления об изменениях.

    Следующие действия являются частью стандартной логики проверки в библиотеках маркеров JWT, и обычно их можно выполнять в виде вызова одной функции. 
    - Убедитесь, что "аудитория" в маркере совпадает с идентификатором вашего приложения.
    - Если у вас есть более одного уведомления об изменении приложения, обязательно проверьте наличие нескольких идентификаторов.


4. **Важно**. Убедитесь, что приложение, создавшее маркер, представляет издателя уведомления об изменениях Microsoft Graph. 

    - Проверьте, что свойство **appid** в маркере соответствует ожидаемому значению `0bf30f3b-4a52-48df-9a82-234910c4a086`.
    - Это гарантирует, что уведомления об изменениях не отправляются другим приложением, не связанным с Microsoft Graph.


### <a name="example-jwt-token"></a>Пример маркера JWT

Ниже приведен пример свойств, включенных в маркер JWT, которые необходимы для проверки.

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
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
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
```java
private boolean IsValidationTokenValid(String[] appIds, String tenantId, String serializedToken) {
    try {
        JwkKeyResolver jwksResolver = new JwkKeyResolver();
        Jws<Claims> token = Jwts.parserBuilder()
        .setSigningKeyResolver(jwksResolver)
        .build()
        .parseClaimsJws(serializedToken);
        Claims body = token.getBody();
        String audience = body.getAudience();
        boolean isAudienceValid = false;
        for(String appId : appIds) {
        isAudienceValid = isAudienceValid || appId.equals(audience);
        }
        boolean isTenantValid = body.getIssuer().endsWith(tenantId + "/");
        return isAudienceValid  && isTenantValid; //nbf,exp and signature are already validated by library
    } catch (Exception e) {
        LOGGER.error("could not validate token");
        LOGGER.error(e.getMessage());
        return false;
    }
}
```
```JavaScript
import jwt from 'jsonwebtoken';
import jkwsClient from 'jwks-rsa';

const client = jkwsClient({
  jwksUri: 'https://login.microsoftonline.com/common/discovery/v2.0/keys'
});

export function getKey(header, callback) {
  client.getSigningKey(header.kid, (err, key) => {
    var signingKey = key.publicKey || key.rsaPublicKey;
    callback(null, signingKey);
  });
}

export function isTokenValid(token, appId, tenantId) {
  return new Promise((resolve) => {
    const options = {
      audience: [appId],
      issuer: [`https://sts.windows.net/${tenantId}/`]
    };
    jwt.verify(token, getKey, options, (err) => {
      if (err) {
        // eslint-disable-next-line no-console
        console.error(err);
        resolve(false);
      } else {
        resolve(true);
      }
    });
  });
}
```
Чтобы пример Java работал, вам также необходимо реализовать `JwkKeyResolver`.  
```java
package com.example.restservice;

import com.auth0.jwk.JwkProvider;
import com.auth0.jwk.UrlJwkProvider;
import com.auth0.jwk.Jwk;
import io.jsonwebtoken.Claims;
import io.jsonwebtoken.JwsHeader;
import io.jsonwebtoken.SigningKeyResolverAdapter;
import java.security.Key;
import java.net.URI;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class JwkKeyResolver extends SigningKeyResolverAdapter {
    private JwkProvider keyStore;
    private final Logger LOGGER = LoggerFactory.getLogger(this.getClass());
    public JwkKeyResolver() throws java.net.URISyntaxException, java.net.MalformedURLException {
        this.keyStore = new UrlJwkProvider((new URI("https://login.microsoftonline.com/common/discovery/keys").toURL()));
    }
    @Override
    public Key resolveSigningKey(JwsHeader jwsHeader, Claims claims) {
        try {
            String keyId = jwsHeader.getKeyId();
            Jwk pub = keyStore.get(keyId);
            return pub.getPublicKey();
        } catch (Exception e) {
            LOGGER.error(e.getMessage());
            return null;
        }
    }
}
```

## <a name="decrypting-resource-data-from-change-notifications"></a>Расшифровка данных ресурсов из уведомлений об изменениях

Свойство **resourceData** уведомления об изменении включает только базовый идентификатор и сведения о типе экземпляра ресурса. Свойство **encryptedData** содержит полные данные о ресурсе, зашифрованные Microsoft Graph с использованием открытого ключа, указанного в подписке. Это свойство также содержит значения, необходимые для проверки и расшифровки. Это делается для повышения безопасности данных клиентов, доступ к которым осуществляется через уведомления об изменениях. Вы отвечаете за защиту закрытого ключа, чтобы убедиться, что данные клиента не могут быть расшифрованы третьим лицом, даже если они управляют отправкой уведомлений об изменении.

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
  
        Этот идентификатор позволяет сопоставлять сертификаты с полученными уведомлениями об изменениях и получать сертификаты из хранилища сертификатов. Длина идентификатора не должна превышать 128 символов.

4. Безопасно управлять закрытым ключом, чтобы код обработки уведомления об изменении мог получать доступ к закрытому ключу для расшифровки данных ресурса.

#### <a name="rotating-keys"></a>Ротация ключей

Чтобы уменьшить риск компрометации закрытого ключа, периодически изменяйте ассиметричные ключи. Чтобы добавить новую пару ключей, выполните следующие действия:

1. Получите новый сертификат с новой парой асимметричных ключей. Используйте его для всех создаваемых подписок.

2. Обновите существующие подписки с использованием нового ключа сертификата.

    - Выполняйте это в рамках регулярного возобновления подписки. 
    - Или перечислите все подписки и укажите ключ. Используйте [операцию PATCH для подписки](/graph/api/subscription-update?view=graph-rest-1.0) и обновите свойства **encryptionCertificate** и **encryptionCertificateId**.

3. Учитывайте следующее:
    - В течение некоторого периода времени старый сертификат по-прежнему можно использовать для шифрования. Чтобы расшифровать контент, у вашего приложения должен быть доступ как к старым, так и к новым сертификатам.
    - Используйте свойство **енкриптионцертификатеид** в каждом уведомлении об изменении, чтобы определить правильный ключ.
    - Удалять старый сертификат только в том случае, если вы не видели последних уведомлений об изменениях, ссылающихся на него.

### <a name="decrypting-resource-data"></a>Расшифровка данных ресурсов

Microsoft Graph использует двухэтапный процесс шифрования с целью оптимизации работы:
  - Создается симметричный ключ однократного применения, который используется для шифрования данных ресурсов.
  - Он использует открытый асимметричный ключ (заданный при подписке) для шифрования симметричного ключа и включает его в каждое уведомление об изменении этой подписки.

Всегда думайте, что симметричный ключ отличается для каждого элемента в уведомлении об изменении.

Чтобы расшифровать данные ресурсов, приложение должно выполнить действия по обратной связи, используя свойства раздела **енкриптедконтент** в каждом уведомлении об изменении:

1. Используйте свойство **encryptionCertificateId**, чтобы определить сертификат для использования.

2. Инициализируйте криптографический компонент RSA (например, .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) с помощью закрытого ключа.

3. Расшифровка симметричного ключа, доставляемого в свойстве **датакэй** каждого элемента в уведомлении об изменении.

    Используйте оптимальное асимметричное шифрование с дополнением (OAEP) в качестве алгоритма расшифровки.

4. Используйте симметричный ключ, чтобы вычислить подпись HMAC-SHA256 значения в объекте **data**.
  
    Сравните его со значением в объекте **dataSignature**. Если они не совпадают, считайте, что полезные данные были подменены, и не расшифровывайте их.

5. Используйте симметричный ключ с AES (например, .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) для расшифровки содержимого в объекте **data**.

    - Используйте следующие параметры расшифровки для алгоритма AES:

        - Дополнение: PKCS7
        - Режим шифрования: CBC
    - Настройте "вектор инициализации", скопировав первые 16 байт симметричного ключа, использованного для расшифровки.

6. Расшифрованное значение — это строка JSON, представляющая экземпляр ресурса в уведомлении об изменении.


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a>Пример: расшифровка уведомления с зашифрованными данными ресурсов

Ниже приведен пример уведомления об изменении, включающего зашифрованные значения свойств экземпляра **chatMessage** в сообщении канала. Экземпляр задается значением `@odata.id`.

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

> **Примечание:** полное описание данных, отправленных при доставке уведомлений об изменении, приведено в разделе [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection).


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
```JavaScript
const base64encodedKey = 'base 64 encoded dataKey value';
const asymetricPrivateKey = 'pem encoded private key';
const decodedKey = Buffer.from(base64encodedKey, 'base64');
const decryptedSymetricKey = crypto.privateDecrypt(asymetricPrivateKey, decodedKey);
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
if (comparisonSignature.equals(encodedHashedData))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```JavaScript
const decryptedSymetricKey = []; //Buffer provided by previous step
const base64encodedSignature = 'base64 encodded value from the dataSignature property';
const hmac = crypto.createHmac('sha256', decryptedSymetricKey);
hmac.write(base64encodedPayload, 'base64');
if(base64encodedSignature === hmac.digest('base64'))
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
```JavaScript
const base64encodedPayload = 'base64 encoded value from data property';
const decryptedSymetricKey = []; //Buffer provided by previous step
const iv = Buffer.alloc(16, 0);
decryptedSymetricKey.copy(iv, 0, 0, 16);
const decipher = crypto.createDecipheriv('aes-256-cbc', decryptedSymetricKey, iv);
let decryptedPayload = decipher.update(base64encodedPayload, 'base64', 'utf8');
decryptedPayload += decipher.final('utf8');
```

## <a name="see-also"></a>См. также

- [Настройка уведомлений об изменениях в пользовательских данных](webhooks.md)
- [Тип ресурса subscription](/graph/api/resources/subscription?view=graph-rest-beta)
- [Получение подписки](/graph/api/subscription-get?view=graph-rest-1.0)
- [Создание подписки](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [Обновление подписки](/graph/api/subscription-update?view=graph-rest-1.0)
