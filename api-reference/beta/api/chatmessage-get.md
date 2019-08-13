---
title: Получение объекта chatMessage
description: Получение одного сообщения в чате.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e3fadc893e67a583b370059513f7e6bf91fd3abc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321715"
---
# <a name="get-chatmessage"></a><span data-ttu-id="0e988-103">Получение объекта chatMessage</span><span class="sxs-lookup"><span data-stu-id="0e988-103">Get chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e988-104">Получение одного [сообщения](../resources/chatmessage.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="0e988-104">Retrieve a single [message](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e988-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e988-105">Permissions</span></span>

<span data-ttu-id="0e988-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e988-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e988-108">Permission type</span></span>      | <span data-ttu-id="0e988-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e988-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e988-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e988-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e988-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e988-111">Chat.Read, Chat.ReadWrite</span></span>   |
|<span data-ttu-id="0e988-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e988-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e988-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e988-113">Not supported.</span></span>    |
|<span data-ttu-id="0e988-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e988-114">Application</span></span> | <span data-ttu-id="0e988-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e988-115">Chat.Read.All</span></span>   |

> [!NOTE]
> <span data-ttu-id="0e988-116">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="0e988-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="0e988-117">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="0e988-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="0e988-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e988-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
GET /chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e988-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0e988-119">Optional query parameters</span></span>

<span data-ttu-id="0e988-120">Это действие в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0e988-120">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e988-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e988-121">Request headers</span></span>
| <span data-ttu-id="0e988-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e988-122">Header</span></span>       | <span data-ttu-id="0e988-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0e988-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e988-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e988-124">Authorization</span></span>  | <span data-ttu-id="0e988-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e988-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e988-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e988-127">Request body</span></span>
<span data-ttu-id="0e988-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e988-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e988-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e988-129">Response</span></span>

<span data-ttu-id="0e988-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e988-130">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e988-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0e988-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e988-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e988-132">Request</span></span>
<span data-ttu-id="0e988-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e988-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0e988-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e988-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e988-135">C#</span><span class="sxs-lookup"><span data-stu-id="0e988-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e988-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e988-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e988-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e988-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0e988-138">Java</span><span class="sxs-lookup"><span data-stu-id="0e988-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e988-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e988-139">Response</span></span>
<span data-ttu-id="0e988-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e988-140">Here is an example of the response.</span></span> 

><span data-ttu-id="0e988-141">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0e988-141">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="0e988-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e988-142">All the properties will be returned from an actual call.</span></span>
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
    "lastModifiedDateTime": null,
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
