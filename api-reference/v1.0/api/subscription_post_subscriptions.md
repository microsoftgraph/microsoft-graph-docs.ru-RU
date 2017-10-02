# <a name="create-subscription"></a>Создание подписки

Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.
## <a name="permissions"></a>Разрешения
Создание подписки требует наличия области чтения для ресурса. Например, чтобы получать сообщения уведомлений, приложению необходимо разрешение `Mail.Read`. В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

| Тип ресурса или элемент        | Разрешение          |
|-----------------------------|---------------------|
| Contacts                    | Contacts.Read       |
| Беседы               | Group.Read.All      |
| События                      | Calendars.Read      |
| Сообщения                    | Mail.Read           |
| Диск (хранилище OneDrive пользователя)    | Files.ReadWrite.     |
| Диски (контент и диски в SharePoint, к которым предоставлен общий доступ) | Files.ReadWrite.All |

 ***Примечание.*** Конечная точка /v1.0 позволяет использовать разрешения для приложений в случае большинства ресурсов. Тип ресурсов Conversations в корневых элементах диска Group и OneDrive не поддерживает разрешения для приложений.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `201, Created` и объект [subscription](../resources/subscription.md) в теле отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->
```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "subscription-identifier"
}
```
Предоставьте в теле запроса описание объекта [subscription](../resources/subscription.md) в формате JSON. Поле *clientState* не является обязательным.

##### <a name="resources-examples"></a>Примеры ресурсов
Ниже приведены допустимые значения свойства ресурса для подписки.

| Тип ресурса | Примеры |
|:------ |:----- |
|Mail|me/mailfolders('inbox')/messages<br />me/messages|
|Contacts|me/contacts|
|Calendars|me/events|
|Conversations|groups('*{id}*')/conversations|
|Drives|me/drive/root|

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 201 Created

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/mailFolders('Inbox')/messages",
  "changeType":"created, updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```
## <a name="subscription-validation"></a>Проверка подписки
Чтобы подписки по ошибке не отправляли уведомления на произвольные URL-адреса, у конечной точки уведомлений подписки должна быть возможность ответить на запрос проверки. Во время обработки запроса `POST` к конечной точке `/subscriptions` Microsoft Graph отправляет запрос `POST` обратно на адрес `notificationUrl` в следующей форме: 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
В течение 10 секунд конечная точка уведомления должна отправить код отклика 200 со значением `<token>` в теле отклика и типом контента `text/plain`, как показано ниже. В противном случае запрос на создание будет отменен.
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
## <a name="notification-payload"></a>Полезные данные уведомлений
При изменении подписанного ресурса веб-перехватчик отправляет уведомление на URL-адрес уведомлений с приведенными ниже полезными данными.  В течение 30 секунд конечная точка уведомлений должна отправить код отклика 200 или 204 без тела отклика. В противном случае будут выполняться повторные попытки отправки уведомления с экспоненциально растущими интервалами.  Службы, у которых обработка запросов постоянно занимает не менее 30 секунд, можно отрегулировать, чтобы сократить отправляемый им набор уведомлений.

В ответ на уведомления службы также могут возвращать код отклика 422. В этом случае подписка автоматически удаляется, в поток уведомлений останавливается.

В зависимости от подписанного ресурса, в дополнительном поле resourceData могут быть представлены различные сведения.

```http
{
   "value":[
      {
         "subscriptionId":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
         "subscriptionExpirationDateTime":"2015-11-20T18:23:45.9356913Z",
         "clientState":"subscription-identifier",
         "changeType":"Created",
         "resource":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
         "resourceData":{
            "@odata.type":"#Microsoft.Graph.Message",
            "@odata.id":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
            "@odata.etag":"W/\"CQAAABYAAACoeN6SYXGLRrvRm+CYrrfQAACvvGdb\"",
            "Id":"AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA="
         }
      }
   ]
}
```
При получении уведомлений от подписок на диски поле resourceData содержит значение null, а для определения внесенных изменений необходимо вызвать API [delta](driveitem_delta.md). Ниже представлен пример уведомления о диске.
```http
{
  "subscriptionId": "aa269f87-2a92-4cff-a43e-2771878c3727",
  "clientState": "My client state",
  "changeType": "updated",
  "resource": "me/drive/root",
  "subscriptionExpirationDateTime": "2016-08-26T23:08:37.00+00:00",
  "resourceData": null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
