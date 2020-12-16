---
title: Получение объекта chatMessage
description: Получение одного сообщения в чате.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 17b030552f110f4d884c81f14668f7e0183b4abf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958326"
---
# <a name="get-chatmessage"></a><span data-ttu-id="5cf23-103">Получение объекта chatMessage</span><span class="sxs-lookup"><span data-stu-id="5cf23-103">Get chatMessage</span></span>

<span data-ttu-id="5cf23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cf23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf23-105">Получение одного [сообщения](../resources/chatmessage.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="5cf23-105">Retrieve a single [message](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5cf23-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cf23-106">Permissions</span></span>

<span data-ttu-id="5cf23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cf23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cf23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cf23-109">Permission type</span></span>      | <span data-ttu-id="5cf23-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cf23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cf23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cf23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5cf23-112">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cf23-112">Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="5cf23-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cf23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cf23-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cf23-114">Not supported.</span></span>    |
|<span data-ttu-id="5cf23-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="5cf23-115">Application</span></span> | <span data-ttu-id="5cf23-116">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cf23-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="5cf23-117">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="5cf23-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="5cf23-118">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="5cf23-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="5cf23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cf23-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
GET /chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cf23-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5cf23-120">Optional query parameters</span></span>

<span data-ttu-id="5cf23-121">Это действие в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5cf23-121">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cf23-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cf23-122">Request headers</span></span>
| <span data-ttu-id="5cf23-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cf23-123">Header</span></span>       | <span data-ttu-id="5cf23-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5cf23-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5cf23-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cf23-125">Authorization</span></span>  | <span data-ttu-id="5cf23-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cf23-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cf23-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cf23-128">Request body</span></span>
<span data-ttu-id="5cf23-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cf23-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cf23-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cf23-130">Response</span></span>

<span data-ttu-id="5cf23-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cf23-131">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cf23-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5cf23-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cf23-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cf23-133">Request</span></span>
<span data-ttu-id="5cf23-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cf23-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5cf23-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5cf23-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/{id}/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="5cf23-136">C#</span><span class="sxs-lookup"><span data-stu-id="5cf23-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5cf23-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cf23-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5cf23-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cf23-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5cf23-139">Java</span><span class="sxs-lookup"><span data-stu-id="5cf23-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5cf23-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cf23-140">Response</span></span>
<span data-ttu-id="5cf23-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5cf23-141">Here is an example of the response.</span></span> 

><span data-ttu-id="5cf23-142">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5cf23-142">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="5cf23-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cf23-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf%40unq.gbl.spaces')/messages/$entity",
    "id": "1555631722147",
    "replyToId": null,
    "etag": "1555631722147",
    "messageType": "message",
    "createdDateTime": "2019-04-18T23:55:22.147Z",
    "lastModifiedDateTime": "2019-05-18T23:55:22.147Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "device": null,
        "user": null,
        "conversation": null,
        "application": {
            "id": "877192bd-9183-47d3-a74c-8aa0426716cf",
            "displayName": "TestBot",
            "applicationIdentityType": "bot"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"bcb243ec589a4537b3c650356421e696\"></attachment>"
    },
    "attachments": [
        {
            "id": "bcb243ec589a4537b3c650356421e696",
            "contentType": "application/vnd.microsoft.card.signin",
            "contentUrl": null,
            "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f7695632ce6ca4b0da2e3ae15fea54c47\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


