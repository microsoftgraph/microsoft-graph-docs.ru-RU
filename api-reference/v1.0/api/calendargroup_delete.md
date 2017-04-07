# <a name="delete-calendargroup"></a>Удаление объекта calendarGroup

Удаление группы календарей, отличной от стандартной.

**Примечание**. Outlook.com поддерживает только группу календарей по умолчанию, доступную по ссылке /me/calendars. Удалить группу календарей в Outlook.com невозможно.

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**: *Calendars.ReadWrite*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | строка  | Bearer <token>. Обязательный параметр. |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
