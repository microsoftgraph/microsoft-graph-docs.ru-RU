# <a name="delete-subscription"></a>Удаление подписки

Удаление подписки.
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных ниже **областей** (в зависимости от целевого ресурса): *Mail.Read*, *Calendars.Read*, *Contacts.Read*, *Group.Read.All*, *Files.ReadWrite* или *Files.ReadWrite.All*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | строка  | Bearer <token>. Обязательный параметр. |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
