---
title: Получение ответа на сообщение канала
description: Получение одного ответа на сообщение в канале команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4d0ec855b2b91ce9ee912725140e7222c32ff630
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262113"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="51653-103">Получение ответа на сообщение канала</span><span class="sxs-lookup"><span data-stu-id="51653-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51653-104">Получение одного ответа на [сообщение](../resources/chatmessage.md) в канале команды [](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="51653-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="51653-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51653-105">Permissions</span></span>

<span data-ttu-id="51653-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51653-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51653-108">Permission Type</span></span>|<span data-ttu-id="51653-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51653-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="51653-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51653-110">Delegated (work or school account)</span></span>|<span data-ttu-id="51653-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51653-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="51653-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51653-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51653-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="51653-113">Not supported</span></span>|
|<span data-ttu-id="51653-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51653-114">Application</span></span>| <span data-ttu-id="51653-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51653-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51653-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51653-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51653-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51653-117">Optional query parameters</span></span>

<span data-ttu-id="51653-118">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="51653-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51653-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51653-119">Request headers</span></span>

| <span data-ttu-id="51653-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51653-120">Header</span></span>       | <span data-ttu-id="51653-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51653-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51653-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51653-122">Authorization</span></span>  | <span data-ttu-id="51653-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51653-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51653-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51653-125">Request body</span></span>

<span data-ttu-id="51653-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51653-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51653-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="51653-127">Response</span></span>

<span data-ttu-id="51653-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51653-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51653-129">Пример</span><span class="sxs-lookup"><span data-stu-id="51653-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="51653-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="51653-130">Request</span></span>

<span data-ttu-id="51653-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51653-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
##### <a name="response"></a><span data-ttu-id="51653-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="51653-132">Response</span></span>
<span data-ttu-id="51653-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51653-133">Here is an example of the response.</span></span> 

><span data-ttu-id="51653-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51653-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="51653-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="51653-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="51653-137">C#</span><span class="sxs-lookup"><span data-stu-id="51653-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51653-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="51653-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="51653-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="51653-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
