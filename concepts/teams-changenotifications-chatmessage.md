---
title: Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph
description: Уведомления об изменениях позволяют прослушивать изменения в сообщениях канала или чата
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 12d8bfd49ebc71b6cb82cccd9525a3706cd570fd
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690615"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="1b5e2-103">Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1b5e2-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="1b5e2-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) [сообщений](/graph/api/resources/chatMessage?preserve-view=true) в [канале](/graph/api/resources/channel?preserve-view=true) или [чате](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="1b5e2-104">Change notifications enable you to subscribe to changes (create, update, and delete) to [messages](/graph/api/resources/chatMessage?preserve-view=true) in a [channel](/graph/api/resources/channel?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true).</span></span> <span data-ttu-id="1b5e2-105">Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять [подпиской](/graph/api/resources/webhooks?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="1b5e2-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="1b5e2-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

><span data-ttu-id="1b5e2-107">**Примечание.** Максимальный срок действия подписки составляет 60 минут. Однако подписки можно продлевать, пока у вызывающий не получит разрешения на доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="1b5e2-108">Подписка на изменения на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="1b5e2-108">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="1b5e2-109">Чтобы отслеживать все изменения, связанные с сообщениями в клиенте, вы можете использовать подписки на уровне клиента для сообщений канала и чата.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-109">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="1b5e2-110">Для этого требуется создать две подписки: одну для отслеживания всех сообщений в [каналах](/graph/api/resources/channel?preserve-view=true), а другую — для отслеживания всех сообщений в [чатах](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="1b5e2-110">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="1b5e2-111">Подписка на сообщения в каналах</span><span class="sxs-lookup"><span data-stu-id="1b5e2-111">Subscribe to messages across channels</span></span>

<span data-ttu-id="1b5e2-112">Чтобы получать уведомления об изменениях всех сообщений и ответов в каналах в клиенте, подпишитесь на `/teams/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-112">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="1b5e2-113">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-113">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="1b5e2-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5e2-114">Permissions</span></span>

|<span data-ttu-id="1b5e2-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5e2-115">Permission type</span></span>      | <span data-ttu-id="1b5e2-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5e2-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-118">Not supported.</span></span> |
|<span data-ttu-id="1b5e2-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5e2-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-120">Not supported.</span></span>    |
|<span data-ttu-id="1b5e2-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b5e2-121">Application</span></span> | <span data-ttu-id="1b5e2-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b5e2-122">ChannelMessage.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="1b5e2-123">Пример</span><span class="sxs-lookup"><span data-stu-id="1b5e2-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="1b5e2-124">Подписка на сообщения в чатах</span><span class="sxs-lookup"><span data-stu-id="1b5e2-124">Subscribe to messages across chats</span></span>

<span data-ttu-id="1b5e2-125">Чтобы получать уведомления об изменениях всех сообщений в чатах в клиенте, подпишитесь на `/chats/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-125">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="1b5e2-126">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="1b5e2-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5e2-127">Permissions</span></span>

|<span data-ttu-id="1b5e2-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5e2-128">Permission type</span></span>      | <span data-ttu-id="1b5e2-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5e2-130">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-130">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5e2-131">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-131">Not supported.</span></span> |
|<span data-ttu-id="1b5e2-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5e2-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-133">Not supported.</span></span>    |
|<span data-ttu-id="1b5e2-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b5e2-134">Application</span></span> | <span data-ttu-id="1b5e2-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b5e2-135">Chat.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="1b5e2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1b5e2-136">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="1b5e2-137">Подписка на сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="1b5e2-137">Subscribe to messages in a channel</span></span>

<span data-ttu-id="1b5e2-138">Чтобы отслеживать сообщения и ответы в канале, вы можете создать подписку на уведомления об изменениях на уровне канала.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-138">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="1b5e2-139">Для этого подпишитесь на `/teams{id}/channels/{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-139">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="1b5e2-140">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-140">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="1b5e2-141">Подписки на уровне канала также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-141">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="1b5e2-142">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5e2-142">Permissions</span></span>

|<span data-ttu-id="1b5e2-143">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5e2-143">Permission type</span></span>      | <span data-ttu-id="1b5e2-144">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-144">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5e2-145">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-145">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5e2-146">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b5e2-146">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="1b5e2-147">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5e2-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-148">Not supported.</span></span>    |
|<span data-ttu-id="1b5e2-149">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b5e2-149">Application</span></span> | <span data-ttu-id="1b5e2-150">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="1b5e2-150">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span></span> |

><span data-ttu-id="1b5e2-151">**Примечание.** ChannelMessage.Read.Group поддерживается как часть [контента, связанного с конкретными ресурсами](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="1b5e2-151">**Note:** ChannelMessage.Read.Group is supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="1b5e2-152">Пример 1. Подписка на все сообщения (и ответы) в канале</span><span class="sxs-lookup"><span data-stu-id="1b5e2-152">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="1b5e2-153">Пример 2. Подписка на сообщения (и ответы) в канале, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="1b5e2-153">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="1b5e2-154">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-154">The following request will send messages that contain `Hello` to the subscriber.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="1b5e2-155">Пример 3. Подписка на сообщения (и ответы) в канале без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="1b5e2-155">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a><span data-ttu-id="1b5e2-156">Пример 4. Подписка на сообщения (и ответы) в канале с упоминанием определенного пользователя</span><span class="sxs-lookup"><span data-stu-id="1b5e2-156">Example 4: Subscribe to messages (and replies) in a channel that mention a specific user</span></span>

<span data-ttu-id="1b5e2-157">Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-157">To get notifications only for messages where a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="1b5e2-158">Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="1b5e2-158">Subscribe to messages in a chat</span></span>

<span data-ttu-id="1b5e2-159">Чтобы отслеживать сообщения в чате, вы можете создать подписку на уведомления об изменениях на уровне чата.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-159">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="1b5e2-160">Для этого подпишитесь на `/chats{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-160">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="1b5e2-161">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-161">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="1b5e2-162">Подписки на уровне чата также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-162">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

> <span data-ttu-id="1b5e2-163">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="1b5e2-163">**Note.**</span></span> <span data-ttu-id="1b5e2-164">Подписка на сообщения в чате находится в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-164">Subcribing to messages in a chat is currently in preview.</span></span>

### <a name="permissions"></a><span data-ttu-id="1b5e2-165">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5e2-165">Permissions</span></span>

|<span data-ttu-id="1b5e2-166">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5e2-166">Permission type</span></span>      | <span data-ttu-id="1b5e2-167">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-167">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5e2-168">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-168">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5e2-169">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="1b5e2-169">Chat.Read</span></span> |
|<span data-ttu-id="1b5e2-170">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b5e2-170">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5e2-171">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-171">Not supported.</span></span>    |
|<span data-ttu-id="1b5e2-172">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b5e2-172">Application</span></span> | <span data-ttu-id="1b5e2-173">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b5e2-173">Chat.Read.All</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="1b5e2-174">Пример 1. Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="1b5e2-174">Example 1: Subscribe to messages in a chat</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="1b5e2-175">Пример 2. Подписка на сообщения в чате, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="1b5e2-175">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="1b5e2-176">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-176">The following request will send messages that contain `Hello` to the subscriber.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="1b5e2-177">Пример 3. Подписка на сообщения (и ответы) в чате без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="1b5e2-177">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a><span data-ttu-id="1b5e2-178">Пример 4. Подписка на сообщения в чате, в которых упоминается определенный пользователь</span><span class="sxs-lookup"><span data-stu-id="1b5e2-178">Example 4: Subscribe to message in a chat in which a specific user is mentioned</span></span>

<span data-ttu-id="1b5e2-179">Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.</span><span class="sxs-lookup"><span data-stu-id="1b5e2-179">To get notifications only for messages in which a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="see-also"></a><span data-ttu-id="1b5e2-180">См. также</span><span class="sxs-lookup"><span data-stu-id="1b5e2-180">See also</span></span>
- [<span data-ttu-id="1b5e2-181">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1b5e2-181">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="1b5e2-182">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1b5e2-182">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
