# <a name="user-getmailtips"></a>user: getMailTips

Получение подсказки (MailTips) для одного или нескольких получателей, доступных для вошедшего в систему [пользователя](../resources/user.md) .

Обратите внимание, что при помощи вызова `POST` действия `getMailTips` можно запросить возврат определенного типа подсказок (MailTips) для нескольких получателей за один раз. Запрошенные подсказки (MailTips) возвращаются в коллекцию [mailTips](../resources/mailtips.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail.Read Mail.Read.Shared    |
|Делегированные (личная учетная запись Майкрософт) | Mail.Read    |
|Для приложений | Mail.Read |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение|
|:-----------  |:------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите JSON-объект с указанными ниже параметрами.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|EmailAddresses|Коллекция String|Коллекция SMTP-адресов получателей для получения подсказок (MailTips).|
|MailTipsOptions|String (строка)|Перечисление флагов, которое представляет запрошенные подсказки. Возможные значения: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions` и `totalMemberCount`.|

## <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailTips](../resources/mailtips.md) в теле отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Следующий пример демонстрирует получение подсказок (MailTips) для указанных получателей, для любых параметров автоматического ответа и состояния переполненности почтового ящика.

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
