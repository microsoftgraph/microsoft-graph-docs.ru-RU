---
title: Создание объекта chatMessage в канале
description: Создание нового chatMessage в указанном канале.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a764a7190432b838bdd982b4275fe6dca897ba56
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868186"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="4936d-103">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="4936d-103">Create chatMessage in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4936d-104">Создание нового [chatMessage](../resources/chatmessage.md) в указанном [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="4936d-104">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="4936d-105">**Note**: мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="4936d-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="4936d-106">Пропускная способность, необходимая для обычной миграции, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="4936d-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="4936d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4936d-107">Permissions</span></span>

<span data-ttu-id="4936d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4936d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4936d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4936d-110">Permission type</span></span>                        | <span data-ttu-id="4936d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4936d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4936d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4936d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4936d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4936d-113">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4936d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4936d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4936d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4936d-115">Not supported.</span></span> |
| <span data-ttu-id="4936d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4936d-116">Application</span></span>                            | <span data-ttu-id="4936d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4936d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4936d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4936d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="4936d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4936d-119">Request headers</span></span>

| <span data-ttu-id="4936d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4936d-120">Name</span></span>          | <span data-ttu-id="4936d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4936d-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4936d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4936d-122">Authorization</span></span> | <span data-ttu-id="4936d-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4936d-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4936d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4936d-124">Request body</span></span>

<span data-ttu-id="4936d-125">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4936d-125">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="4936d-126">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="4936d-126">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="4936d-127">Note: отправка сообщений с вложениями и изображениями не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4936d-127">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="4936d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4936d-128">Response</span></span>

<span data-ttu-id="4936d-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4936d-129">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4936d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="4936d-130">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="4936d-131">Пример 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="4936d-131">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="4936d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4936d-132">Request</span></span>
<span data-ttu-id="4936d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4936d-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4936d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4936d-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4936d-135">C#</span><span class="sxs-lookup"><span data-stu-id="4936d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4936d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4936d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4936d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4936d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4936d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4936d-138">Response</span></span>

<span data-ttu-id="4936d-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4936d-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4936d-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4936d-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4936d-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4936d-141">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-mentions"></a><span data-ttu-id="4936d-142">Пример 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="4936d-142">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="4936d-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4936d-143">Request</span></span>
<span data-ttu-id="4936d-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4936d-144">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="4936d-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="4936d-145">Response</span></span>

<span data-ttu-id="4936d-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4936d-146">The following is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="4936d-147">Пример 3: карты</span><span class="sxs-lookup"><span data-stu-id="4936d-147">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="4936d-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4936d-148">Request</span></span>
<span data-ttu-id="4936d-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4936d-149">The following is an example of the request.</span></span>

> <span data-ttu-id="4936d-150">Note: идентификатор вложения должен быть уникальным и может быть новым случайно созданным идентификатором GUID.</span><span class="sxs-lookup"><span data-stu-id="4936d-150">Note: The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="4936d-151">Однако идентификатор вложения должен быть одинаковым в элементах _Body_ и _вложениях_ .</span><span class="sxs-lookup"><span data-stu-id="4936d-151">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>

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

#### <a name="response"></a><span data-ttu-id="4936d-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="4936d-152">Response</span></span>

<span data-ttu-id="4936d-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4936d-153">The following is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4936d-154">См. также</span><span class="sxs-lookup"><span data-stu-id="4936d-154">See also</span></span>

- [<span data-ttu-id="4936d-155">Справочник по карточкам</span><span class="sxs-lookup"><span data-stu-id="4936d-155">Cards Reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)

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
