---
title: Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph
description: Уведомления об изменениях позволяют прослушивать изменения в сообщениях канала или чата
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 1d9767a913b5fe5878cb1cc8e72ec9900fcec4ac
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000719"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="c6b3d-103">Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c6b3d-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="c6b3d-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) [сообщений](/graph/api/resources/chatMessage?preserve-view=true) в [канале](/graph/api/resources/channel?preserve-view=true) или [чате](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="c6b3d-104">Change notifications enable you to subscribe to changes (create, update, and delete) to [messages](/graph/api/resources/chatMessage?preserve-view=true) in a [channel](/graph/api/resources/channel?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true).</span></span> <span data-ttu-id="c6b3d-105">Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять [подпиской](/graph/api/resources/webhooks?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="c6b3d-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="c6b3d-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

><span data-ttu-id="c6b3d-107">**Примечание.** Максимальный срок действия подписки составляет 60 минут. Однако подписки можно продлевать, пока у вызывающий не получит разрешения на доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="c6b3d-108">Подписка на изменения на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="c6b3d-108">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="c6b3d-109">Чтобы отслеживать все изменения, связанные с сообщениями в клиенте, вы можете использовать подписки на уровне клиента для сообщений канала и чата.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-109">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="c6b3d-110">Для этого требуется создать две подписки: одну для отслеживания всех сообщений в [каналах](/graph/api/resources/channel?preserve-view=true), а другую — для отслеживания всех сообщений в [чатах](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="c6b3d-110">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="c6b3d-111">Подписка на сообщения в каналах</span><span class="sxs-lookup"><span data-stu-id="c6b3d-111">Subscribe to messages across channels</span></span>

<span data-ttu-id="c6b3d-112">Чтобы получать уведомления об изменениях всех сообщений и ответов в каналах в клиенте, подпишитесь на `/teams/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-112">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="c6b3d-113">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-113">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="c6b3d-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-114">Permissions</span></span>

|<span data-ttu-id="c6b3d-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-115">Permission type</span></span>      | <span data-ttu-id="c6b3d-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6b3d-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c6b3d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-118">Not supported.</span></span> |
|<span data-ttu-id="c6b3d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6b3d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-120">Not supported.</span></span>    |
|<span data-ttu-id="c6b3d-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-121">Application</span></span> | <span data-ttu-id="c6b3d-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6b3d-122">ChannelMessage.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="c6b3d-123">Пример</span><span class="sxs-lookup"><span data-stu-id="c6b3d-123">Example</span></span>

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

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="c6b3d-124">Подписка на сообщения в чатах</span><span class="sxs-lookup"><span data-stu-id="c6b3d-124">Subscribe to messages across chats</span></span>

<span data-ttu-id="c6b3d-125">Чтобы получать уведомления об изменениях всех сообщений в чатах в клиенте, подпишитесь на `/chats/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-125">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="c6b3d-126">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="c6b3d-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-127">Permissions</span></span>

|<span data-ttu-id="c6b3d-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-128">Permission type</span></span>      | <span data-ttu-id="c6b3d-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6b3d-130">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-130">Delegated (work or school account)</span></span> | <span data-ttu-id="c6b3d-131">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-131">Not supported.</span></span> |
|<span data-ttu-id="c6b3d-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6b3d-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-133">Not supported.</span></span>    |
|<span data-ttu-id="c6b3d-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="c6b3d-134">Application</span></span> | <span data-ttu-id="c6b3d-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6b3d-135">Chat.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="c6b3d-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c6b3d-136">Example</span></span>

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

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="c6b3d-137">Подписка на сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="c6b3d-137">Subscribe to messages in a channel</span></span>

<span data-ttu-id="c6b3d-138">Чтобы отслеживать сообщения и ответы в канале, вы можете создать подписку на уведомления об изменениях на уровне канала.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-138">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="c6b3d-139">Для этого подпишитесь на `/teams{id}/channels/{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-139">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="c6b3d-140">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-140">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="c6b3d-141">Подписки на уровне канала также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-141">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="c6b3d-142">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-142">Permissions</span></span>

|<span data-ttu-id="c6b3d-143">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-143">Permission type</span></span>      | <span data-ttu-id="c6b3d-144">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-144">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6b3d-145">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-145">Delegated (work or school account)</span></span> | <span data-ttu-id="c6b3d-146">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6b3d-146">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="c6b3d-147">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6b3d-148">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-148">Not supported.</span></span>    |
|<span data-ttu-id="c6b3d-149">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-149">Application</span></span> | <span data-ttu-id="c6b3d-150">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6b3d-150">ChannelMessage.Read.All</span></span> |

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="c6b3d-151">Пример 1. Подписка на все сообщения (и ответы) в канале</span><span class="sxs-lookup"><span data-stu-id="c6b3d-151">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

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

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="c6b3d-152">Пример 2. Подписка на сообщения (и ответы) в канале, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="c6b3d-152">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="c6b3d-153">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-153">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="c6b3d-154">Пример 3. Подписка на сообщения (и ответы) в канале без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="c6b3d-154">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

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

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="c6b3d-155">Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="c6b3d-155">Subscribe to messages in a chat</span></span>

<span data-ttu-id="c6b3d-156">Чтобы отслеживать сообщения в чате, вы можете создать подписку на уведомления об изменениях на уровне чата.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-156">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="c6b3d-157">Для этого подпишитесь на `/chats{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-157">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="c6b3d-158">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-158">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="c6b3d-159">Подписки на уровне чата также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-159">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="c6b3d-160">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-160">Permissions</span></span>

|<span data-ttu-id="c6b3d-161">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b3d-161">Permission type</span></span>      | <span data-ttu-id="c6b3d-162">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-162">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6b3d-163">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-163">Delegated (work or school account)</span></span> | <span data-ttu-id="c6b3d-164">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="c6b3d-164">Chat.Read</span></span> |
|<span data-ttu-id="c6b3d-165">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6b3d-165">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6b3d-166">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-166">Not supported.</span></span>    |
|<span data-ttu-id="c6b3d-167">Приложение</span><span class="sxs-lookup"><span data-stu-id="c6b3d-167">Application</span></span> | <span data-ttu-id="c6b3d-168">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6b3d-168">Chat.Read.All</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="c6b3d-169">Пример 1. Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="c6b3d-169">Example 1: Subscribe to messages in a chat</span></span>

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

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="c6b3d-170">Пример 2. Подписка на сообщения в чате, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="c6b3d-170">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="c6b3d-171">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="c6b3d-171">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="c6b3d-172">Пример 3. Подписка на сообщения (и ответы) в чате без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="c6b3d-172">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c6b3d-173">См. также</span><span class="sxs-lookup"><span data-stu-id="c6b3d-173">See also</span></span>
- [<span data-ttu-id="c6b3d-174">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c6b3d-174">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="c6b3d-175">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c6b3d-175">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
