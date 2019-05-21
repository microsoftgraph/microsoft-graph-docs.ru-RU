---
title: Получение сообщения в канале
description: Получение одного сообщения (без ответов) в канале команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 48ff7af72e630973ef120808e407cce44d379f2b
ms.sourcegitcommit: abca7fcefeaa74b50f4600b35d816b626ba08468
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2019
ms.locfileid: "34310813"
---
# <a name="get-channel-message"></a><span data-ttu-id="4c349-103">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="4c349-103">Get channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c349-104">Получение одного [сообщения](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) команды.</span><span class="sxs-lookup"><span data-stu-id="4c349-104">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c349-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c349-105">Permissions</span></span>
<span data-ttu-id="4c349-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c349-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c349-108">Permission Type</span></span>|<span data-ttu-id="4c349-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c349-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="4c349-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c349-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4c349-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c349-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="4c349-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c349-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c349-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4c349-113">Not supported</span></span>|
|<span data-ttu-id="4c349-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c349-114">Application</span></span>| <span data-ttu-id="4c349-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c349-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c349-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c349-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c349-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c349-117">Optional query parameters</span></span>
<span data-ttu-id="4c349-118">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="4c349-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c349-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c349-119">Request headers</span></span>
| <span data-ttu-id="4c349-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c349-120">Header</span></span>       | <span data-ttu-id="4c349-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4c349-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c349-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c349-122">Authorization</span></span>  | <span data-ttu-id="4c349-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c349-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c349-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c349-125">Request body</span></span>
<span data-ttu-id="4c349-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c349-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c349-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c349-127">Response</span></span>

<span data-ttu-id="4c349-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c349-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c349-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4c349-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c349-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c349-130">Request</span></span>
<span data-ttu-id="4c349-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c349-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184
```
##### <a name="response"></a><span data-ttu-id="4c349-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c349-132">Response</span></span>
<span data-ttu-id="4c349-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c349-133">Here is an example of the response.</span></span> 

><span data-ttu-id="4c349-134">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c349-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="4c349-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c349-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages/$entity",
    "id": "1555375673184",
    "replyToId": null,
    "etag": "1555375673184",
    "messageType": "message",
    "createdDateTime": "2019-04-16T00:47:53.184Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": "",
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "webUrl": "https://teams.microsoft.com/l/message/19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype/1555375673184?groupId=303d2c1c-f1c5-40ce-b68e-544343d7f42b&tenantId=123d12b3-1234-12ab-b1a2-123ba45c6789&createdTime=1555375673184&parentMessageId=1555375673188",       
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
        "content": "<div><div>Nice to join this team. <at id=\"0\">Megan Bowen</at>, have we got the March report ready please?</div>\n</div>"
    },
    "attachments": [
        {
            "id": "5e32f195-168a-474f-a273-123123123",
            "contentType": "reference",
            "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
            "content": null,
            "name": "Test.txt",
            "thumbnailUrl": null
        }
    ],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Megan Bowen",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                    "displayName": "Megan Bowen",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": [
      {
        "reactionType": "like",
        "user": {
            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
            "displayName": "Megan Bowen",
            "userIdentityType": "aadUser"
        },
        "createdDateTime": "2019-04-16T00:58:53.184Z"
      }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c349-136">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="4c349-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4c349-137">C#</span><span class="sxs-lookup"><span data-stu-id="4c349-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c349-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c349-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
