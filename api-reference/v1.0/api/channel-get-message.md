---
title: Получение сообщения в канале
description: Получение одного сообщения (без ответов) в канале команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3363d252bb58302e8446c01212b7bd2178d43fa9
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115178"
---
# <a name="get-channel-message"></a><span data-ttu-id="3fd1c-103">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="3fd1c-103">Get channel message</span></span>

<span data-ttu-id="3fd1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fd1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fd1c-105">Получение одного [сообщения](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) команды.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-105">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fd1c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fd1c-106">Permissions</span></span>
<span data-ttu-id="3fd1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fd1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fd1c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fd1c-109">Permission Type</span></span>|<span data-ttu-id="3fd1c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fd1c-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3fd1c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fd1c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="3fd1c-112">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fd1c-112">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="3fd1c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fd1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fd1c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-114">Not supported.</span></span>|
|<span data-ttu-id="3fd1c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fd1c-115">Application</span></span>| <span data-ttu-id="3fd1c-116">ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="3fd1c-116">ChannelMessage.Read.Group\*</span></span> |

> <span data-ttu-id="3fd1c-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="3fd1c-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="3fd1c-118">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="3fd1c-119">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="3fd1c-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="3fd1c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fd1c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fd1c-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3fd1c-121">Optional query parameters</span></span>
<span data-ttu-id="3fd1c-122">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fd1c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fd1c-123">Request headers</span></span>
| <span data-ttu-id="3fd1c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fd1c-124">Header</span></span>       | <span data-ttu-id="3fd1c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="3fd1c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3fd1c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fd1c-126">Authorization</span></span>  | <span data-ttu-id="3fd1c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3fd1c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fd1c-129">Request body</span></span>
<span data-ttu-id="3fd1c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fd1c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fd1c-131">Response</span></span>

<span data-ttu-id="3fd1c-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-132">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fd1c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3fd1c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fd1c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fd1c-134">Request</span></span>
<span data-ttu-id="3fd1c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3fd1c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fd1c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184
```
# <a name="c"></a>[<span data-ttu-id="3fd1c-137">C#</span><span class="sxs-lookup"><span data-stu-id="3fd1c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fd1c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fd1c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fd1c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fd1c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fd1c-140">Java</span><span class="sxs-lookup"><span data-stu-id="3fd1c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3fd1c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fd1c-141">Response</span></span>
<span data-ttu-id="3fd1c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-142">Here is an example of the response.</span></span> 

><span data-ttu-id="3fd1c-143">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-143">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="3fd1c-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fd1c-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages/$entity",
    "id": "1555375673184",
    "replyToId": null,
    "etag": "1555375673184",
    "messageType": "message",
    "createdDateTime": "2019-04-16T00:47:53.184Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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
  ]
}
-->


