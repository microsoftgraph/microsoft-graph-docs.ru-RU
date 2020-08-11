---
title: Отправка chatMessage в канале или чате
description: Отправка нового chatMessage в указанном канале или чате.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 402056371f5140f85838b02323b494f829d46541
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630462"
---
# <a name="send-chatmessage-in-a-channel-or-a-chat"></a>Отправка chatMessage в канале или чате

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [chatMessage](../resources/chatmessage.md) в указанном [канале](../resources/channel.md) или [чате](../resources/chat.md).

> **Note**: мы не рекомендуем использовать этот API для переноса данных. Пропускная способность, необходимая для обычной миграции, отсутствует.

> **Note**: нарушение [условий использования](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) Microsoft Teams в качестве файла журнала. Отправлять только сообщения, которые пользователи смогут читать.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-for-channel"></a>Разрешения для канала
| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Чаннелмессаже. Send, Group. ReadWrite. ALL |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

### <a name="permissions-for-chat"></a>Разрешения для чата
| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | ChatMessage. Send, Chat. ReadWrite |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

### <a name="sending-message-in-a-channel"></a>Отправка сообщения в канале
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

### <a name="sending-replies-in-a-channel"></a>Отправка ответов в канале
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

### <a name="sending-message-in-a-chat"></a>Отправка сообщения в чате
<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {код}. Обязательно. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON. Только свойство Body является обязательным; другие свойства являются необязательными.


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.

## <a name="examples"></a>Примеры

В следующих примерах URL-адрес может использовать [синтаксис HTTP](#http-request) , описанный [для отправки сообщения в чат](chat-post-message.md), [отправки сообщения в канал](channel-post-message.md)или [отправки ответа каналу](channel-post-messagereply.md).

### <a name="example-1-hello-world"></a>Пример 1: Hello World

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-mentions"></a>Пример 2: @mentions

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

### <a name="example-3-cards"></a>Пример 3: карты

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

> **Примечание:** Идентификатор вложения должен быть уникальным и может быть новым случайно созданным идентификатором GUID. Однако идентификатор вложения должен быть одинаковым в элементах _Body_ и _вложениях_ .

<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "subject": null,
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ]
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('bdb7bcda-9c3b-4341-b9a9-f52bf9a23407')/channels('19%3A786524f437c042b68bac5c0511ad6be2%40thread.skype')/messages/$entity",
    "id": "1554837297516",
    "replyToId": null,
    "etag": "1554837297516",
    "messageType": "message",
    "createdDateTime": "2019-04-09T19:14:57.516Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\n\\r\\n\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\n\\r\\n\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-4-file-attachments"></a>Пример 4: вложенные файлы

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

>**Примечание:** Файл уже должен находиться в SharePoint. Чтобы найти свойства файла, получите **driveItem** для файла. Например,/дривес/{ИД}/итемс/{ИД}. Идентификатор вложения — это идентификатор GUID в элементе **ETag** объекта **DriveItem**, вложение **ContentURL** — это **webUrl** папки **driveItem**плюс имя **driveItem**, а имя вложения — имя **driveItem**.

<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "body": {
        "contentType": "html",
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "name": "Budget.docx"
        }
    ]
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('13a99602-a5d3-4fed-99d2-7dc3ffe3730d')/channels('19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2')/messages/$entity",
    "id": "1589481435511",
    "replyToId": null,
    "etag": "1589481435511",
    "messageType": "message",
    "createdDateTime": "2020-05-14T18:37:15.511Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2/1589481435511?groupId=13a99602-a5d3-4fed-99d2-7dc3ffe3730d&tenantId=e5648b2b-1dea-445a-ab65-4f9326c2bd10&createdTime=1589481435511&parentMessageId=1589481435511",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "598efcd4-e549-402a-9602-0b50201faebe",
            "displayName": "MOD Administrator",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "content": null,
            "name": "Budget.docx",
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-5-sending-inlined-images-along-with-the-message"></a>Пример 5: отправка встроенных изображений вместе с сообщением

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

> **Примечание:** **Темпорарид** в коллекции хостедконтентс является СЛУЧАЙным идентификатором, но он должен быть одинаковым для элементов **Body** и **хостедконтентс** . (Обратите внимание, что для **темпорарид** задано значение **1** , а ссылка в основном тексте как `../hostedContents/**1**/$value` .)

для **contentBytes** должны быть заданы байты двоичных строк в кодировке Base64. Это можно сделать в C# с помощью`Convert.ToBase64String(File.ReadAllBytes("image.png"));`

<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "body": {
        "contentType": "html",
        "content": "<div><div>\n<div><span><img height=\"297\" src=\"../hostedContents/1/$value\" width=\"297\" style=\"vertical-align:bottom; width:297px; height:297px\"></span>\n\n</div>\n\n\n</div>\n</div>"
    },
    "hostedContents":[
        {
          "@microsoft.graph.temporaryId": "1",
          "contentBytes": "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",
            "contentType": "image/png"
        }
    ]
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('13a99602-a5d3-4fed-99d2-7dc3ffe3730d')/channels('19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2')/messages/$entity",
    "id": "1596261390440",
    "replyToId": null,
    "etag": "1596261390440",
    "messageType": "message",
    "createdDateTime": "2020-08-01T05:56:30.44Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2/1596261390440?groupId=13a99602-a5d3-4fed-99d2-7dc3ffe3730d&tenantId=e5648b2b-1dea-445a-ab65-4f9326c2bd10&createdTime=1596261390440&parentMessageId=1596261390440",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "598efcd4-e549-402a-9602-0b50201faebe",
            "displayName": "MOD Administrator",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<div><div>\n<div><span><img height=\"297\" src=\"https://graph.microsoft.com/beta/teams/233ae542-57e7-4593-b5bf-50549df74710/channels/19:8af03d1e70f5455fbb74d36acbe2957f@thread.tacv2/messages/1596261390440/hostedContents/aWQ9eF8wLWNhbmFyeWN1cy1kNS1jNjU0M2NjNjhkNjdlMzY1ZDUwODQ1MGU1MTRhNjEwNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLWNhbmFyeWN1cy1kNS1jNjU0M2NjNjhkNjdlMzY1ZDUwODQ1MGU1MTRhNjEwNS92aWV3cy9pbWdv/$value\" width=\"297\" style=\"vertical-align:bottom; width:297px; height:297px\"></span>\n\n</div>\n\n\n</div>\n</div>"
    },
    "channelIdentity": {
        "teamId": "13a99602-a5d3-4fed-99d2-7dc3ffe3730d",
        "channelId": "19:8af03d1e70f5455fbb74d36acbe2957f@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a>См. также

- [Ссылки на карточки](/microsoftteams/platform/concepts/cards/cards-reference)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
