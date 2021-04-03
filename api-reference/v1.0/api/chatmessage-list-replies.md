---
title: Списки сообщений канала
description: Список всех ответов сообщения в канале группы.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aaa40106f3b1364bc1b5ad13ac0a8ecfbc894513
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582955"
---
# <a name="list-replies"></a><span data-ttu-id="3de4d-103">Ответы списка</span><span class="sxs-lookup"><span data-stu-id="3de4d-103">List replies</span></span>

<span data-ttu-id="3de4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3de4d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3de4d-105">Список всех ответов на [сообщение](../resources/chatmessage.md) в [канале](../resources/channel.md) группы.</span><span class="sxs-lookup"><span data-stu-id="3de4d-105">List all the replies to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="3de4d-106">В этом методе перечислены только ответы указанного сообщения, если таково.</span><span class="sxs-lookup"><span data-stu-id="3de4d-106">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="3de4d-107">Чтобы получить само сообщение, просто позвоните [получить сообщение канала](chatmessage-get.md).</span><span class="sxs-lookup"><span data-stu-id="3de4d-107">To get the message itself, simply call [get channel message](chatmessage-get.md).</span></span>

> <span data-ttu-id="3de4d-108">**Примечание**. Этот API поддерживает подписку на изменения (создание, обновление и удаление) с использованием [уведомлений об изменениях](../resources/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="3de4d-108">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="3de4d-109">Это позволяет вызывающим подписаться на изменения и получать их в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="3de4d-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="3de4d-110">Дополнительные сведения см. в разделе [Получение уведомлений о сообщениях](/graph/teams-changenotifications-chatmessage).</span><span class="sxs-lookup"><span data-stu-id="3de4d-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="3de4d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3de4d-111">Permissions</span></span>
<span data-ttu-id="3de4d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3de4d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de4d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3de4d-114">Permission Type</span></span>|<span data-ttu-id="3de4d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3de4d-115">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3de4d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3de4d-116">Delegated (work or school account)</span></span>| <span data-ttu-id="3de4d-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="3de4d-117">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="3de4d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3de4d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3de4d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de4d-119">Not supported.</span></span>|
|<span data-ttu-id="3de4d-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="3de4d-120">Application</span></span>| <span data-ttu-id="3de4d-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="3de4d-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="3de4d-122">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="3de4d-122">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="3de4d-123">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="3de4d-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="3de4d-124">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="3de4d-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="3de4d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3de4d-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3de4d-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3de4d-126">Optional query parameters</span></span>

<span data-ttu-id="3de4d-127">Вы можете использовать параметр запроса [$top](/graph/query-parameters#top-parameter) для управления количеством элементов в одном отклике.</span><span class="sxs-lookup"><span data-stu-id="3de4d-127">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="3de4d-128">Максимальное значение `$top`: 50.</span><span class="sxs-lookup"><span data-stu-id="3de4d-128">Maximum allowed `$top` value is 50.</span></span>
<span data-ttu-id="3de4d-129">Другие [параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="3de4d-129">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3de4d-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3de4d-130">Request headers</span></span>
| <span data-ttu-id="3de4d-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3de4d-131">Header</span></span>       | <span data-ttu-id="3de4d-132">Значение</span><span class="sxs-lookup"><span data-stu-id="3de4d-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3de4d-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3de4d-133">Authorization</span></span>  | <span data-ttu-id="3de4d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3de4d-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3de4d-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3de4d-136">Request body</span></span>
<span data-ttu-id="3de4d-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3de4d-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3de4d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de4d-138">Response</span></span>
<span data-ttu-id="3de4d-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3de4d-139">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de4d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3de4d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3de4d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3de4d-141">Request</span></span>
<span data-ttu-id="3de4d-142">В этом примере указанное сообщение имеет три ответа.</span><span class="sxs-lookup"><span data-stu-id="3de4d-142">In this example, the specified message has three replies.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_listmessagereplies_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616989510408/replies
```

### <a name="response"></a><span data-ttu-id="3de4d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de4d-143">Response</span></span>
<span data-ttu-id="3de4d-144">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3de4d-144">The following example shows the response.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616989510408')/replies",
    "@odata.count": 3,
    "value": [
        {
            "id": "1616989753153",
            "replyToId": "1616989510408",
            "etag": "1616989753153",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:13.153Z",
            "lastModifiedDateTime": "2021-03-29T03:49:13.153Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989753153?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989753153&parentMessageId=1616989510408",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Reply3"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1616989750004",
            "replyToId": "1616989510408",
            "etag": "1616989750004",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:10.004Z",
            "lastModifiedDateTime": "2021-03-29T03:49:10.004Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989750004?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989750004&parentMessageId=1616989510408",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Reply2"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1616989747416",
            "replyToId": "1616989510408",
            "etag": "1616989747416",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:07.416Z",
            "lastModifiedDateTime": "2021-03-29T03:49:07.416Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989747416?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989747416&parentMessageId=1616989510408",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Reply1"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
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
  "description": "List channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->