---
title: 'message: createReply'
description: Создайте черновик для ответа отправителю сообщения в формате JSON или MIME.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3ba7d5be91c2fdc98efdd23c95a596370ae19dc2
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870411"
---
# <a name="message-createreply"></a>message: createReply

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте черновик для ответа отправителю сообщения в формате JSON или MIME. [](../resources/message.md)

При использовании формата JSON:
- Укажите комментарий или **свойство** тела `message` параметра. При указании обоих возвращается ошибка http 400 Bad Request.
- Если replyTo указывается в исходном сообщении в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)необходимо отправить ответ получателям в **replyTo,** а не получателям из **.** 
- Вы можете [обновить проект](../api/message-update.md) позже, чтобы добавить содержимое ответа в **тело или** изменить другие свойства сообщения.

При использовании формата MIME:
- Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.
- Добавьте все вложения и свойства S/MIME в содержимое MIME.

[Отправьте](../api/message-send.md) черновик сообщения в ходе последующей операции.

Кроме того, [ответьте на сообщение в](../api/message-reply.md) одной операции.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Mail.ReadWrite    |
|Для приложений | Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание| 
|:---------------|:--------|:----------
| Authorization  | string  | Bearer {токен}. Обязательный.|
| Content-Type | string  | Характер данных в теле объекта. Обязательный.<br/> Используйте `application/json` для объекта JSON и `text/plain` для содержимого MIME.|

## <a name="request-body"></a>Текст запроса
При использовании формата JSON укажите объект JSON со следующими параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|comment|String|Добавляемый комментарий. Может быть пустой строкой.|
|message|[message](../resources/message.md)|Любые свойства, которые можно записать для обновления в ответном сообщении.|

При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными сообщениями в Интернете, все закодированные в **формате base64** в тексте запроса.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.

Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".

## <a name="examples"></a>Примеры
### <a name="example-1-create-a-draft-in-json-format-to-reply-to-an-existing-message"></a>Пример 1. Создание черновика в формате JSON для ответа на существующее сообщение
В следующем примере создается черновик ответа, добавляется комментарий и получатель в тело запроса.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group if the project is approved, please?" 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('86b6ceaf-57f7-4278-97c4-4da0a97f6cdb@70559e59-b378-49ea-8e53-07a3a3d27f5b')/messages('AAMkADA1MTAAAH5JKoAAA=')",
  "@odata.etag": "W/\"CQAAABYAAADX8oL1Wa7jQbcPAHouCzswAAAH5/DO\"",
  "id": "AAMkADA1MTAAAH5JKoAAA=",
  "subject": "RE: Let's start a group",
  "Body": {
    "contentType": "HTML",
    "content": "<html>\r\n<body>Samantha, Randi, would you name the group if the project is approved, please?\r\n<b>From:</b> Samantha Booth<br>\r\n<b>Sent:</b> Friday, March 4, 2016 12:23:35 AM<br>\r\n<b>To:</b> Admin<br>\r\n<b>Subject:</b> Re: Let's start a group</font>\r\n<p>That's a great idea!<br>\r\n</body>\r\n</html>"
  },
  "sender": {
    "emailAddress": {
      "name": "Admin",
      "address": "admin@contoso.onmicrosoft.com"
    }
  },
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress": {
        "name": "Randi Welch",
        "address": "randiw@contoso.onmicrosoft.com"
      }
    }
  ]
}
```

### <a name="example-2-create-a-draft-message-in-mime-format-to-reply-to-an-existing-message"></a>Пример 2. Создание черновика сообщения в формате MIME для ответа на существующее сообщение
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "message_createReply_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCA
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('0aaa0aa0-0000-0a00-a00a-0000009000a0')/messages/$entity",
    "@odata.etag": "W/\"AAAAAAAAAAAa00AAAa0aAaAa0a0AAAaAAAAaAa0a\"",
    "id": "AAMkADA1MTAAAAqldOAAA=",
    "createdDateTime": "2021-04-23T18:13:44Z",
    "lastModifiedDateTime": "2021-04-23T18:13:44Z",
    "changeKey": "AAAAAAAAAAAA00aaaa000aaA",
    "categories": [],
    "receivedDateTime": "2021-04-23T18:13:44Z",
    "sentDateTime": "2021-02-28T07:15:00Z",
    "hasAttachments": false,
    "internetMessageId": "<AAAAAAAAAA@AAAAAAA0001AA0000.codcod00.prod.outlook.com>",
    "subject": "Internal Resume Submission: Sales Associate",
    "bodyPreview": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here...",
    "importance": "normal",
    "parentFolderId": "LKJDSKJHkjhfakKJHFKWKKJHKJdhkjHDK==",
    "conversationId": "SDSFSmFSDGI5LWZhYjc4fsdfsd=",
    "conversationIndex": "Adfsdfsdfsdfw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": true,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkAGNhOWAvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "body": {
        "contentType": "text",
        "content": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here... Regards,Alex"
    },
    "sender": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}

```

Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


