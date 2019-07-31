---
title: Получение ответа на сообщение канала
description: Получение одного ответа на сообщение в канале команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 50f371f9fa1d98d2e8fae17def4dc23158bad97b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944319"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="7a85c-103">Получение ответа на сообщение канала</span><span class="sxs-lookup"><span data-stu-id="7a85c-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a85c-104">Получение одного ответа на [сообщение](../resources/chatmessage.md) в канале команды [](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="7a85c-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a85c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a85c-105">Permissions</span></span>

<span data-ttu-id="7a85c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a85c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a85c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a85c-108">Permission Type</span></span>|<span data-ttu-id="7a85c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a85c-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="7a85c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a85c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7a85c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a85c-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="7a85c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a85c-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a85c-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7a85c-113">Not supported</span></span>|
|<span data-ttu-id="7a85c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a85c-114">Application</span></span>| <span data-ttu-id="7a85c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a85c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="7a85c-116">Перед вызовом этого API с разрешениями для приложений необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="7a85c-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="7a85c-117">Дополнительные сведения см [в разделе protected API в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="7a85c-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="7a85c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a85c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a85c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a85c-119">Optional query parameters</span></span>

<span data-ttu-id="7a85c-120">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="7a85c-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a85c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a85c-121">Request headers</span></span>

| <span data-ttu-id="7a85c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a85c-122">Header</span></span>       | <span data-ttu-id="7a85c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7a85c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a85c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a85c-124">Authorization</span></span>  | <span data-ttu-id="7a85c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a85c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a85c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7a85c-127">Request body</span></span>

<span data-ttu-id="7a85c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a85c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a85c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a85c-129">Response</span></span>

<span data-ttu-id="7a85c-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a85c-130">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a85c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7a85c-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7a85c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a85c-132">Request</span></span>

<span data-ttu-id="7a85c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a85c-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a85c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a85c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a85c-135">C#</span><span class="sxs-lookup"><span data-stu-id="7a85c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a85c-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a85c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a85c-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7a85c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a85c-138">Java</span><span class="sxs-lookup"><span data-stu-id="7a85c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-message-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a85c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a85c-139">Response</span></span>
<span data-ttu-id="7a85c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7a85c-140">Here is an example of the response.</span></span> 

><span data-ttu-id="7a85c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a85c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies/$entity",
    "id": "1555377090002",
    "replyToId": "1555375673184",
    "etag": "1555377090002",
    "messageType": "message",
    "createdDateTime": "2019-04-16T01:11:30.002Z",
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
            "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
            "displayName": "Adele Vance",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Megan",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                    "displayName": "Megan",
                    "userIdentityType": "aadUser"
                }
            }
        },
        {
            "id": 1,
            "mentionText": "Alex",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                    "displayName": "Alex",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a reply to a channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
