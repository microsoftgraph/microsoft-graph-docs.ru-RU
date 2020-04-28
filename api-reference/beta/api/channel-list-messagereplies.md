---
title: Список ответов на сообщения канала
description: Перечисление всех ответов на сообщение в канале команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1d1fc22e939e15353a033b7bae2691fc2d375a50
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43179012"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="92145-103">Список ответов на сообщения канала</span><span class="sxs-lookup"><span data-stu-id="92145-103">List channel message replies</span></span>

<span data-ttu-id="92145-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92145-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92145-105">Перечисление всех ответов на [сообщение](../resources/chatmessage.md) в [канале](../resources/channel.md) команды.</span><span class="sxs-lookup"><span data-stu-id="92145-105">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="92145-106">Этот метод перечисляет только ответы на заданное сообщение, если таковые имеются.</span><span class="sxs-lookup"><span data-stu-id="92145-106">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="92145-107">Чтобы получить само сообщение, просто вызовите [сообщение Get Channel](channel-get-message.md).</span><span class="sxs-lookup"><span data-stu-id="92145-107">To get the message itself, simply call [get channel message](channel-get-message.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="92145-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92145-108">Permissions</span></span>
<span data-ttu-id="92145-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92145-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92145-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92145-111">Permission Type</span></span>|<span data-ttu-id="92145-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92145-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="92145-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92145-113">Delegated (work or school account)</span></span>| <span data-ttu-id="92145-114">ChannelMessage.Read.All, Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92145-114">ChannelMessage.Read.All, Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="92145-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92145-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92145-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="92145-116">Not supported</span></span>|
|<span data-ttu-id="92145-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92145-117">Application</span></span>| <span data-ttu-id="92145-118">ChannelMessage.Read.All, Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92145-118">ChannelMessage.Read.All, Group.Read.All,Group.ReadWrite.All</span></span>|

> [!NOTE]
> <span data-ttu-id="92145-119">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="92145-119">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="92145-120">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="92145-120">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="92145-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92145-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92145-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92145-122">Optional query parameters</span></span>

<span data-ttu-id="92145-123">Вы можете использовать параметр запроса [$top](/graph/query-parameters#top-parameter) для управления количеством элементов в одном отклике.</span><span class="sxs-lookup"><span data-stu-id="92145-123">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="92145-124">Другие [параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="92145-124">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92145-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92145-125">Request headers</span></span>
| <span data-ttu-id="92145-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92145-126">Header</span></span>       | <span data-ttu-id="92145-127">Значение</span><span class="sxs-lookup"><span data-stu-id="92145-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92145-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92145-128">Authorization</span></span>  | <span data-ttu-id="92145-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92145-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92145-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="92145-131">Request body</span></span>
<span data-ttu-id="92145-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92145-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92145-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="92145-133">Response</span></span>
<span data-ttu-id="92145-134">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92145-134">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92145-135">Пример</span><span class="sxs-lookup"><span data-stu-id="92145-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92145-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="92145-136">Request</span></span>
<span data-ttu-id="92145-137">В этом примере указанное сообщение имеет два ответа.</span><span class="sxs-lookup"><span data-stu-id="92145-137">In this example, the specified message has two replies.</span></span> <span data-ttu-id="92145-138">Каждый ответ содержит один или несколько объектов [чатмессажементион](../resources/chatmessagemention.md) .</span><span class="sxs-lookup"><span data-stu-id="92145-138">Each reply has one or more [chatMessageMention](../resources/chatmessagemention.md) objects.</span></span>

# <a name="http"></a>[<span data-ttu-id="92145-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="92145-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message_replies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies
```
# <a name="c"></a>[<span data-ttu-id="92145-140">C#</span><span class="sxs-lookup"><span data-stu-id="92145-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92145-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92145-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92145-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92145-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="92145-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="92145-143">Response</span></span>
<span data-ttu-id="92145-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92145-144">Here is an example of the response.</span></span> 

><span data-ttu-id="92145-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92145-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies",
    "@odata.count": 2,
    "value": [
        {
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
        },
        {
            "id": "1555375848360",
            "replyToId": "1555375673184",
            "etag": "1555375848360",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:50:48.36Z",
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
                "content": "<div><div>And, <at id=\"0\">Alex Wilber</at>, can we see the February report as well?</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Alex Wilber",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                            "displayName": "Alex Wilber",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
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
  "description": "List channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
