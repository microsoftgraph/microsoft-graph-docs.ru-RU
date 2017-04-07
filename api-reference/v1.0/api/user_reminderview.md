# <a name="user-reminderview"></a>user: reminderView
Возвращает список напоминаний календаря за указанный период времени. 

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**: *Calendars.Read; Calendars.ReadWrite*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a>Параметры функции
В URL-адресе запроса укажите перечисленные ниже параметры функции и их значения.

| Параметр       | Тип    |Описание|
|:---------------|:--------|:----------|
|startDateTime|String|Дата и время начала события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T19:00:00.0000000".|
|endDateTime|String|Дата и время окончания события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T20:00:00.0000000".|


## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer <token>. Обязательный параметр.  |
| Content-Type   | application/json |
| Предпочтительно | <Часовой-пояс>. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.| 

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200, OK` и объект коллекции [reminder](../resources/reminder.md) в тексте отклика.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/reminderView?startDateTime=startDateTime-value&endDateTime=endDateTime-value
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
  "value": [
    {
      "eventId": "eventId-value",
      "eventStartTime": {
        "dateTime": "dateTime-value",
        "timeZone": "timeZone-value"
      },
      "eventEndTime": {
        "dateTime": "dateTime-value",
        "timeZone": "timeZone-value"
      },
      "changeKey": "changeKey-value",
      "eventSubject": "eventSubject-value",
      "eventLocation": {
        "displayName": "displayName-value",
        "address": {
          "street": "street-value",
          "city": "city-value",
          "state": "state-value",
          "countryOrRegion": "countryOrRegion-value",
          "postalCode": "postalCode-value"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
