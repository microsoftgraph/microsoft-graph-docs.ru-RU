---
title: Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph
description: Уведомления об изменениях позволяют прослушивать изменения в сообщениях канала или чата
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 78718b1b486231ae2549323433312aa878806210
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941426"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="30d2a-103">Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="30d2a-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="30d2a-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) сообщений в канале или чате.</span><span class="sxs-lookup"><span data-stu-id="30d2a-104">Change notifications enable you to subscribe to changes (create, update, and delete) to messages in a channel or chat.</span></span> <span data-ttu-id="30d2a-105">Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять подпиской.</span><span class="sxs-lookup"><span data-stu-id="30d2a-105">Change notifications provide a low latency model by allowing you to maintain a subscription.</span></span> <span data-ttu-id="30d2a-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="30d2a-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="30d2a-107">Подписка на изменения на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="30d2a-107">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="30d2a-108">Чтобы отслеживать все изменения, связанные с сообщениями в клиенте, вы можете использовать подписки на уровне клиента для сообщений канала и чата.</span><span class="sxs-lookup"><span data-stu-id="30d2a-108">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="30d2a-109">Для этого требуется создать две подписки: одну для отслеживания всех сообщений в [каналах](/graph/api/resources/channel?preserve-view=true), а другую — для отслеживания всех сообщений в [чатах](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="30d2a-109">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="30d2a-110">Подписка на сообщения в каналах</span><span class="sxs-lookup"><span data-stu-id="30d2a-110">Subscribe to messages across channels</span></span>

<span data-ttu-id="30d2a-111">Чтобы получать уведомления об изменениях всех сообщений и ответов в каналах в клиенте, подпишитесь на `/teams/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="30d2a-111">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="30d2a-112">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="30d2a-112">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="30d2a-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30d2a-113">Permissions</span></span>

|<span data-ttu-id="30d2a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30d2a-114">Permission type</span></span>      | <span data-ttu-id="30d2a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30d2a-115">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="30d2a-116">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="30d2a-116">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="30d2a-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30d2a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="30d2a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-118">Not supported.</span></span> | <span data-ttu-id="30d2a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-119">Not supported.</span></span> |
|<span data-ttu-id="30d2a-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30d2a-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30d2a-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-121">Not supported.</span></span>    | <span data-ttu-id="30d2a-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-122">Not supported.</span></span> |
|<span data-ttu-id="30d2a-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="30d2a-123">Application</span></span> | <span data-ttu-id="30d2a-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="30d2a-124">ChannelMessage.Read.All</span></span> | <span data-ttu-id="30d2a-125">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="30d2a-125">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="30d2a-126">Пример</span><span class="sxs-lookup"><span data-stu-id="30d2a-126">Example</span></span>

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

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="30d2a-127">Подписка на сообщения в чатах</span><span class="sxs-lookup"><span data-stu-id="30d2a-127">Subscribe to messages across chats</span></span>

<span data-ttu-id="30d2a-128">Чтобы получать уведомления об изменениях всех сообщений в чатах в клиенте, подпишитесь на `/chats/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="30d2a-128">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="30d2a-129">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="30d2a-129">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="30d2a-130">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30d2a-130">Permissions</span></span>

|<span data-ttu-id="30d2a-131">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30d2a-131">Permission type</span></span>      | <span data-ttu-id="30d2a-132">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30d2a-132">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="30d2a-133">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="30d2a-133">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="30d2a-134">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30d2a-134">Delegated (work or school account)</span></span> | <span data-ttu-id="30d2a-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-135">Not supported.</span></span> | <span data-ttu-id="30d2a-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-136">Not supported.</span></span> |
|<span data-ttu-id="30d2a-137">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30d2a-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30d2a-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-138">Not supported.</span></span>    | <span data-ttu-id="30d2a-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-139">Not supported.</span></span> |
|<span data-ttu-id="30d2a-140">Приложение</span><span class="sxs-lookup"><span data-stu-id="30d2a-140">Application</span></span> | <span data-ttu-id="30d2a-141">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="30d2a-141">Chat.Read.All</span></span> | <span data-ttu-id="30d2a-142">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="30d2a-142">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="30d2a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="30d2a-143">Example</span></span>

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

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="30d2a-144">Подписка на сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="30d2a-144">Subscribe to messages in a channel</span></span>

<span data-ttu-id="30d2a-145">Чтобы отслеживать сообщения и ответы в канале, вы можете создать подписку на уведомления об изменениях на уровне канала.</span><span class="sxs-lookup"><span data-stu-id="30d2a-145">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="30d2a-146">Для этого подпишитесь на `/teams{id}/channels/{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="30d2a-146">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="30d2a-147">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="30d2a-147">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="30d2a-148">Подписки на уровне канала также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="30d2a-148">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="30d2a-149">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30d2a-149">Permissions</span></span>

|<span data-ttu-id="30d2a-150">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30d2a-150">Permission type</span></span>      | <span data-ttu-id="30d2a-151">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30d2a-151">Permissions (from least to most privileged)</span></span>              |<span data-ttu-id="30d2a-152">Поддерживается в версии</span><span class="sxs-lookup"><span data-stu-id="30d2a-152">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:--------------------|
|<span data-ttu-id="30d2a-153">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30d2a-153">Delegated (work or school account)</span></span> | <span data-ttu-id="30d2a-154">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="30d2a-154">ChannelMessage.Read.All</span></span> | <span data-ttu-id="30d2a-155">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="30d2a-155">beta, v1.0</span></span> |
|<span data-ttu-id="30d2a-156">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30d2a-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30d2a-157">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-157">Not supported.</span></span>    | <span data-ttu-id="30d2a-158">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-158">Not supported.</span></span> |
|<span data-ttu-id="30d2a-159">Приложение</span><span class="sxs-lookup"><span data-stu-id="30d2a-159">Application</span></span> | <span data-ttu-id="30d2a-160">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="30d2a-160">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span></span> | <span data-ttu-id="30d2a-161">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="30d2a-161">beta, v1.0</span></span> |

><span data-ttu-id="30d2a-162">**Примечание.** ChannelMessage.Read.Group поддерживается как часть [контента, связанного с конкретными ресурсами](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="30d2a-162">**Note:** ChannelMessage.Read.Group is supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="30d2a-163">Пример 1. Подписка на все сообщения (и ответы) в канале</span><span class="sxs-lookup"><span data-stu-id="30d2a-163">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

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

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="30d2a-164">Пример 2. Подписка на сообщения (и ответы) в канале, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="30d2a-164">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="30d2a-165">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="30d2a-165">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="30d2a-166">Пример 3. Подписка на сообщения (и ответы) в канале без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="30d2a-166">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

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

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a><span data-ttu-id="30d2a-167">Пример 4. Подписка на сообщения (и ответы) в канале с упоминанием определенного пользователя</span><span class="sxs-lookup"><span data-stu-id="30d2a-167">Example 4: Subscribe to messages (and replies) in a channel that mention a specific user</span></span>

<span data-ttu-id="30d2a-168">Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.</span><span class="sxs-lookup"><span data-stu-id="30d2a-168">To get notifications only for messages where a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="30d2a-169">Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="30d2a-169">Subscribe to messages in a chat</span></span>

<span data-ttu-id="30d2a-170">Чтобы отслеживать сообщения в чате, вы можете создать подписку на уведомления об изменениях на уровне чата.</span><span class="sxs-lookup"><span data-stu-id="30d2a-170">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="30d2a-171">Для этого подпишитесь на `/chats{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="30d2a-171">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="30d2a-172">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="30d2a-172">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="30d2a-173">Подписки на уровне чата также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="30d2a-173">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

> <span data-ttu-id="30d2a-174">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="30d2a-174">**Note.**</span></span> <span data-ttu-id="30d2a-175">Подписка на сообщения в чате находится в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="30d2a-175">Subcribing to messages in a chat is currently in preview.</span></span>

### <a name="permissions"></a><span data-ttu-id="30d2a-176">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30d2a-176">Permissions</span></span>

|<span data-ttu-id="30d2a-177">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30d2a-177">Permission type</span></span>      | <span data-ttu-id="30d2a-178">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30d2a-178">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="30d2a-179">Поддерживается в версии</span><span class="sxs-lookup"><span data-stu-id="30d2a-179">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:---------------------|
|<span data-ttu-id="30d2a-180">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30d2a-180">Delegated (work or school account)</span></span> | <span data-ttu-id="30d2a-181">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="30d2a-181">Chat.Read</span></span> | <span data-ttu-id="30d2a-182">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="30d2a-182">beta, v1.0</span></span> |
|<span data-ttu-id="30d2a-183">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30d2a-183">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30d2a-184">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-184">Not supported.</span></span>    | <span data-ttu-id="30d2a-185">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d2a-185">Not supported.</span></span> |
|<span data-ttu-id="30d2a-186">Приложение</span><span class="sxs-lookup"><span data-stu-id="30d2a-186">Application</span></span> | <span data-ttu-id="30d2a-187">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="30d2a-187">Chat.Read.All</span></span> | <span data-ttu-id="30d2a-188">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="30d2a-188">beta, v1.0</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="30d2a-189">Пример 1. Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="30d2a-189">Example 1: Subscribe to messages in a chat</span></span>

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

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="30d2a-190">Пример 2. Подписка на сообщения в чате, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="30d2a-190">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="30d2a-191">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="30d2a-191">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="30d2a-192">Пример 3. Подписка на сообщения (и ответы) в чате без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="30d2a-192">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

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

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a><span data-ttu-id="30d2a-193">Пример 4. Подписка на сообщения в чате, в которых упоминается определенный пользователь</span><span class="sxs-lookup"><span data-stu-id="30d2a-193">Example 4: Subscribe to message in a chat in which a specific user is mentioned</span></span>

<span data-ttu-id="30d2a-194">Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.</span><span class="sxs-lookup"><span data-stu-id="30d2a-194">To get notifications only for messages in which a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="notification-payloads"></a><span data-ttu-id="30d2a-195">Полезные данные уведомлений</span><span class="sxs-lookup"><span data-stu-id="30d2a-195">Notification payloads</span></span>

<span data-ttu-id="30d2a-196">В зависимости от вашей подписки вы можете получать уведомление с данными ресурсов или без них.</span><span class="sxs-lookup"><span data-stu-id="30d2a-196">Depending on your subscription, you can either get the notification with resource data, or without it.</span></span> <span data-ttu-id="30d2a-197">Подписка с данными ресурсов позволяет получать полезные данные вместе с уведомлением, устраняя необходимость обратного вызова и получения содержимого.</span><span class="sxs-lookup"><span data-stu-id="30d2a-197">Subscribing with resource data allows you to get the message payload along with the notification, removing the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="30d2a-198">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="30d2a-198">Notifications with resource data</span></span>

<span data-ttu-id="30d2a-199">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="30d2a-199">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="30d2a-200">Это полезные данные для сообщения, отправленного в чате.</span><span class="sxs-lookup"><span data-stu-id="30d2a-200">This payload is for a message sent in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="30d2a-201">Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="30d2a-201">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="30d2a-202">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="30d2a-202">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="30d2a-203">Полезные данные соответствуют схеме [chatMessage](/graph/api/resources/chatMessage?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="30d2a-203">The payload conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="30d2a-204">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="30d2a-204">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="30d2a-205">Уведомления без данных о ресурсах</span><span class="sxs-lookup"><span data-stu-id="30d2a-205">Notifications without resource data</span></span>

<span data-ttu-id="30d2a-206">Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения.</span><span class="sxs-lookup"><span data-stu-id="30d2a-206">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="30d2a-207">Для подписок на уведомления без данных о ресурсах не требуется сертификат шифрования (так как фактические данные ресурсов не передаются).</span><span class="sxs-lookup"><span data-stu-id="30d2a-207">Subscriptions for notifications without resource data do not require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="30d2a-208">Полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="30d2a-208">The payload looks like the following.</span></span> <span data-ttu-id="30d2a-209">Это полезные данные для сообщения, отправленного в канале.</span><span class="sxs-lookup"><span data-stu-id="30d2a-209">This payload is for a message sent in a channel.</span></span>

```json
 {
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```

<span data-ttu-id="30d2a-210">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения.</span><span class="sxs-lookup"><span data-stu-id="30d2a-210">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="30d2a-211">Вызовы GET всегда возвращают текущее состояние сообщения.</span><span class="sxs-lookup"><span data-stu-id="30d2a-211">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="30d2a-212">Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.</span><span class="sxs-lookup"><span data-stu-id="30d2a-212">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="30d2a-213">См. также</span><span class="sxs-lookup"><span data-stu-id="30d2a-213">See also</span></span>
- [<span data-ttu-id="30d2a-214">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="30d2a-214">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="30d2a-215">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="30d2a-215">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
