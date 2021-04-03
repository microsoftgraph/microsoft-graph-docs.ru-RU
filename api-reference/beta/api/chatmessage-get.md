---
title: Получение объекта chatMessage в канале или чате
description: Получение одного сообщения (без ответов) в канале или чате.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5d8ab3e40de66e2187701f67d1460eef5af14c8c
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51583095"
---
# <a name="get-chatmessage-in-a-channel-or-chat"></a><span data-ttu-id="405ff-103">Получение объекта chatMessage в канале или чате</span><span class="sxs-lookup"><span data-stu-id="405ff-103">Get chatMessage in a channel or chat</span></span>

<span data-ttu-id="405ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="405ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="405ff-105">Получение одного [сообщения](../resources/chatmessage.md) или [ответа на сообщение](../resources/chatmessage.md) в [канале](../resources/channel.md) или [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="405ff-105">Retrieve a single [message](../resources/chatmessage.md) or a [message reply](../resources/chatmessage.md) in a [channel](../resources/channel.md) or a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="405ff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="405ff-106">Permissions</span></span>

<span data-ttu-id="405ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="405ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="405ff-109">Разрешения для канала</span><span class="sxs-lookup"><span data-stu-id="405ff-109">Permissions for channel</span></span>

| <span data-ttu-id="405ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="405ff-110">Permission type</span></span>                        | <span data-ttu-id="405ff-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="405ff-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="405ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="405ff-112">Delegated (work or school account)</span></span>| <span data-ttu-id="405ff-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="405ff-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="405ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="405ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="405ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="405ff-115">Not supported.</span></span>|
|<span data-ttu-id="405ff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="405ff-116">Application</span></span>| <span data-ttu-id="405ff-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="405ff-117">ChannelMessage.Read.Group, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="405ff-118">Разрешения для чата</span><span class="sxs-lookup"><span data-stu-id="405ff-118">Permissions for chat</span></span>

| <span data-ttu-id="405ff-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="405ff-119">Permission type</span></span>                        | <span data-ttu-id="405ff-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="405ff-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="405ff-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="405ff-121">Delegated (work or school account)</span></span>| <span data-ttu-id="405ff-122">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="405ff-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="405ff-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="405ff-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="405ff-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="405ff-124">Not supported.</span></span>|
|<span data-ttu-id="405ff-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="405ff-125">Application</span></span>| <span data-ttu-id="405ff-126">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="405ff-126">Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="405ff-127">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="405ff-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="405ff-128">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="405ff-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="405ff-129">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="405ff-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="405ff-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="405ff-130">HTTP request</span></span>

<span data-ttu-id="405ff-131">**Получение сообщения в канале**</span><span class="sxs-lookup"><span data-stu-id="405ff-131">**Get message in a channel**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}
```

<span data-ttu-id="405ff-132">**Получение сообщения в чате**</span><span class="sxs-lookup"><span data-stu-id="405ff-132">**Get message in a chat**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}
GET /users/{user-id}/chats/{chat-id}/messages/{message-id}
GET /me/chats/{chat-id}/messages/{message-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="405ff-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="405ff-133">Optional query parameters</span></span>
<span data-ttu-id="405ff-134">Этот метод не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="405ff-134">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="405ff-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="405ff-135">Request headers</span></span>
| <span data-ttu-id="405ff-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="405ff-136">Header</span></span>       | <span data-ttu-id="405ff-137">Значение</span><span class="sxs-lookup"><span data-stu-id="405ff-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="405ff-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="405ff-138">Authorization</span></span>  | <span data-ttu-id="405ff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="405ff-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="405ff-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="405ff-141">Request body</span></span>
<span data-ttu-id="405ff-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="405ff-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="405ff-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="405ff-143">Response</span></span>

<span data-ttu-id="405ff-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="405ff-144">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="405ff-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="405ff-145">Examples</span></span>

### <a name="example-1-get-a-message-in-a-chat"></a><span data-ttu-id="405ff-146">Пример 1. Получение сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="405ff-146">Example 1: Get a message in a chat</span></span>
#### <a name="request"></a><span data-ttu-id="405ff-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="405ff-147">Request</span></span>
<span data-ttu-id="405ff-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="405ff-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_1"
}-->
```http
GET https://graph.microsoft.com/beta/chats/19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces/messages/1612289992105
```

#### <a name="response"></a><span data-ttu-id="405ff-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="405ff-149">Response</span></span>
<span data-ttu-id="405ff-150">Ниже показан пример отклика. `chatId`</span><span class="sxs-lookup"><span data-stu-id="405ff-150">The following example shows the response.`chatId`</span></span> <span data-ttu-id="405ff-151">определяет [чат](../resources/chat.md), содержащий это сообщение.</span><span class="sxs-lookup"><span data-stu-id="405ff-151">identifies the [chat](../resources/chat.md) that contains this message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5%40unq.gbl.spaces')/messages/$entity",
    "id": "1612289992105",
    "replyToId": null,
    "etag": "1612289992105",
    "messageType": "message",
    "createdDateTime": "2021-02-02T18:19:52.105Z",
    "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
    "importance": "normal",
    "locale": "en-us",
    "webUrl": null,
    "channelIdentity": null,
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
        "content": "test"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-get-a-message-in-a-channel"></a><span data-ttu-id="405ff-152">Пример 2. Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="405ff-152">Example 2: Get a message in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="405ff-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="405ff-153">Request</span></span>
<span data-ttu-id="405ff-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="405ff-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_2"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349
```

#### <a name="response"></a><span data-ttu-id="405ff-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="405ff-155">Response</span></span>
<span data-ttu-id="405ff-156">Ниже показан пример отклика. `channelIdentity`</span><span class="sxs-lookup"><span data-stu-id="405ff-156">The following example shows the response.`channelIdentity`</span></span> <span data-ttu-id="405ff-157">определяет [команду](../resources/team.md) и [канал](../resources/channel.md), содержащий это сообщение.</span><span class="sxs-lookup"><span data-stu-id="405ff-157">identifies the [team](../resources/team.md) and [channel](../resources/channel.md) that contains this message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1614618259349",
    "replyToId": null,
    "etag": "1614618259349",
    "messageType": "message",
    "createdDateTime": "2021-03-01T17:04:19.349Z",
    "lastModifiedDateTime": "2021-03-01T17:04:19.349Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1614618259349?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1614618259349&parentMessageId=1614618259349",
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
        "contentType": "html",
        "content": "<div><div><div><span><img height=\"250\" src=\"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents/aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv/$value\" width=\"424.6575342465753\" style=\"vertical-align:bottom; width:424px; height:250px\"></span></div></div></div>"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-3-get-reply-to-a-message-in-a-channel"></a><span data-ttu-id="405ff-158">Пример 3. Получение ответа на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="405ff-158">Example 3: Get reply to a message in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="405ff-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="405ff-159">Request</span></span>
<span data-ttu-id="405ff-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="405ff-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_3"
}-->
```http
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1612509044972/replies/1613671348387
```

#### <a name="response"></a><span data-ttu-id="405ff-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="405ff-161">Response</span></span>
<span data-ttu-id="405ff-162">Ниже показан пример отклика. `replyToId`</span><span class="sxs-lookup"><span data-stu-id="405ff-162">The following example shows the response.`replyToId`</span></span> <span data-ttu-id="405ff-163">содержит `id` корневого сообщения.</span><span class="sxs-lookup"><span data-stu-id="405ff-163">contains the `id` of the root message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1612509044972')/replies/$entity",
    "id": "1613671348387",
    "replyToId": "1612509044972",
    "etag": "1613671348387",
    "messageType": "message",
    "createdDateTime": "2021-02-18T18:02:28.387Z",
    "lastModifiedDateTime": "2021-02-18T18:02:28.387Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1613671348387?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1613671348387&parentMessageId=1612509044972",
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
        "contentType": "html",
        "content": "<div><div>Test</div></div>"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a><span data-ttu-id="405ff-164">См. также</span><span class="sxs-lookup"><span data-stu-id="405ff-164">See also</span></span>

- [<span data-ttu-id="405ff-165">Список сообщений в канале</span><span class="sxs-lookup"><span data-stu-id="405ff-165">List messages in a channel</span></span>](channel-list-messages.md)
- [<span data-ttu-id="405ff-166">Список сообщений в чате</span><span class="sxs-lookup"><span data-stu-id="405ff-166">List messages in a chat</span></span>](chat-list-messages.md)
- [<span data-ttu-id="405ff-167">Отправка сообщения в канале или чате</span><span class="sxs-lookup"><span data-stu-id="405ff-167">Send message in a channel or a chat</span></span>](chatmessage-post.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a single message (without its replies) in a channel or a chat.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->