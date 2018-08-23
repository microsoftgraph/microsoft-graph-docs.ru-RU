# <a name="create-subscription"></a>Создание подписки

Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.

## <a name="permissions"></a>Разрешения

Создание подписки требует наличия области чтения для ресурса. Например, чтобы получать сообщения уведомлений, приложению необходимо разрешение `Mail.Read`. В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

| Тип ресурса или элемент        | Разрешение          |
|-----------------------------|---------------------|
| Контакты                    | Contacts.Read       |
| Разговоры               | Group.Read.All      |
| События                      | Calendars.Read      |
| Сообщения                    | Mail.Read           |
| Группы                      | Group.Read.All      |
| Пользователи                       | User.Read.All       |
| Диск (хранилище OneDrive пользователя)    | Files.ReadWrite.     |
| Диски (содержимое и диски в SharePoint, к которым предоставлен общий доступ) | Files.ReadWrite.All |

 > **Примечание:** Конечная точка /v1.0 позволяет использовать разрешения для приложений для большинства ресурсов. Разговоры в группе и в корневом диске OneDrive не поддерживаются разрешениями приложений.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Авторизация  | строка  | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.

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
   "clientState": "secretClientValue"
}
```

В теле запроса укажите JSON-представление объекта [подписки](../resources/subscription.md).
Поле `clientState` является необязательным.

##### <a name="resources-examples"></a>Примеры ресурсов

Ниже приведены допустимые значения свойства ресурса для подписки.

| Тип ресурса | Примеры |
|:------ |:----- |
|Почта|me/mailfolders('inbox')/messages<br />me/messages|
|Контакты|me/contacts|
|Календари|me/events|
|Пользователи|users|
|Группы|groups|
|Разговоры|groups('*{id}*')/conversations|
|Диски|me/drive/root|

##### <a name="response"></a>Отклик

Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a>Проверка конечной точки уведомлений

Конечная точка уведомления подписки (указанного в свойстве`notificationUrl`) должна быть способна отвечать на запрос проверки, как описано в [Настройка уведомлений для изменения данных пользователя](../../../concepts/webhooks.md#notification-endpoint-validation). Если не удается выполнить проверку, запрос на создание подписки возвращает ошибку "400— Ошибочный запрос".

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
