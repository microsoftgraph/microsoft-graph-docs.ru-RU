# <a name="create-conversation"></a>Создание объекта Conversation

Создание беседы путем включения цепочки и записи. 

Размещать в беседе дальнейшие записи можно с помощью ответов на [цепочки](conversationthread_reply.md) и [записи](post_reply.md).
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
Предоставьте в тексте запроса описание объекта [conversation](../resources/conversation.md), содержащего объекты [conversationThread](../resources/conversationThread.md) и [post](../resources/post.md), в формате JSON.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `201, Created` и объект [conversation](../resources/conversation.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations
Content-type: application/json

{
  "topic": "New Conversation Topic",
  "threads": [{
    "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      },
      "newParticipants": [{
        "emailAddress": {
          "name": "Alex Darrow",
          "address": "alexd@contoso.com"
        }
      }]
    }]
  }]
}
```
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->