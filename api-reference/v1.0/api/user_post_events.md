# <a name="create-event"></a>Создание объекта Event

Создание [события](../resources/event.md) в стандартном календаре пользователя. 

В рамках этих значений вы можете задать часовой пояс для каждого времени начала или окончания события, так как свойства **start** и **end** относятся к типу [DateTimeTimeZone](../resources/datetimetimezone.md). 

При создании события сервер отправляет приглашения всем участникам.


## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**: *Calendars.ReadWrite*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:-----------|:------|
| Авторизация  | Bearer <token>. Обязательный параметр.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Тело запроса
Предоставьте в теле запроса описание объекта [Event](../resources/event.md) в формате JSON.

Так как ресурс **event** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `201, Created` и объект [Event](../resources/event.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
