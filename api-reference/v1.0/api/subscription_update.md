# <a name="update-subscription"></a>Обновление подписки

Возобновление подписки путем увеличения срока действия.

Даты окончания срока действия для подписок на ресурсы задаются отдельными типами ресурсов.  Чтобы не пропускать уведомления, следует продлевать подписки задолго до конечной даты.  Отдельные даты окончания срока действия представлены в описании ресурса [subscription](../resources/subscription.md).
## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных ниже **областей** (в зависимости от целевого ресурса): *Mail.Read*, *Calendars.Read*, *Contacts.Read*, *Group.Read.All*, *Files.ReadWrite* или *Files.ReadWrite.All*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | строка  | Bearer <token>. Обязательный параметр. |

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
