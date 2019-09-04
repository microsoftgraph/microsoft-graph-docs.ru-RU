---
title: Список сообщений чата
description: 'Получение списка сообщений в чате. '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 51fbd91d521baef806ad91840e7971bc59f03bd0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719817"
---
# <a name="list-chat-messages"></a><span data-ttu-id="b9ebe-103">Список сообщений чата</span><span class="sxs-lookup"><span data-stu-id="b9ebe-103">List chat messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9ebe-104">Получение списка [сообщений](../resources/chatmessage.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="b9ebe-104">Retrieve the list of [messages](../resources/chatmessage.md) in a [chat](../resources/chat.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="b9ebe-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9ebe-105">Permissions</span></span>

<span data-ttu-id="b9ebe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9ebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9ebe-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9ebe-108">Permission type</span></span>      | <span data-ttu-id="b9ebe-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9ebe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9ebe-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9ebe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9ebe-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="b9ebe-111">Chat.Read</span></span>   |
|<span data-ttu-id="b9ebe-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9ebe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9ebe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-113">Not supported.</span></span>    |
|<span data-ttu-id="b9ebe-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="b9ebe-114">Application</span></span> | <span data-ttu-id="b9ebe-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9ebe-115">Chat.Read.All</span></span>   |

> [!NOTE]
> <span data-ttu-id="b9ebe-116">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="b9ebe-117">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="b9ebe-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="b9ebe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9ebe-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}/messages
GET /users/{id}/chats/{id}/messages
GET /chats/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9ebe-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9ebe-119">Optional query parameters</span></span>

<span data-ttu-id="b9ebe-120">Это действие в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-120">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9ebe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9ebe-121">Request headers</span></span>

| <span data-ttu-id="b9ebe-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9ebe-122">Header</span></span>       | <span data-ttu-id="b9ebe-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b9ebe-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9ebe-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9ebe-124">Authorization</span></span>  | <span data-ttu-id="b9ebe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9ebe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9ebe-127">Request body</span></span>

<span data-ttu-id="b9ebe-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9ebe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9ebe-129">Response</span></span>

<span data-ttu-id="b9ebe-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-130">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9ebe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b9ebe-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b9ebe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9ebe-132">Request</span></span>

<span data-ttu-id="b9ebe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b9ebe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9ebe-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b9ebe-135">C#</span><span class="sxs-lookup"><span data-stu-id="b9ebe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9ebe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9ebe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b9ebe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9ebe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9ebe-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9ebe-138">Response</span></span>
<span data-ttu-id="b9ebe-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-139">Here is an example of the response.</span></span> 

><span data-ttu-id="b9ebe-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9ebe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf%40unq.gbl.spaces')/messages",
    "@odata.count": 4,
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces/messages?$skiptoken=M2Y1YjAwMDAwMDMxMzkzYTM4NjIzMDM4MzE2NTY2MzYyZDM0MzczOTMyMmQzNDY0NjU2NjJkNjIzMjYzMzkyZDYzMzMzNjMzNjEzMTYyNjYzNDMxNjQzNTVmMzgzNzM3MzEzOTMyNjI2NDJkMzkzMTM4MzMyZDM0Mzc2NDMzMmQ2MTM3MzQ2MzJkMzg2MTYxMzAzNDMyMzYzNzMxMzY2MzY2NDA3NTZlNzEyZTY3NjI2YzJlNzM3MDYxNjM2NTczMDE5N2Y3ZGMzMjZhMDEwMDAwMDg1YjNmNGI2YTAxMDAwMDAwfDE1NTU2MzE3MjIxNDc%3d",
    "value": [
        {
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
                "content": "<attachment id=\"a7bda643d32b4541b74ec1f4ace7f391\"></attachment>"
            },
            "attachments": [
                {
                    "id": "a7bda643d32b4541b74ec1f4ace7f391",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f7695632ce6ca4b0da2e3ae15fea54c47\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631540287",
            "replyToId": null,
            "etag": "1555631540287",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:52:20.287Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
                    "displayName": "MOD Administrator",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "yo"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631512068",
            "replyToId": null,
            "etag": "1555631512068",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:51:52.068Z",
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
                "content": "<attachment id=\"6309ad5424a04c5899efd130342b165a\"></attachment>"
            },
            "attachments": [
                {
                    "id": "6309ad5424a04c5899efd130342b165a",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f978574f2993640bf9cbc5e438824a645\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1555631511115",
            "replyToId": null,
            "etag": "1555631511115",
            "messageType": "message",
            "createdDateTime": "2019-04-18T23:51:51.115Z",
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
                "content": "<attachment id=\"9b6e6d3bde7741bcac561bb15ec2721b\"></attachment>"
            },
            "attachments": [
                {
                    "id": "9b6e6d3bde7741bcac561bb15ec2721b",
                    "contentType": "application/vnd.microsoft.card.signin",
                    "contentUrl": null,
                    "content": "{\r\n  \"text\": \"Please sign in to sample to proceed.\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"signin\",\r\n      \"title\": \"Sign In\",\r\n      \"value\": \"https://token.botframework.com/api/oauth/signin?signin=921d46120f01039912d88040739e2780ef54656557\"\r\n    }\r\n  ]\r\n}",
                    "name": null,
                    "thumbnailUrl": null
                }
            ],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
