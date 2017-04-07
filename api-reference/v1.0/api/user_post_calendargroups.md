# <a name="create-calendargroup"></a>Создание объекта CalendarGroup

С помощью этого API можно создать объект CalendarGroup.
## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**: *Calendars.ReadWrite*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer <token>. Обязательный параметр.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `201, Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
