# <a name="delete-subscription"></a>Удаление подписки

Удаление подписки.

## <a name="prerequisites"></a>Предварительные условия

В таблице ниже перечислены рекомендуемые разрешения, которые требуются для каждого ресурса.

| Тип ресурса / Элемент        | Область               |
|-----------------------------|---------------------|
| Контакты                    | Contacts.Read       |
| Беседы               | Group.Read.All      |
| События                      | Calendars.Read      |
| Сообщения                    | Mail.Read           |
| Диск (хранилище OneDrive пользователя)    | Files.ReadWrite.     |
| Диски (контент и диски в SharePoint, к которым предоставлен общий доступ) | Files.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
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
Ниже приведен пример ответа.
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
