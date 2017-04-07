# <a name="working-with-webhooks-in-microsoft-graph"></a>Работа с веб-перехватчиками в Microsoft Graph

REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях.

С помощью REST API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

* Сообщения
* События
* Контакты
* Беседы групп
* Корневые элементы диска

Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке. Затем приложение действует в соответствии с бизнес-логикой. Например, оно получает дополнительные данные, обновляет кэш и представления и т. д.

Приложения должны обновлять свои подписки, пока не истечет срок их действия. В любой момент подписку можно отменить, чтобы перестать получать уведомления.

Изучите указанные ниже примеры кода на сайте GitHub.

* [Пример Microsoft Graph Webhooks для Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Пример Microsoft Graph Webhooks для ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

Рассмотрим процесс создания подписки.

# <a name="creating-a-subscription"></a>Создание подписки

Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:

1. Клиент отправляет запрос (POST) на подписку для определенного ресурса.
2. Microsoft Graph проверяет запрос.
  * Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.
  * В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.
3. Клиент отправляет маркер проверки обратно в Microsoft Graph.

Клиент должен сохранить идентификатор подписки, чтобы сопоставить уведомление с соответствующей подпиской.

## <a name="characteristics-of-subscriptions"></a>Характеристики подписок

Вы можете создавать подписки на такие ресурсы, как сообщения, события, контакты и элементы в корне диска.

Вы можете создать подписку на определенную папку: `https://graph.microsoft.com/v1.0/me/mailfolders('inbox')/messages`

Или на ресурс верхнего уровня: `https://graph.microsoft.com/v1.0/me/messages`

Или на элемент в корне диска: `https://graph.microsoft.com/v1.0/me/drive/root`

В большинстве случае для создания подписки требуется область чтения для ресурса. Например, чтобы получать сообщения уведомлений, приложению необходимо разрешение `mail.read`. Обратите внимание, что в настоящее время разрешение `Files.ReadWrite` необходимо для элементов в корне диска OneDrive, а для дисков, связанных с сайтами SharePoint, необходимо разрешение `Files.ReadWrite.All`.

Срок действия подписок ограничен. В настоящее время самый длительный срок действия составляет три дня без 90 минут (то есть 4230 минут) с момента создания подписки. Приложения должны обновлять свои подписки до истечения срока их действия. В противном случае им потребуется создать новую подписку.

## <a name="notification-url-validation"></a>Проверка URL-адреса уведомлений

Прежде чем создавать подписку, Microsoft Graph проверяет URL-адрес уведомлений в запросе на подписку. Проверка происходит следующим образом:

1. Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. В течение 10 секунд клиент должен предоставить отклик со следующими характеристиками:

  * Код состояния 200 (OK).
  * Необходимый тип контента — текст (в том числе обычный). 
  * Текст должен включать маркер проверки, который предоставил Microsoft Graph.

Клиент должен удалить маркер проверки после того, как предоставит его в отклике.

## <a name="subscription-request-example"></a>Пример запроса на подписку

```
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

Свойства changeType, notificationUrl, resource и expirationDateTime являются обязательными. Определения и значения свойств представлены в [описании типа ресурса subscription](subscription.md). Хотя свойство clientState является необязательным, в нашем процессе обработки уведомлений рекомендуется указать его.

В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [subscription](subscription.md) в теле отклика.

# <a name="renewing-a-subscription"></a>Возобновление подписки

Клиент может возобновить подписку, указав срок действия до трех дней с момента отправки запроса. Свойство expirationDateTime является обязательным.

## <a name="subscription-renewal-example"></a>Пример продления подписки

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [subscription](subscription.md) в теле отклика. Объект подписки включает новое значение expirationDateTime. 

# <a name="deleting-a-subscription"></a>Удаление подписки

Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.

# <a name="notifications"></a>Уведомления

После создания подписки клиент начнет получать уведомления. При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений. Клиент получает уведомления только об изменениях определенных типов, например *created*.

## <a name="notification-properties"></a>Свойства уведомлений

Объект уведомления содержит следующие свойства:

* id — идентификатор подписки, к которой относится уведомление.
* expirationDateTime — время окончания срока действия для подписки.
* clientState — свойство clientState, указанное в запросе на подписку.
* changeType — тип события, вызвавшего уведомление. Примеры: *created* при получении сообщения или *updated*, когда сообщение помечается как прочитанное.
* resource — URI ресурса относительно `https://graph.microsoft.com`. 
* resourceData — объект, зависящий от ресурса, подписка на который создается.  Например, для ресурсов Outlook:
  * @odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.
  * @odata.id — идентификатор OData для объекта.
  * @odata.etag — HTTP-тег сущности, представляющий версию объекта.
  * Id — идентификатор объекта.


> Примечание. Значение Id, указанное в resourceData, действительно в момент добавления уведомления в очередь. Некоторые действия, например перемещение сообщения в другую папку, могут привести к изменению идентификатора ресурса. 

## <a name="notification-example"></a>Пример уведомления

Когда пользователь получает электронное сообщение, Microsoft Graph отправляет уведомления, подобные следующему:

```
{
  "value":[
  {
    "id":"<subscription_guid>",
    "expirationDateTime":"\"2016-03-19T22:11:09.952Z\"",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
    "resourceData":
    {
      "@odata.type":"#Microsoft.Graph.Message",
      "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
      "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
      "Id":"<long_id_string>"
    }
  }
  ]
}
```

Обратите внимание, что объект значения содержит список. Если в очереди много уведомлений, Microsoft Graph отправляет их в одном запросе.

## <a name="processing-the-notification"></a>Обработка уведомления

Когда приложение начинает получать уведомления, оно должно обрабатывать их. Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.

1. Проверьте свойство `clientState`. Свойство clientState уведомления должно совпадать со значением, отправленным в запросе на подписку.
  > Примечание. Если это не так, уведомление не следует рассматривать как действительное. Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.

2. Обновляйте приложение в соответствии с бизнес-логикой.
3. Отправляйте код состояния `202 - Accepted` в ответе, отправляемом в Microsoft Graph. Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.
  > Код состояния `202 - Accepted` следует отправлять, даже если свойство clientState не совпадает со значением, отправленным в запросе на подписку.

Повторяйте эти действия для других уведомлений в запросе.

# <a name="additional-resources"></a>Дополнительные ресурсы

* [Тип ресурса Subscription](subscription.md)
* [Получение подписки](../api/subscription_get.md)
* [Создание подписки](../api/subscription_post_subscriptions.md)
* [Пример Microsoft Graph Webhooks для Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Пример Microsoft Graph Webhooks для ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
