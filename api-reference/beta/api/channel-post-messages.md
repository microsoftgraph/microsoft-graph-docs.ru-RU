---
title: Создание chatMessage в канале
description: Создание нового chatMessage в указанном канале.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 15405b437a629eece2a974863e2c71f146c3bb3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944214"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="2613f-103">Создание chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="2613f-103">Create chatMessage in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2613f-104">Создание нового [chatMessage](../resources/chatmessage.md) в указанном [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="2613f-104">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="2613f-105">**Note**: мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="2613f-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="2613f-106">Пропускная способность, необходимая для обычной миграции, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="2613f-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="2613f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2613f-107">Permissions</span></span>

<span data-ttu-id="2613f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2613f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2613f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2613f-110">Permission type</span></span>                        | <span data-ttu-id="2613f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2613f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2613f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2613f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2613f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2613f-113">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2613f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2613f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2613f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2613f-115">Not supported.</span></span> |
| <span data-ttu-id="2613f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2613f-116">Application</span></span>                            | <span data-ttu-id="2613f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2613f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2613f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2613f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="2613f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2613f-119">Request headers</span></span>

| <span data-ttu-id="2613f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2613f-120">Name</span></span>          | <span data-ttu-id="2613f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2613f-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2613f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2613f-122">Authorization</span></span> | <span data-ttu-id="2613f-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2613f-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2613f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2613f-124">Request body</span></span>

<span data-ttu-id="2613f-125">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2613f-125">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="2613f-126">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="2613f-126">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="2613f-127">Note: отправка сообщений с вложениями и изображениями не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2613f-127">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="2613f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2613f-128">Response</span></span>

<span data-ttu-id="2613f-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2613f-129">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2613f-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2613f-130">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="2613f-131">Пример 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="2613f-131">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="2613f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2613f-132">Request</span></span>
<span data-ttu-id="2613f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2613f-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2613f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2613f-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2613f-135">C#</span><span class="sxs-lookup"><span data-stu-id="2613f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2613f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="2613f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2613f-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2613f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2613f-138">Java</span><span class="sxs-lookup"><span data-stu-id="2613f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2613f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2613f-139">Response</span></span>

<span data-ttu-id="2613f-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2613f-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2613f-141">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2613f-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2613f-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2613f-142">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-mentions"></a><span data-ttu-id="2613f-143">Пример 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="2613f-143">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="2613f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2613f-144">Request</span></span>
<span data-ttu-id="2613f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2613f-145">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="2613f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2613f-146">Response</span></span>

<span data-ttu-id="2613f-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2613f-147">The following is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="2613f-148">Пример 3: карты</span><span class="sxs-lookup"><span data-stu-id="2613f-148">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="2613f-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2613f-149">Request</span></span>
<span data-ttu-id="2613f-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2613f-150">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="2613f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2613f-151">Response</span></span>

<span data-ttu-id="2613f-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2613f-152">The following is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2613f-153">См. также</span><span class="sxs-lookup"><span data-stu-id="2613f-153">See also</span></span>

- [<span data-ttu-id="2613f-154">Справочник по карточкам</span><span class="sxs-lookup"><span data-stu-id="2613f-154">Cards Reference</span></span>](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards-reference)

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
