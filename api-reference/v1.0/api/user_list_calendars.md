# <a name="list-calendars"></a>Список календарей

Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы по умолчанию или из указанной группы календарей. 
## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**: *Calendars.Read; Calendars.ReadWrite*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

Все календари пользователя.
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

Календари пользователя в объекте [calendarGroup](../resources/calendarGroup.md) по умолчанию.
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

Календари пользователя в указанном объекте [calendarGroup](../resources/calendarGroup.md).
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type   | application/json | 

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.
## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": "auto",
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->