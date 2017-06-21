# <a name="create-thread"></a>Создание цепочки

Создание цепочки в указанной беседе. 

Создание указанных цепочки и записи. Используйте [цепочку ответов](conversationthread_reply.md), чтобы размещать дальнейшие записи в этой цепочке. Кроме того, если вы получаете идентификатор записи, вы можете [ответить](post_reply.md) на эту запись в цепочке.

Примечание. Вы также можете [начать новую беседу, создав цепочку](group_post_threads.md).

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуются указанные ниже **области**. *Group.ReadWrite.All*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В теле запроса укажите описание объекта [ConversationThread](../resources/conversationthread.md) в формате JSON.


## <a name="response"></a>Отклик
В случае успеха этот метод возвратит код отклика `201, Created` и объект [ConversationThread](../resources/conversationthread.md) в теле отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
В теле запроса укажите описание объекта [conversationThread](../resources/conversationthread.md) в формате JSON.
##### <a name="response"></a>Отклик

В случае успеха этот метод возвратит код отклика `201, Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
