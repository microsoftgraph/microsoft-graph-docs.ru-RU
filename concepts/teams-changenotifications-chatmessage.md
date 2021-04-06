---
title: Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph
description: Уведомления об изменениях позволяют прослушивать изменения в сообщениях канала или чата
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 2e5490549e4ff204957c46e5da39a5516ed7d866
ms.sourcegitcommit: 8b1a6d7b0516f936ce4626246408f067527f5082
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2021
ms.locfileid: "51594863"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="d5f30-103">Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d5f30-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="d5f30-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) [сообщений](/graph/api/resources/chatMessage?preserve-view=true) в [канале](/graph/api/resources/channel?preserve-view=true) или [чате](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="d5f30-104">Change notifications enable you to subscribe to changes (create, update, and delete) to [messages](/graph/api/resources/chatMessage?preserve-view=true) in a [channel](/graph/api/resources/channel?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true).</span></span> <span data-ttu-id="d5f30-105">Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять [подпиской](/graph/api/resources/webhooks?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="d5f30-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="d5f30-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="d5f30-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

><span data-ttu-id="d5f30-107">**Примечание.** Максимальный срок действия подписки составляет 60 минут. Однако подписки можно продлевать, пока у вызывающий не получит разрешения на доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="d5f30-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="d5f30-108">Подписка на изменения на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="d5f30-108">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="d5f30-109">Чтобы отслеживать все изменения, связанные с сообщениями в клиенте, вы можете использовать подписки на уровне клиента для сообщений канала и чата.</span><span class="sxs-lookup"><span data-stu-id="d5f30-109">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="d5f30-110">Для этого требуется создать две подписки: одну для отслеживания всех сообщений в [каналах](/graph/api/resources/channel?preserve-view=true), а другую — для отслеживания всех сообщений в [чатах](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="d5f30-110">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="d5f30-111">Подписка на сообщения в каналах</span><span class="sxs-lookup"><span data-stu-id="d5f30-111">Subscribe to messages across channels</span></span>

<span data-ttu-id="d5f30-112">Чтобы получать уведомления об изменениях всех сообщений и ответов в каналах в клиенте, подпишитесь на `/teams/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="d5f30-112">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="d5f30-113">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="d5f30-113">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="d5f30-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f30-114">Permissions</span></span>

|<span data-ttu-id="d5f30-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f30-115">Permission type</span></span>      | <span data-ttu-id="d5f30-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5f30-116">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="d5f30-117">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="d5f30-117">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="d5f30-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5f30-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d5f30-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-119">Not supported.</span></span> | <span data-ttu-id="d5f30-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-120">Not supported.</span></span> |
|<span data-ttu-id="d5f30-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5f30-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5f30-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-122">Not supported.</span></span>    | <span data-ttu-id="d5f30-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-123">Not supported.</span></span> |
|<span data-ttu-id="d5f30-124">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5f30-124">Application</span></span> | <span data-ttu-id="d5f30-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5f30-125">ChannelMessage.Read.All</span></span> | <span data-ttu-id="d5f30-126">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="d5f30-126">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="d5f30-127">Пример</span><span class="sxs-lookup"><span data-stu-id="d5f30-127">Example</span></span>

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

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="d5f30-128">Подписка на сообщения в чатах</span><span class="sxs-lookup"><span data-stu-id="d5f30-128">Subscribe to messages across chats</span></span>

<span data-ttu-id="d5f30-129">Чтобы получать уведомления об изменениях всех сообщений в чатах в клиенте, подпишитесь на `/chats/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="d5f30-129">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="d5f30-130">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="d5f30-130">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="d5f30-131">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f30-131">Permissions</span></span>

|<span data-ttu-id="d5f30-132">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f30-132">Permission type</span></span>      | <span data-ttu-id="d5f30-133">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5f30-133">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="d5f30-134">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="d5f30-134">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="d5f30-135">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5f30-135">Delegated (work or school account)</span></span> | <span data-ttu-id="d5f30-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-136">Not supported.</span></span> | <span data-ttu-id="d5f30-137">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-137">Not supported.</span></span> |
|<span data-ttu-id="d5f30-138">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5f30-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5f30-139">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-139">Not supported.</span></span>    | <span data-ttu-id="d5f30-140">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-140">Not supported.</span></span> |
|<span data-ttu-id="d5f30-141">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5f30-141">Application</span></span> | <span data-ttu-id="d5f30-142">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5f30-142">Chat.Read.All</span></span> | <span data-ttu-id="d5f30-143">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="d5f30-143">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="d5f30-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d5f30-144">Example</span></span>

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

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="d5f30-145">Подписка на сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="d5f30-145">Subscribe to messages in a channel</span></span>

<span data-ttu-id="d5f30-146">Чтобы отслеживать сообщения и ответы в канале, вы можете создать подписку на уведомления об изменениях на уровне канала.</span><span class="sxs-lookup"><span data-stu-id="d5f30-146">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="d5f30-147">Для этого подпишитесь на `/teams{id}/channels/{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="d5f30-147">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="d5f30-148">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="d5f30-148">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="d5f30-149">Подписки на уровне канала также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="d5f30-149">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="d5f30-150">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f30-150">Permissions</span></span>

|<span data-ttu-id="d5f30-151">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f30-151">Permission type</span></span>      | <span data-ttu-id="d5f30-152">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5f30-152">Permissions (from least to most privileged)</span></span>              |<span data-ttu-id="d5f30-153">Поддерживается в версии</span><span class="sxs-lookup"><span data-stu-id="d5f30-153">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:--------------------|
|<span data-ttu-id="d5f30-154">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5f30-154">Delegated (work or school account)</span></span> | <span data-ttu-id="d5f30-155">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5f30-155">ChannelMessage.Read.All</span></span> | <span data-ttu-id="d5f30-156">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="d5f30-156">beta, v1.0</span></span> |
|<span data-ttu-id="d5f30-157">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5f30-157">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5f30-158">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-158">Not supported.</span></span>    | <span data-ttu-id="d5f30-159">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-159">Not supported.</span></span> |
|<span data-ttu-id="d5f30-160">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5f30-160">Application</span></span> | <span data-ttu-id="d5f30-161">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="d5f30-161">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span></span> | <span data-ttu-id="d5f30-162">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="d5f30-162">beta, v1.0</span></span> |

><span data-ttu-id="d5f30-163">**Примечание.** ChannelMessage.Read.Group поддерживается как часть [контента, связанного с конкретными ресурсами](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="d5f30-163">**Note:** ChannelMessage.Read.Group is supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="d5f30-164">Пример 1. Подписка на все сообщения (и ответы) в канале</span><span class="sxs-lookup"><span data-stu-id="d5f30-164">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

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

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="d5f30-165">Пример 2. Подписка на сообщения (и ответы) в канале, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="d5f30-165">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="d5f30-166">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="d5f30-166">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="d5f30-167">Пример 3. Подписка на сообщения (и ответы) в канале без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="d5f30-167">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

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

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a><span data-ttu-id="d5f30-168">Пример 4. Подписка на сообщения (и ответы) в канале с упоминанием определенного пользователя</span><span class="sxs-lookup"><span data-stu-id="d5f30-168">Example 4: Subscribe to messages (and replies) in a channel that mention a specific user</span></span>

<span data-ttu-id="d5f30-169">Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.</span><span class="sxs-lookup"><span data-stu-id="d5f30-169">To get notifications only for messages where a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="d5f30-170">Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="d5f30-170">Subscribe to messages in a chat</span></span>

<span data-ttu-id="d5f30-171">Чтобы отслеживать сообщения в чате, вы можете создать подписку на уведомления об изменениях на уровне чата.</span><span class="sxs-lookup"><span data-stu-id="d5f30-171">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="d5f30-172">Для этого подпишитесь на `/chats{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="d5f30-172">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="d5f30-173">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.</span><span class="sxs-lookup"><span data-stu-id="d5f30-173">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="d5f30-174">Подписки на уровне чата также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="d5f30-174">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

> <span data-ttu-id="d5f30-175">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="d5f30-175">**Note.**</span></span> <span data-ttu-id="d5f30-176">Подписка на сообщения в чате находится в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="d5f30-176">Subcribing to messages in a chat is currently in preview.</span></span>

### <a name="permissions"></a><span data-ttu-id="d5f30-177">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f30-177">Permissions</span></span>

|<span data-ttu-id="d5f30-178">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5f30-178">Permission type</span></span>      | <span data-ttu-id="d5f30-179">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5f30-179">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="d5f30-180">Поддерживается в версии</span><span class="sxs-lookup"><span data-stu-id="d5f30-180">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:---------------------|
|<span data-ttu-id="d5f30-181">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5f30-181">Delegated (work or school account)</span></span> | <span data-ttu-id="d5f30-182">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="d5f30-182">Chat.Read</span></span> | <span data-ttu-id="d5f30-183">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="d5f30-183">beta, v1.0</span></span> |
|<span data-ttu-id="d5f30-184">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5f30-184">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5f30-185">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-185">Not supported.</span></span>    | <span data-ttu-id="d5f30-186">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5f30-186">Not supported.</span></span> |
|<span data-ttu-id="d5f30-187">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5f30-187">Application</span></span> | <span data-ttu-id="d5f30-188">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5f30-188">Chat.Read.All</span></span> | <span data-ttu-id="d5f30-189">Бета-версия, версия 1.0</span><span class="sxs-lookup"><span data-stu-id="d5f30-189">beta, v1.0</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="d5f30-190">Пример 1. Подписка на сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="d5f30-190">Example 1: Subscribe to messages in a chat</span></span>

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

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="d5f30-191">Пример 2. Подписка на сообщения в чате, содержащие определенный текст</span><span class="sxs-lookup"><span data-stu-id="d5f30-191">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="d5f30-192">Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.</span><span class="sxs-lookup"><span data-stu-id="d5f30-192">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="d5f30-193">Пример 3. Подписка на сообщения (и ответы) в чате без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="d5f30-193">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

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

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a><span data-ttu-id="d5f30-194">Пример 4. Подписка на сообщения в чате, в которых упоминается определенный пользователь</span><span class="sxs-lookup"><span data-stu-id="d5f30-194">Example 4: Subscribe to message in a chat in which a specific user is mentioned</span></span>

<span data-ttu-id="d5f30-195">Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.</span><span class="sxs-lookup"><span data-stu-id="d5f30-195">To get notifications only for messages in which a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="notification-payloads"></a><span data-ttu-id="d5f30-196">Полезные данные уведомлений</span><span class="sxs-lookup"><span data-stu-id="d5f30-196">Notification payloads</span></span>

<span data-ttu-id="d5f30-197">В зависимости от вашей подписки вы можете получать уведомление с данными ресурсов или без них.</span><span class="sxs-lookup"><span data-stu-id="d5f30-197">Depending on your subscription, you can either get the notification with resource data, or without it.</span></span> <span data-ttu-id="d5f30-198">Подписка с данными ресурсов позволяет получать полезные данные вместе с уведомлением, устраняя необходимость обратного вызова и получения содержимого.</span><span class="sxs-lookup"><span data-stu-id="d5f30-198">Subscribing with resource data allows you to get the message payload along with the notification, removing the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="d5f30-199">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="d5f30-199">Notifications with resource data</span></span>

<span data-ttu-id="d5f30-200">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="d5f30-200">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="d5f30-201">Это полезные данные для сообщения, отправленного в чате.</span><span class="sxs-lookup"><span data-stu-id="d5f30-201">This payload is for a message sent in a chat.</span></span>

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

<span data-ttu-id="d5f30-202">Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="d5f30-202">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="d5f30-203">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="d5f30-203">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="d5f30-204">Полезные данные соответствуют схеме [chatMessage](/graph/api/resources/chatMessage?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="d5f30-204">The payload conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="d5f30-205">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="d5f30-205">The payload is similar to that returned by GET operations.</span></span>

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

### <a name="notifications-without-resource-data"></a><span data-ttu-id="d5f30-206">Уведомления без данных о ресурсах</span><span class="sxs-lookup"><span data-stu-id="d5f30-206">Notifications without resource data</span></span>

<span data-ttu-id="d5f30-207">Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения.</span><span class="sxs-lookup"><span data-stu-id="d5f30-207">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="d5f30-208">Для подписок на уведомления без данных о ресурсах не требуется сертификат шифрования (так как фактические данные ресурсов не передаются).</span><span class="sxs-lookup"><span data-stu-id="d5f30-208">Subscriptions for notifications without resource data do not require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="d5f30-209">Полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="d5f30-209">The payload looks like the following.</span></span> <span data-ttu-id="d5f30-210">Это полезные данные для сообщения, отправленного в канале.</span><span class="sxs-lookup"><span data-stu-id="d5f30-210">This payload is for a message sent in a channel.</span></span>

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

<span data-ttu-id="d5f30-211">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения.</span><span class="sxs-lookup"><span data-stu-id="d5f30-211">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="d5f30-212">Вызовы GET всегда возвращают текущее состояние сообщения.</span><span class="sxs-lookup"><span data-stu-id="d5f30-212">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="d5f30-213">Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.</span><span class="sxs-lookup"><span data-stu-id="d5f30-213">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="d5f30-214">См. также</span><span class="sxs-lookup"><span data-stu-id="d5f30-214">See also</span></span>
- [<span data-ttu-id="d5f30-215">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d5f30-215">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="d5f30-216">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d5f30-216">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
