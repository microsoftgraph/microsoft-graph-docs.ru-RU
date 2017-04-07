# <a name="create-calendar"></a>Создание объекта Calendar

С помощью этого API можно создать календарь в группе календарей.
## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных ниже **областей**. _Calendars.ReadWrite_
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.
```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```
Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.
```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer <token>. Обязательный параметр.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Предоставьте в тексте запроса описание объекта [Calendar](../resources/calendar.md) в формате JSON.


## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `201, Created` и объект [Calendar](../resources/calendar.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```
Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
