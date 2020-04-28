---
title: Получение ответа на сообщение канала
description: Получение одного ответа на сообщение в канале команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c6dff7204068f6c9ebb3397cc8e745229e399efa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440348"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="7c3d1-103">Получение ответа на сообщение канала</span><span class="sxs-lookup"><span data-stu-id="7c3d1-103">Get a reply to a channel message</span></span>

<span data-ttu-id="7c3d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c3d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c3d1-105">Получение одного ответа на [сообщение](../resources/chatmessage.md) в [канале](../resources/channel.md) команды.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-105">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c3d1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c3d1-106">Permissions</span></span>

<span data-ttu-id="7c3d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c3d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c3d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c3d1-109">Permission Type</span></span>|<span data-ttu-id="7c3d1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c3d1-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="7c3d1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c3d1-111">Delegated (work or school account)</span></span>| <span data-ttu-id="7c3d1-112">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c3d1-112">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="7c3d1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c3d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c3d1-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c3d1-114">Not supported</span></span>|
|<span data-ttu-id="7c3d1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c3d1-115">Application</span></span>| <span data-ttu-id="7c3d1-116">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c3d1-116">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="7c3d1-117">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="7c3d1-118">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="7c3d1-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="7c3d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c3d1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c3d1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7c3d1-120">Optional query parameters</span></span>

<span data-ttu-id="7c3d1-121">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-121">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c3d1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c3d1-122">Request headers</span></span>

| <span data-ttu-id="7c3d1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c3d1-123">Header</span></span>       | <span data-ttu-id="7c3d1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7c3d1-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c3d1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c3d1-125">Authorization</span></span>  | <span data-ttu-id="7c3d1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c3d1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c3d1-128">Request body</span></span>

<span data-ttu-id="7c3d1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c3d1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c3d1-130">Response</span></span>

<span data-ttu-id="7c3d1-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-131">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c3d1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7c3d1-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7c3d1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c3d1-133">Request</span></span>

<span data-ttu-id="7c3d1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c3d1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c3d1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
# <a name="c"></a>[<span data-ttu-id="7c3d1-136">C#</span><span class="sxs-lookup"><span data-stu-id="7c3d1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c3d1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c3d1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c3d1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c3d1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7c3d1-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c3d1-139">Response</span></span>
<span data-ttu-id="7c3d1-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-140">Here is an example of the response.</span></span> 

><span data-ttu-id="7c3d1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c3d1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
