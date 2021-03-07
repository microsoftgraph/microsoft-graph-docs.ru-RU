---
title: Перечисление сообщений в каналах
description: 'Получение списка сообщений (без ответов) в канале команды. Чтобы получить ответы на сообщение, вызовите API перечисления ответов на сообщение или получения ответа на сообщение. '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c12646d969c170e019f2892acde3afc9fa88d544
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515926"
---
# <a name="list-channel-messages"></a><span data-ttu-id="2b8f0-104">Перечисление сообщений в каналах</span><span class="sxs-lookup"><span data-stu-id="2b8f0-104">List channel messages</span></span>

<span data-ttu-id="2b8f0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b8f0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b8f0-106">Получение списка [сообщений](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="2b8f0-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> 

<span data-ttu-id="2b8f0-107">Чтобы получить ответы на сообщение, вызовите API [перечисления ответов на сообщение](channel-list-messagereplies.md) или [получения ответа на сообщение](channel-get-messagereply.md).</span><span class="sxs-lookup"><span data-stu-id="2b8f0-107">To get the replies for a message, call the [list message replies](channel-list-messagereplies.md) or the [get message reply](channel-get-messagereply.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2b8f0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b8f0-108">Permissions</span></span>

<span data-ttu-id="2b8f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b8f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b8f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b8f0-111">Permission Type</span></span>|<span data-ttu-id="2b8f0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b8f0-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="2b8f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b8f0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2b8f0-114">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b8f0-114">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="2b8f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b8f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b8f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-116">Not supported.</span></span>|
|<span data-ttu-id="2b8f0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b8f0-117">Application</span></span>| <span data-ttu-id="2b8f0-118">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b8f0-118">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="2b8f0-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="2b8f0-119">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="2b8f0-120">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="2b8f0-121">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="2b8f0-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="2b8f0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b8f0-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b8f0-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b8f0-123">Optional query parameters</span></span>

<span data-ttu-id="2b8f0-124">Вы можете использовать параметр запроса [$top](/graph/query-parameters#top-parameter) для управления количеством элементов в одном отклике.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-124">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="2b8f0-125">Другие [параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-125">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

> <span data-ttu-id="2b8f0-126">**Примечание.** Метод [GET /teams/{id}/channels/{id}/messages/delta](chatmessage-delta.md) поддерживает фильтрацию по дате, предоставляя схожие данные с методом GET /teams/{id}/channels/{id}/messages.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-126">**Note:** [GET /teams/{id}/channels/{id}/messages/delta](chatmessage-delta.md) supports filtering by date, which provides similar data to GET /teams/{id}/channels/{id}/messages.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b8f0-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b8f0-127">Request headers</span></span>

| <span data-ttu-id="2b8f0-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b8f0-128">Header</span></span>       | <span data-ttu-id="2b8f0-129">Значение</span><span class="sxs-lookup"><span data-stu-id="2b8f0-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b8f0-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b8f0-130">Authorization</span></span>  | <span data-ttu-id="2b8f0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b8f0-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b8f0-133">Request body</span></span>

<span data-ttu-id="2b8f0-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b8f0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b8f0-135">Response</span></span>

<span data-ttu-id="2b8f0-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-136">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b8f0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="2b8f0-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b8f0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b8f0-138">Request</span></span>

<span data-ttu-id="2b8f0-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b8f0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b8f0-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"],
  "name": "get_channel_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages
```
# <a name="c"></a>[<span data-ttu-id="2b8f0-141">C#</span><span class="sxs-lookup"><span data-stu-id="2b8f0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b8f0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b8f0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b8f0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b8f0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b8f0-144">Java</span><span class="sxs-lookup"><span data-stu-id="2b8f0-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2b8f0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b8f0-145">Response</span></span>
<span data-ttu-id="2b8f0-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-146">Here is an example of the response.</span></span> 

><span data-ttu-id="2b8f0-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b8f0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages",
    "@odata.count": 3,
    "value": [
        {
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
            "attachments": [],
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
            "reactions": []
        },
        {
            "id": "1548100551644",
            "replyToId": null,
            "etag": "1548100551893",
            "messageType": "message",
            "createdDateTime": "2019-01-21T19:55:51.644Z",
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
                    "id": "c651e5be-7631-42ad-99c6-12c59def11fb",
                    "displayName": "Miriam Graham",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div>I've added an Excel tab to the channel containing the P&amp;L Summary. \r\n<div style=\"display:inline\"><at id=\"0\">Isaiah Langer</at></div> and team, please review the Sale Summary tab in particular, and make any necessary updates.</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Isaiah Langer",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "b525e831-bd00-45e5-860c-a4329ef5f5d8",
                            "displayName": "Isaiah Langer",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": [
                {
                    "reactionType": "like",
                    "createdDateTime": "2019-01-21T19:55:51.893Z",
                    "user": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "e1ecb745-c10f-40af-a9d4-cab946c80ac7",
                            "displayName": null,
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ]
        },
        {
            "id": "1548100547534",
            "replyToId": null,
            "etag": "1548100547534",
            "messageType": "message",
            "createdDateTime": "2019-01-21T19:55:47.534Z",
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "high",
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
                "content": "<div>Just a reminder to everyone to please update your monthly reports by this Friday!</div>"
            },
            "attachments": [],
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
  "description": "List channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


