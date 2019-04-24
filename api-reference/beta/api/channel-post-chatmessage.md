---
title: Отправка сообщения в канал
description: Отправка нового сообщения в указанном канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c0ee2535cf9e47b08e1eb44d8fa9b07fb078c2bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456523"
---
# <a name="send-a-message-to-a-channel"></a><span data-ttu-id="77101-103">Отправка сообщения в канал</span><span class="sxs-lookup"><span data-stu-id="77101-103">Send a message to a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77101-104">Создайте новое [сообщение](../resources/chatmessage.md) в заданном [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="77101-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="77101-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77101-105">Permissions</span></span>
<span data-ttu-id="77101-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77101-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77101-108">Permission type</span></span>      | <span data-ttu-id="77101-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77101-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77101-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77101-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77101-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77101-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="77101-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77101-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77101-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77101-113">Not supported.</span></span>    |
|<span data-ttu-id="77101-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77101-114">Application</span></span> | <span data-ttu-id="77101-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77101-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77101-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77101-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="77101-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77101-117">Request headers</span></span>
| <span data-ttu-id="77101-118">Имя</span><span class="sxs-lookup"><span data-stu-id="77101-118">Name</span></span>       | <span data-ttu-id="77101-119">Тип</span><span class="sxs-lookup"><span data-stu-id="77101-119">Type</span></span> | <span data-ttu-id="77101-120">Описание</span><span class="sxs-lookup"><span data-stu-id="77101-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="77101-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="77101-121">Authorization</span></span>  | <span data-ttu-id="77101-122">string</span><span class="sxs-lookup"><span data-stu-id="77101-122">string</span></span>  | <span data-ttu-id="77101-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77101-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77101-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77101-125">Request body</span></span>
<span data-ttu-id="77101-126">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77101-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="77101-127">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="77101-127">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="77101-128">Note: отправка сообщений с вложениями и изображениями не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77101-128">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="77101-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="77101-129">Response</span></span>

<span data-ttu-id="77101-130">В случае успешного выполнения этот метод `201 Created` возвращает код отклика с созданным [сообщением](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="77101-130">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="77101-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="77101-131">Examples</span></span> 

### <a name="example-1-hello-world"></a><span data-ttu-id="77101-132">Пример 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="77101-132">Example 1: Hello World</span></span>

##### <a name="request"></a><span data-ttu-id="77101-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="77101-133">Request</span></span>
<span data-ttu-id="77101-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77101-134">Here is an example of the request.</span></span>
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
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="77101-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="77101-135">Response</span></span>

<span data-ttu-id="77101-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77101-136">Here is an example of the response.</span></span>
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

### <a name="example-2-mentions"></a><span data-ttu-id="77101-137">Пример 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="77101-137">Example 2: @mentions</span></span>

##### <a name="request"></a><span data-ttu-id="77101-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="77101-138">Request</span></span>
<span data-ttu-id="77101-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77101-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="77101-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="77101-140">Response</span></span>

<span data-ttu-id="77101-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77101-141">Here is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="77101-142">Пример 3: карты</span><span class="sxs-lookup"><span data-stu-id="77101-142">Example 3: Cards</span></span>

##### <a name="request"></a><span data-ttu-id="77101-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="77101-143">Request</span></span>
<span data-ttu-id="77101-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77101-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="77101-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="77101-145">Response</span></span>

<span data-ttu-id="77101-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77101-146">Here is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="77101-147">См. также</span><span class="sxs-lookup"><span data-stu-id="77101-147">See also</span></span>

- [<span data-ttu-id="77101-148">Справочник по карточкам</span><span class="sxs-lookup"><span data-stu-id="77101-148">Cards Reference</span></span>](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards-reference)

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
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
