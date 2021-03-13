---
title: Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph
description: Уведомления об изменениях позволяют прослушивать изменения в сообщениях канала или чата
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: e6e859e76e35e4eefd5ef18a26f0f1339c01a8a2
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761572"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="6aa8e-103">Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6aa8e-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="6aa8e-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) [сообщений](/graph/api/resources/chatMessage?preserve-view=true) в [канале](/graph/api/resources/channel?preserve-view=true) или [чате](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6aa8e-104">Change notifications enable you to subscribe to changes (create, update, and delete) to [messages](/graph/api/resources/chatMessage?preserve-view=true) in a [channel](/graph/api/resources/channel?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true).</span></span> <span data-ttu-id="6aa8e-105">Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять [подпиской](/graph/api/resources/webhooks?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6aa8e-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="6aa8e-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

><span data-ttu-id="6aa8e-107">**Примечание.** Максимальный срок действия подписки составляет 60 минут. Однако подписки можно продлевать, пока у вызывающий не получит разрешения на доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="6aa8e-108">Подписка на изменения на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="6aa8e-108">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="6aa8e-109">Чтобы отслеживать все изменения, связанные с сообщениями в клиенте, вы можете использовать подписки на уровне клиента для сообщений канала и чата.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-109">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="6aa8e-110">Для этого требуется создать две подписки: одну для отслеживания всех сообщений в [каналах](/graph/api/resources/channel?preserve-view=true), а другую — для отслеживания всех сообщений в [чатах](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6aa8e-110">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="6aa8e-111">Подписка на сообщения в каналах</span><span class="sxs-lookup"><span data-stu-id="6aa8e-111">Subscribe to messages across channels</span></span>

<span data-ttu-id="6aa8e-112">Чтобы получать уведомления об изменениях всех сообщений и ответов в каналах в клиенте, подпишитесь на `/teams/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-112">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="6aa8e-113">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-113">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="6aa8e-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa8e-114">Permissions</span></span>

|<span data-ttu-id="6aa8e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa8e-115">Permission type</span></span>      | <span data-ttu-id="6aa8e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-116">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="6aa8e-117">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="6aa8e-117">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="6aa8e-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="6aa8e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-119">Not supported.</span></span> | <span data-ttu-id="6aa8e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-120">Not supported.</span></span> |
|<span data-ttu-id="6aa8e-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aa8e-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-122">Not supported.</span></span>    | <span data-ttu-id="6aa8e-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-123">Not supported.</span></span> |
|<span data-ttu-id="6aa8e-124">Приложение</span><span class="sxs-lookup"><span data-stu-id="6aa8e-124">Application</span></span> | <span data-ttu-id="6aa8e-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aa8e-125">ChannelMessage.Read.All</span></span> | <span data-ttu-id="6aa8e-126">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="6aa8e-126">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="6aa8e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6aa8e-127">Example</span></span>

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

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="6aa8e-128">Подписка на сообщения в чатах</span><span class="sxs-lookup"><span data-stu-id="6aa8e-128">Subscribe to messages across chats</span></span>

<span data-ttu-id="6aa8e-129">Чтобы получать уведомления об изменениях всех сообщений в чатах в клиенте, подпишитесь на `/chats/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-129">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="6aa8e-130">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-130">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="6aa8e-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa8e-131">Permissions</span></span>

|<span data-ttu-id="6aa8e-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa8e-132">Permission type</span></span>      | <span data-ttu-id="6aa8e-133">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-133">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="6aa8e-134">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="6aa8e-134">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="6aa8e-135">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-135">Delegated (work or school account)</span></span> | <span data-ttu-id="6aa8e-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-136">Not supported.</span></span> | <span data-ttu-id="6aa8e-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-137">Not supported.</span></span> |
|<span data-ttu-id="6aa8e-138">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aa8e-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-139">Not supported.</span></span>    | <span data-ttu-id="6aa8e-140">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-140">Not supported.</span></span> |
|<span data-ttu-id="6aa8e-141">Приложение</span><span class="sxs-lookup"><span data-stu-id="6aa8e-141">Application</span></span> | <span data-ttu-id="6aa8e-142">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aa8e-142">Chat.Read.All</span></span> | <span data-ttu-id="6aa8e-143">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="6aa8e-143">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="6aa8e-144">Пример</span><span class="sxs-lookup"><span data-stu-id="6aa8e-144">Example</span></span>

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

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="6aa8e-145">Подписка на сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="6aa8e-145">Subscribe to messages in a channel</span></span>

<span data-ttu-id="6aa8e-146">Чтобы отслеживать сообщения и ответы в канале, вы можете создать подписку на уведомления об изменениях на уровне канала.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-146">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="6aa8e-147">Для этого подпишитесь на `/teams{id}/channels/{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-147">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="6aa8e-148">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-148">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="6aa8e-149">Подписки на уровне канала также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-149">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="6aa8e-150">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa8e-150">Permissions</span></span>

|<span data-ttu-id="6aa8e-151">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa8e-151">Permission type</span></span>      | <span data-ttu-id="6aa8e-152">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-152">Permissions (from least to most privileged)</span></span>              |<span data-ttu-id="6aa8e-153">Поддерживается в версии</span><span class="sxs-lookup"><span data-stu-id="6aa8e-153">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:--------------------|
|<span data-ttu-id="6aa8e-154">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-154">Delegated (work or school account)</span></span> | <span data-ttu-id="6aa8e-155">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aa8e-155">ChannelMessage.Read.All</span></span> | <span data-ttu-id="6aa8e-156">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="6aa8e-156">beta, v1.0</span></span> |
|<span data-ttu-id="6aa8e-157">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-157">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aa8e-158">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-158">Not supported.</span></span>    | <span data-ttu-id="6aa8e-159">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-159">Not supported.</span></span> |
|<span data-ttu-id="6aa8e-160">Приложение</span><span class="sxs-lookup"><span data-stu-id="6aa8e-160">Application</span></span> | <span data-ttu-id="6aa8e-161">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="6aa8e-161">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span></span> | <span data-ttu-id="6aa8e-162">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="6aa8e-162">beta, v1.0</span></span> |

><span data-ttu-id="6aa8e-163">**Примечание.** ChannelMessage.Read.Group поддерживается как часть [контента, связанного с конкретными ресурсами](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="6aa8e-163">**Note:** ChannelMessage.Read.Group is supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="6aa8e-164">Пример 1. Подписка на все сообщения (и ответы) в канале</span><span class="sxs-lookup"><span data-stu-id="6aa8e-164">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

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

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="6aa8e-165">Пример 2. Подписка на сообщения (и ответы) в канале, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="6aa8e-165">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="6aa8e-166">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-166">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="6aa8e-167">Пример 3. Подписка на сообщения (и ответы) в канале без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="6aa8e-167">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

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

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a><span data-ttu-id="6aa8e-168">Пример 4. Подписка на сообщения (и ответы) в канале с упоминанием определенного пользователя</span><span class="sxs-lookup"><span data-stu-id="6aa8e-168">Example 4: Subscribe to messages (and replies) in a channel that mention a specific user</span></span>

<span data-ttu-id="6aa8e-169">Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-169">To get notifications only for messages where a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="6aa8e-170">Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="6aa8e-170">Subscribe to messages in a chat</span></span>

<span data-ttu-id="6aa8e-171">Чтобы отслеживать сообщения в чате, вы можете создать подписку на уведомления об изменениях на уровне чата.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-171">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="6aa8e-172">Для этого подпишитесь на `/chats{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-172">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="6aa8e-173">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-173">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="6aa8e-174">Подписки на уровне чата также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-174">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

> <span data-ttu-id="6aa8e-175">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="6aa8e-175">**Note.**</span></span> <span data-ttu-id="6aa8e-176">Подписка на сообщения в чате находится в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-176">Subcribing to messages in a chat is currently in preview.</span></span>

### <a name="permissions"></a><span data-ttu-id="6aa8e-177">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa8e-177">Permissions</span></span>

|<span data-ttu-id="6aa8e-178">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa8e-178">Permission type</span></span>      | <span data-ttu-id="6aa8e-179">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-179">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="6aa8e-180">Поддерживается в версии</span><span class="sxs-lookup"><span data-stu-id="6aa8e-180">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:---------------------|
|<span data-ttu-id="6aa8e-181">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-181">Delegated (work or school account)</span></span> | <span data-ttu-id="6aa8e-182">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="6aa8e-182">Chat.Read</span></span> | <span data-ttu-id="6aa8e-183">Бета-версия</span><span class="sxs-lookup"><span data-stu-id="6aa8e-183">beta</span></span> |
|<span data-ttu-id="6aa8e-184">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa8e-184">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aa8e-185">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-185">Not supported.</span></span>    | <span data-ttu-id="6aa8e-186">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-186">Not supported.</span></span> |
|<span data-ttu-id="6aa8e-187">Приложение</span><span class="sxs-lookup"><span data-stu-id="6aa8e-187">Application</span></span> | <span data-ttu-id="6aa8e-188">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aa8e-188">Chat.Read.All</span></span> | <span data-ttu-id="6aa8e-189">Бета-версия</span><span class="sxs-lookup"><span data-stu-id="6aa8e-189">beta</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="6aa8e-190">Пример 1. Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="6aa8e-190">Example 1: Subscribe to messages in a chat</span></span>

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

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="6aa8e-191">Пример 2. Подписка на сообщения в чате, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="6aa8e-191">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="6aa8e-192">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-192">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="6aa8e-193">Пример 3. Подписка на сообщения (и ответы) в чате без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="6aa8e-193">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

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

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a><span data-ttu-id="6aa8e-194">Пример 4. Подписка на сообщения в чате, в которых упоминается определенный пользователь</span><span class="sxs-lookup"><span data-stu-id="6aa8e-194">Example 4: Subscribe to message in a chat in which a specific user is mentioned</span></span>

<span data-ttu-id="6aa8e-195">Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-195">To get notifications only for messages in which a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="notification-payloads"></a><span data-ttu-id="6aa8e-196">Полезные данные уведомлений</span><span class="sxs-lookup"><span data-stu-id="6aa8e-196">Notification payloads</span></span>

<span data-ttu-id="6aa8e-197">В зависимости от вашей подписки вы можете получать уведомление с данными ресурсов или без них.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-197">Depending on your subscription, you can either get the notification with resource data, or without it.</span></span> <span data-ttu-id="6aa8e-198">Подписка с данными ресурсов позволяет получать полезные данные вместе с уведомлением, устраняя необходимость обратного вызова и получения содержимого.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-198">Subscribing with resource data allows you to get the message payload along with the notification, removing the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="6aa8e-199">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="6aa8e-199">Notifications with resource data</span></span>

<span data-ttu-id="6aa8e-200">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-200">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="6aa8e-201">Это полезные данные для сообщения, отправленного в чате.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-201">This payload is for a message sent in a chat.</span></span>

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

<span data-ttu-id="6aa8e-202">Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="6aa8e-202">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="6aa8e-203">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-203">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="6aa8e-204">Полезные данные соответствуют схеме [chatMessage](/graph/api/resources/chatMessage?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6aa8e-204">The payload conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="6aa8e-205">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-205">The payload is similar to that returned by GET operations.</span></span>

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

### <a name="notifications-without-resource-data"></a><span data-ttu-id="6aa8e-206">Уведомления без данных о ресурсах</span><span class="sxs-lookup"><span data-stu-id="6aa8e-206">Notifications without resource data</span></span>

<span data-ttu-id="6aa8e-207">Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-207">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="6aa8e-208">Для подписок на уведомления без данных о ресурсах не требуется сертификат шифрования (так как фактические данные ресурсов не передаются).</span><span class="sxs-lookup"><span data-stu-id="6aa8e-208">Subscriptions for notifications without resource data do not require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="6aa8e-209">Полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-209">The payload looks like the following.</span></span> <span data-ttu-id="6aa8e-210">Это полезные данные для сообщения, отправленного в канале.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-210">This payload is for a message sent in a channel.</span></span>

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

<span data-ttu-id="6aa8e-211">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-211">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="6aa8e-212">Вызовы GET всегда возвращают текущее состояние сообщения.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-212">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="6aa8e-213">Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.</span><span class="sxs-lookup"><span data-stu-id="6aa8e-213">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="6aa8e-214">См. также</span><span class="sxs-lookup"><span data-stu-id="6aa8e-214">See also</span></span>
- [<span data-ttu-id="6aa8e-215">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6aa8e-215">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="6aa8e-216">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6aa8e-216">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
