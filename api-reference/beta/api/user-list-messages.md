---
title: Список сообщений
description: 'Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 87a5fc5f29d23b6c9a7fbbe48b059066001d5419
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177004"
---
# <a name="list-messages"></a>Список сообщений

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). 

В зависимости от размера страницы и данных почтового ящика получение сообщений из почтового ящика может повлечь множество запросов. По умолчанию страница содержит 10 сообщений. Используется `$top` для настройки размера страницы в диапазоне от 1 до 1000.

Чтобы повысить время отклика операции, укажите точные свойства. См. пример `$select` [1](#example-1-list-all-messages) ниже. Точно настройте значения для и, особенно если необходимо использовать более крупный размер страницы, так как возвращение страницы с сотнями сообщений с полными полезной нагрузкой ответа может вызвать время отклика `$select` `$top` шлюза (HTTP 504). [](/graph/errors#http-status-codes)

Для получения следующей странице с сообщениями, просто примените весь URL-адрес, возвращаемый в `@odata.nextLink`, для другого запроса на получение сообщений. Этот URL-адрес включает любые параметры запроса, которые указаны в первоначальном запросе. 

Не извлекайте значение `$skip` из URL-адреса `@odata.nextLink` для операций с ответами. Данный API использует значение `$skip` для учета всех элементов, просмотренных в почтовом ящике пользователя, и возврата элементов типа сообщение на странице. Таким образом, существует возможность, что даже в первоначальном ответе, значение `$skip` будет больше, чем размер страницы. Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)

Вы можете отфильтровать сообщения и получить [](../resources/mention.md) только те сообщения, которые содержат упоминание во включенного пользователя. См. [пример](#request-2) ниже. По умолчанию операция не возвращает свойство `GET /me/messages` **mentions.** Используйте параметр `$expand` запроса, [чтобы найти сведения о каждом упоминаемом в сообщении.](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message)

Существует два сценария, когда приложение может получить сообщения из папки почты другого пользователя:

* У приложения есть разрешения для приложений; или
* У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ. См. [подробные сведения и пример](/graph/outlook-share-messages-folders).

> **Примечание** Необходимо учитывать [известную проблему](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) с включением сообщений чата Microsoft Teams в ответ операции.
 
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail.ReadBasic, Mail.Read, Mail.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Mail.ReadBasic, Mail.Read, Mail.ReadWrite    |
|Приложение | Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

Для получения всех сообщений в почтовом ящике пользователя:

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

Для получения сообщений из определенной папки в почтовом ящике пользователя:

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

Чтобы получить все сообщения в почтовом ящике  пользователя, которые содержат упоминание пользователя:

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

Параметр запроса можно `$filter` использовать в свойстве **mentionsPreview** для получения сообщений, в которых упоминается во время выполнения действия пользователя.

### <a name="using-filter-and-orderby-in-the-same-query"></a>Использование операторов filter и orderby в одном запросе
При использовании операторов `$filter` и `$orderby` в одном запросе на получение сообщений необходимо указать свойства, соблюдая указанные ниже условия.

1. Свойства, используемые в операторе `$orderby`, также должны использоваться в операторе `$filter`. 
2. Свойства, используемые в операторе `$orderby`, представлены в том же порядке, что и для оператора `$filter`.
3. Свойства, присутствующие в операторе `$orderby`, представлены в операторе `$filter` раньше всех остальных свойств.

В противном случае возникнет следующая ошибка:

- Код ошибки: `InefficientFilter`
- Сообщение об ошибке: `The restriction or sort order is too complex for this operation.`

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Prefer: outlook.body-content-type | string | Формат возвращаемых свойств **body** и **uniqueBody**. Возможные значения: "text" или "html". Если заголовок не указан, свойства **body** и **uniqueBody** возвращаются в формате HTML. Необязательный параметр. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` объектов [сообщений](../resources/message.md) в тексте отклика.

## <a name="examples"></a>Примеры
### <a name="example-1-list-all-messages"></a>Пример 1. Список всех сообщений
#### <a name="request"></a>Запрос
В первом примере по умолчанию возвращается 10 сообщений в почтовом ящике пользователя, выписав его. `$select` используется для получения подмножества свойств каждого сообщения в ответе. 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже приведен пример отклика. Чтобы получить следующую страницу с сообщениями, примените URL-адрес, возвращенный в `@odata.nextLink`, для последующего запроса GET.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/messages?$select=sender%2csubject&$skip=14",
    "value": [
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAwR4Hg\"",
            "id": "AAMkAGUAAAwTW09AAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D1e\"",
            "id": "AAMkAGUAAAq5QKlAAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D0v\"",
            "id": "AAMkAGUAAAq5QKkAAA=",
            "subject": "Your Azure AD Identity Protection Weekly Digest",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Azure",
                    "address": "azure-noreply@contoso.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DsN\"",
            "id": "AAMkAGUAAAq5QKjAAA=",
            "subject": "Use attached file",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq9\"",
            "id": "AAMkAGUAAAq5QKiAAA=",
            "subject": "Original invitation",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq1\"",
            "id": "AAMkAGUAAAq5QKhAAA=",
            "subject": "Koala image",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dqp\"",
            "id": "AAMkAGUAAAq5QKgAAA=",
            "subject": "Sales invoice template",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessageRequest",
            "@odata.etag": "W/\"CwAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dfa\"",
            "id": "AAMkAGUAAAq5T8tAAA=",
            "subject": "Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.com"
                }
            }
        }
    ]
}
```

### <a name="example-2-use-filter-to-get-all-messages-satisfying-a-specific-condition"></a>Пример 2. Использование $filter для получения всех сообщений, удовлетворяющих определенному условию
#### <a name="request"></a>Запрос
В следующем примере фильтруются все сообщения в почтовом ящике пользователя, выписав его. Он также использует для возврата подмножество свойств каждого `$select` сообщения в ответе. 

В пример также включена кодивка URL-адресов для пробелов в строке параметра запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

### <a name="example-3-use-prefer-header-to-get-the-message-body-and-uniquebody-is-text-format"></a>Пример 3. Используйте заголовщик prefer для получения текста сообщения, а uniqueBody — текстовый формат
#### <a name="request"></a>Запрос
В третьем примере показано, как использовать заголовщик для получения текста и свойств `Prefer: outlook.body-content-type="text"` **uniqueBody** каждого сообщения  в текстовом формате.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
            "subject":"Welcome to our group!",
            "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
            "body":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
