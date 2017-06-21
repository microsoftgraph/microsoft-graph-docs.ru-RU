# <a name="get-attachment"></a>Вывод вложения

Чтение свойств и связей объекта, представляющего вложение, которое было добавлено к [данным о событии](../resources/event.md), [сообщению](../resources/message.md) или [записи](../resources/post.md). 

Допустимые типы вложений:

* файл (ресурс [fileAttachment](../resources/fileattachment.md));
* элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));
* ссылка на файл (ресурс [referenceAttachment](../resources/referenceAttachment.md)).

Все типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md). 

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**:

* При доступе к вложениям в сообщениях: *Mail.Read*
* При доступе к вложениям в событиях: *Calendars.Read*
* При доступе к вложениям в событиях или записях групп: *Group.Read.All*

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md) по умолчанию для пользователя или группы.
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /groups/{id}/events/{id}/attachments/{id}

GET /me/calendar/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
```
Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
Вложения [события](../resources/event.md) в [календаре](../resources/calendar.md), принадлежащем к группе [calendarGroup](../resources/calendargroup.md) пользователя.
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Основной текст запросов
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и объект [attachment](../resources/attachment.md) в тексте отклика.

## <a name="example-file-attachment"></a>Пример (вложенный файл)

##### <a name="request"></a>Запрос
Ниже приведен пример запроса на получение вложенного файла из данных, касающихся события.
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "contentType": "contentType-value",
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```
## <a name="example-item-attachment"></a>Пример (вложенный элемент)

##### <a name="request"></a>Запрос
Ниже приведен пример запроса на получение вложенного элемента из данных, касающихся события.
<!-- {
  "blockType": "request",
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


## <a name="example-reference-attachment"></a>Пример (вложенная ссылка)
##### <a name="request"></a>Запрос
Ниже приведен пример запроса на получение вложенной ссылки из данных, касающихся события.
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "contentType": "contentType-value",
  "lastModifiedDateTime": "datetime-value",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99,
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
