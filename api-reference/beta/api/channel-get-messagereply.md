---
title: Получение ответа на сообщение канала
description: Получение одного ответа на сообщение в канале команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0ff885b7e2fdb8424ffef611a909955ac471ae33
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491637"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="8c86e-103">Получение ответа на сообщение канала</span><span class="sxs-lookup"><span data-stu-id="8c86e-103">Get a reply to a channel message</span></span>

<span data-ttu-id="8c86e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c86e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c86e-105">Получение одного ответа на [сообщение](../resources/chatmessage.md) в [канале](../resources/channel.md) команды.</span><span class="sxs-lookup"><span data-stu-id="8c86e-105">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c86e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c86e-106">Permissions</span></span>

<span data-ttu-id="8c86e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c86e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c86e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c86e-109">Permission Type</span></span>|<span data-ttu-id="8c86e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c86e-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="8c86e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c86e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8c86e-112">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c86e-112">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="8c86e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c86e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c86e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c86e-114">Not supported.</span></span>|
|<span data-ttu-id="8c86e-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="8c86e-115">Application</span></span>| <span data-ttu-id="8c86e-116">Чаннелмессаже. Read. Group \*, Чаннелмессаже. Read. ALL, Group. Read. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8c86e-116">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="8c86e-117">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="8c86e-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="8c86e-118">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="8c86e-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="8c86e-119">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="8c86e-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="8c86e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c86e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c86e-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c86e-121">Optional query parameters</span></span>

<span data-ttu-id="8c86e-122">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8c86e-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c86e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c86e-123">Request headers</span></span>

| <span data-ttu-id="8c86e-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c86e-124">Header</span></span>       | <span data-ttu-id="8c86e-125">Значение</span><span class="sxs-lookup"><span data-stu-id="8c86e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c86e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c86e-126">Authorization</span></span>  | <span data-ttu-id="8c86e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c86e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c86e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c86e-129">Request body</span></span>

<span data-ttu-id="8c86e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c86e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c86e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c86e-131">Response</span></span>

<span data-ttu-id="8c86e-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c86e-132">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c86e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8c86e-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8c86e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c86e-134">Request</span></span>

<span data-ttu-id="8c86e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c86e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c86e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c86e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
# <a name="c"></a>[<span data-ttu-id="8c86e-137">C#</span><span class="sxs-lookup"><span data-stu-id="8c86e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c86e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c86e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c86e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c86e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c86e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c86e-140">Response</span></span>
<span data-ttu-id="8c86e-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c86e-141">Here is an example of the response.</span></span> 

><span data-ttu-id="8c86e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c86e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
