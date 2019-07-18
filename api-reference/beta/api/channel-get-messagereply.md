---
title: Получение ответа на сообщение канала
description: Получение одного ответа на сообщение в канале команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4f5efcb73b6b0f9b23ab8157fbc4a1b3b1271785
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778420"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="1ccd3-103">Получение ответа на сообщение канала</span><span class="sxs-lookup"><span data-stu-id="1ccd3-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ccd3-104">Получение одного ответа на [сообщение](../resources/chatmessage.md) в канале команды [](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="1ccd3-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ccd3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ccd3-105">Permissions</span></span>

<span data-ttu-id="1ccd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ccd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ccd3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ccd3-108">Permission Type</span></span>|<span data-ttu-id="1ccd3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ccd3-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="1ccd3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ccd3-110">Delegated (work or school account)</span></span>|<span data-ttu-id="1ccd3-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ccd3-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="1ccd3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ccd3-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ccd3-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1ccd3-113">Not supported</span></span>|
|<span data-ttu-id="1ccd3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ccd3-114">Application</span></span>| <span data-ttu-id="1ccd3-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ccd3-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="1ccd3-116">Перед вызовом этого API с разрешениями для приложений необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="1ccd3-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="1ccd3-117">Дополнительные сведения см [в разделе protected API в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="1ccd3-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="1ccd3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ccd3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ccd3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ccd3-119">Optional query parameters</span></span>

<span data-ttu-id="1ccd3-120">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="1ccd3-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ccd3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ccd3-121">Request headers</span></span>

| <span data-ttu-id="1ccd3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ccd3-122">Header</span></span>       | <span data-ttu-id="1ccd3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1ccd3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ccd3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ccd3-124">Authorization</span></span>  | <span data-ttu-id="1ccd3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ccd3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ccd3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ccd3-127">Request body</span></span>

<span data-ttu-id="1ccd3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ccd3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ccd3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ccd3-129">Response</span></span>

<span data-ttu-id="1ccd3-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ccd3-130">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ccd3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1ccd3-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1ccd3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ccd3-132">Request</span></span>

<span data-ttu-id="1ccd3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ccd3-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1ccd3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ccd3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ccd3-135">C#</span><span class="sxs-lookup"><span data-stu-id="1ccd3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ccd3-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ccd3-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1ccd3-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1ccd3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1ccd3-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ccd3-138">Response</span></span>
<span data-ttu-id="1ccd3-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ccd3-139">Here is an example of the response.</span></span> 

><span data-ttu-id="1ccd3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ccd3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
