# <a name="working-with-webhooks-in-microsoft-graph"></a>Работа с веб-перехватчиками в Microsoft Graph

REST API Microsoft Graph использует механизм веб-перехватчиков для доставки уведомлений клиентам. Клиент — это веб-служба, которая настраивает свой URL-адрес для получения уведомлений. С помощью уведомлений клиентские приложения обновляют свое состояние при изменениях.

С помощью REST API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

* Сообщения
* События
* Контакты
* пользователи;
* Группы
* Беседы группы
* Контент с общим доступом в OneDrive, включая диски, сопоставленные с сайтами SharePoint
* Личные папки пользователя в OneDrive

Например, вы можете создать подписку на определенную папку: `me/mailFolders('inbox')/messages`

Или определенный идентификатор: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`

Или на ресурс верхнего уровня: `me/messages`, `me/contacts`, `me/events`, `users` или `groups`

В Sharepoint либо на диске в OneDrive для бизнеса: `/drive/root`

Либо в личном OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`

Приняв запрос на подписку, Microsoft Graph отправляет уведомления на URL-адрес, указанный в подписке. Затем приложение действует в соответствии с бизнес-логикой. Например, оно получает дополнительные данные, обновляет кэш и представления и т. д.

Приложениям необходимо обновлять свои подписки до истечения срока их действия. В противном случае им потребуется создавать новые подписки. Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).

Кроме того, приложение в любое время может отменить подписку, чтобы больше не получать уведомления.

В общем случае для операций с подписками необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления для сообщений, приложению необходимо разрешение `Mail.Read`. В статье, посвященной [созданию подписок](../api-reference/v1.0/api/subscription_post_subscriptions.md), перечислены разрешения, необходимые для каждого типа ресурса. В таблице ниже перечислены типы разрешений, которые ваше приложение может запрашивать, чтобы использовать веб-перехватчики для определенных типов ресурсов. 

| Тип разрешения                        | Типы ресурсов, поддерживаемые в версии 1.0                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| Delegated — рабочая или учебная учетная запись     | [contact][], [conversation][], [drive][], [event][], [message][] |
| Delegated — личная учетная запись Майкрософт | Нет                                                             |
| Application                            | [contact][], [conversation][], [event][], [message][]            |


## <a name="code-samples"></a>Примеры кода

Указанные ниже примеры кода доступны на сайте GitHub.

* [Пример веб-перехватчиков Microsoft Graph для Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Пример веб-перехватчиков Microsoft Graph для ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

### <a name="creating-a-subscription"></a>Создание подписки

Чтобы начать получать уведомления о ресурсе, сначала необходимо создать подписку. Это происходит следующим образом:

1. Клиент отправляет запрос (POST) на подписку для определенного ресурса.
2. Microsoft Graph проверяет запрос.
  * Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.
  * В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.
3. Клиент отправляет маркер проверки обратно в Microsoft Graph.

Клиент должен хранить идентификатор подписки, чтобы можно было сопоставлять уведомления с соответствующими подписками.

### <a name="notification-url-validation"></a>Проверка URL-адреса уведомления

Прежде чем создавать подписку, Microsoft Graph проверяет URL-адрес уведомлений в запросе на подписку. Проверка происходит следующим образом:

1. Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```

2. В течение 10 секунд клиент должен предоставить отклик с указанными ниже характеристиками.

  * Код состояния 200 (OK).
  * Необходимый тип контента — текст (в том числе обычный). 
  * Текст должен включать маркер проверки, который предоставил Microsoft Graph.

Клиент должен удалить маркер проверки после того, как предоставит его в отклике.

### <a name="subscription-request-example"></a>Пример запроса на подписку

``` http
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

Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`. Определения и значения свойств представлены в [описании типа ресурса subscription](../api-reference/v1.0/resources/subscription.md). Хотя свойство `clientState` необязательное, рекомендуем указать его в нашем процессе обработки уведомлений.

В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [subscription](../api-reference/v1.0/resources/subscription.md) в теле отклика.

### <a name="azure-ad-resource-limitations"></a>Ограничения ресурсов Azure AD

К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения могут возникать ошибки.

* Квоты максимальной подписки:

  * На приложение: 50 000 подписок всего
  * На клиента: 35 подписок всего во всех приложениях
  * На сочетание приложения и клиента: 7 подписок всего

* Клиенты Azure AD B2C не поддерживаются

* Пользователи потребительской версии не поддерживаются

## <a name="renewing-a-subscription"></a>Возобновление подписки

Клиент может возобновить подписку, указав срок действия до трех дней с момента отправки запроса. Свойство expirationDateTime является обязательным.

### <a name="subscription-renewal-example"></a>Пример продления подписки

``` http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [subscription](../api-reference/v1.0/resources/subscription.md) в теле отклика. Объект подписки включает новое значение expirationDateTime. 

## <a name="deleting-a-subscription"></a>Удаление подписки

Клиент может прекратить получать уведомления, удалив подписку по ее идентификатору.

``` http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.

## <a name="notifications"></a>Уведомления

После создания подписки клиент начнет получать уведомления. При изменении ресурса Microsoft Graph отправляет запрос POST на URL-адрес уведомлений. Клиент получает уведомления только об изменениях определенных типов, например *created*.

### <a name="notification-properties"></a>Свойства уведомлений

Объект уведомления содержит следующие свойства:

* subscriptionId — идентификатор подписки, к которой относится уведомление.
* subscriptionExpirationDateTime — время окончания срока действия для подписки.
* clientState — свойство clientState, указанное в запросе на подписку.
* changeType — тип события, вызвавшего уведомление. Примеры: *created* при получении сообщения или *updated*, когда сообщение помечается как прочитанное.
* resource — URI ресурса относительно `https://graph.microsoft.com`. 
* resourceData — объект, зависящий от ресурса, подписка на который создается.  Например, для ресурсов Outlook:
  * @odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.
  * @odata.id — идентификатор OData для объекта.
  * @odata.etag — HTTP-тег сущности, представляющий версию объекта.
  * id — идентификатор объекта.

> Примечание. Значение Id, указанное в resourceData, действительно в момент добавления уведомления в очередь. Некоторые действия, например перемещение сообщения в другую папку, могут привести к изменению идентификатора ресурса. 

### <a name="notification-example"></a>Пример уведомления

Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомления, аналогичные указанному ниже.

``` json
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
    "resourceData":
    {
      "@odata.type":"#Microsoft.Graph.Message",
      "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
      "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
      "id":"<long_id_string>"
    }
  }
  ]
}
```

Обратите внимание, что объект value содержит список. Если в очереди много уведомлений, Microsoft Graph отправляет их в одном запросе.

### <a name="processing-the-notification"></a>Обработка уведомления

Когда приложение начинает получать уведомления, оно должно обрабатывать их. Ниже перечислены основные задачи, которые приложение должно выполнить для обработки уведомления.

1. Проверьте свойство `clientState`. Свойство clientState уведомления должно совпадать со значением, отправленным в запросе на подписку.
  > Примечание. Если это не так, уведомление не следует рассматривать как действительное. Вы также можете определить, откуда поступило уведомление, и выполнить соответствующие действия.

2. Обновляйте приложение в соответствии с бизнес-логикой.

3. Отправляйте код состояния `202 - Accepted` в ответе, отправляемом в Microsoft Graph. Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.
  > Код состояния `202 - Accepted` следует отправлять, даже если свойство clientState не совпадает со значением, отправленным в запросе на подписку.

Повторяйте эти действия для других уведомлений в запросе.

## <a name="see-also"></a>См. также

* [Тип ресурса subscription](../api-reference/v1.0/resources/subscription.md)
* [Получение подписки](../api-reference/v1.0/api/subscription_get.md)
* [Создание подписки](../api-reference/v1.0/api/subscription_post_subscriptions.md)
* [Пример Microsoft Graph Webhooks для Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Пример Microsoft Graph Webhooks для ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

[контакт]: ../api-reference/v1.0/resources/contact.md
[беседа]: ../api-reference/v1.0/resources/conversation.md
[диск]: ../api-reference/v1.0/resources/drive.md
[событие]: ../api-reference/v1.0/resources/event.md
[сообщение]: ../api-reference/v1.0/resources/message.md
