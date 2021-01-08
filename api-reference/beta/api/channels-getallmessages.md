---
title: 'каналы: getAllMessages'
description: Извлечение всех сообщений, отправленных по каналам в группе.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4ad45990655059db63d90c79225c676e4cf06ec0
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784783"
---
# <a name="channels-getallmessages"></a><span data-ttu-id="88d59-103">каналы: getAllMessages</span><span class="sxs-lookup"><span data-stu-id="88d59-103">channels: getAllMessages</span></span>

<span data-ttu-id="88d59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88d59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88d59-105">Извлечение всех [сообщений](../resources/chatmessage.md), отправленных по всем [каналам](../resources/channel.md) в [команде](../resources/team.md), включая текстовые, аудио и видео сообщения.</span><span class="sxs-lookup"><span data-stu-id="88d59-105">Retrieve all [messages](../resources/chatmessage.md) across all [channels](../resources/channel.md) in a [team](../resources/team.md) including text, audio, and video conversations.</span></span>

## <a name="permissions"></a><span data-ttu-id="88d59-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88d59-106">Permissions</span></span>

<span data-ttu-id="88d59-107">Для вызова этого API требуются разрешения ниже.</span><span class="sxs-lookup"><span data-stu-id="88d59-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="88d59-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88d59-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d59-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88d59-109">Permission type</span></span>      | <span data-ttu-id="88d59-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88d59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88d59-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88d59-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88d59-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="88d59-112">Not supported</span></span> |
|<span data-ttu-id="88d59-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88d59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88d59-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="88d59-114">Not supported</span></span> |
|<span data-ttu-id="88d59-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="88d59-115">Application</span></span> | <span data-ttu-id="88d59-116">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d59-116">ChannelMessage.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="88d59-117">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="88d59-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="88d59-118">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="88d59-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="88d59-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88d59-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88d59-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="88d59-120">Optional query parameters</span></span>

<span data-ttu-id="88d59-121">Это действие в настоящее время не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="88d59-121">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="88d59-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88d59-122">Request body</span></span>

<span data-ttu-id="88d59-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88d59-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88d59-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="88d59-124">Response</span></span>

<span data-ttu-id="88d59-125">В случае успешного выполнения этот метод возвращает код отклика `200 OK`, а также все сообщения в канале.</span><span class="sxs-lookup"><span data-stu-id="88d59-125">If successful, this method returns a `200 OK` response code and also returns all the messages in the channel.</span></span>

## <a name="example"></a><span data-ttu-id="88d59-126">Пример</span><span class="sxs-lookup"><span data-stu-id="88d59-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="88d59-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="88d59-127">Request</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/0e05a7e4-a48d-4615-b0b7-c7494da9ce68/channels/getAllMessages
```

### <a name="response"></a><span data-ttu-id="88d59-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="88d59-128">Response</span></span>

><span data-ttu-id="88d59-129">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="88d59-129">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metdata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/a5212c6a-a8b1-49cd-bd40-7f83f0a42861/channels/getAllMessages?$top=2&$skip=2",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/teams/ab5332ba-6dd9-46d3-ade5-5c61a2f148b2/channels/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/messages/1580173996201",
            "id": "1580173996201",
            "replyToId": null,
            "etag": "1580173996201",
            "messageType": "message",
            "createdDateTime": "2020-01-28T01:13:16.201Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/1580173996201?groupId=ab5332ba-6dd9-46d3-ade5-5c61a2f148b2&tenantId=e0d829d2-c239-4b28-9d08-c096da71be7a&createdTime=1580173996201&parentMessageId=1580173996201",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "a5212c6a-a8b1-49cd-bd40-7f83f0a42861",
                    "displayName": "spoons test",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Test"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.id": "https://graph.microsoft.com/beta/teams/ab5332ba-6dd9-46d3-ade5-5c61a2f148b2/channels/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/messages/1580768557513",
            "id": "1580768557513",
            "replyToId": null,
            "etag": "1580768557513",
            "messageType": "message",
            "createdDateTime": "2020-02-03T22:22:37.513Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "a5212c6a-a8b1-49cd-bd40-7f83f0a42861",
                    "displayName": "spoons test",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "hi user1,user3"
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
  "description": "channels: getallmessages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
