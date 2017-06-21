# <a name="get-user-mailbox-settings"></a>Получение параметров почтового ящика пользователя

Получение объекта [mailboxSettings](../resources/mailboxsettings.md) пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при получении их почты), языкового стандарта (сведения о языке и стране или регионе) и часового пояса.

Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется **область** *MailboxSettings.Read*.  

## <a name="http-request"></a>HTTP-запрос
Чтобы получить все параметры почтового ящика, включающие параметры автоматических ответов, используйте указанные ниже команды.
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

Чтобы получить определенные параметры, например только параметры автоматических ответов, сведения о языковом стандарте и часовом поясе, выполните указанные ниже команды.
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
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
При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.

- Объект [mailboxSettings](../resources/mailboxsettings.md).
- Объект [automaticRepliesSetting](../resources/automaticRepliesSetting.md).
- Объект [localeInfo](../resources/localeinfo.md).
- Строка (для параметра **timeZone**).

## <a name="example"></a>Пример
##### <a name="request-1"></a>Запрос 1
В первом примере показано, как получить все параметры почтового ящика пользователя, вошедшего в систему, в том числе параметры автоматических ответов, сведения о часовом поясе и параметры языка.
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a>Отклик 1
Отклик включает все параметры почтового ящика. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    }
}
```

##### <a name="request-2"></a>Запрос 2
Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a>Отклик 2
Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->