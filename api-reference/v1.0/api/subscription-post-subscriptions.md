---
title: Создание подписки
description: Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменении данных в Microsoft Graph.
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: apiPageType
ms.openlocfilehash: 239de6da37b9e795c5b0c2eec359f0b4b457f5f4
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912056"
---
# <a name="create-subscription"></a><span data-ttu-id="d106e-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="d106e-103">Create subscription</span></span>

<span data-ttu-id="d106e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d106e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d106e-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d106e-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="d106e-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="d106e-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="d106e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d106e-107">Permissions</span></span>

<span data-ttu-id="d106e-108">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d106e-108">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="d106e-109">Например, чтобы получать уведомления об изменениях в сообщениях, приложению необходимо разрешение `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="d106e-109">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
<span data-ttu-id="d106e-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d106e-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d106e-111">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d106e-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d106e-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="d106e-112">Supported resource</span></span> | <span data-ttu-id="d106e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d106e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d106e-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d106e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d106e-115">Application</span><span class="sxs-lookup"><span data-stu-id="d106e-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="d106e-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="d106e-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="d106e-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-117">Not supported</span></span> | <span data-ttu-id="d106e-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-118">Not supported</span></span> | <span data-ttu-id="d106e-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="d106e-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d106e-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="d106e-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-121">ChannelMessage.Read.All</span></span> | <span data-ttu-id="d106e-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-122">Not supported</span></span> |  <span data-ttu-id="d106e-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d106e-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="d106e-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="d106e-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-125">Not supported</span></span> | <span data-ttu-id="d106e-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-126">Not supported</span></span> | <span data-ttu-id="d106e-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d106e-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d106e-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="d106e-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-129">Not supported</span></span> | <span data-ttu-id="d106e-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-130">Not supported</span></span> | <span data-ttu-id="d106e-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="d106e-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="d106e-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="d106e-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-133">Not supported</span></span> | <span data-ttu-id="d106e-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-134">Not supported</span></span> | <span data-ttu-id="d106e-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="d106e-136">contact</span><span class="sxs-lookup"><span data-stu-id="d106e-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d106e-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-137">Contacts.Read</span></span> | <span data-ttu-id="d106e-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-138">Contacts.Read</span></span> | <span data-ttu-id="d106e-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-139">Contacts.Read</span></span> |
|<span data-ttu-id="d106e-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="d106e-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="d106e-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-141">Not supported</span></span> | <span data-ttu-id="d106e-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d106e-142">Files.ReadWrite</span></span> | <span data-ttu-id="d106e-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-143">Not supported</span></span> |
|<span data-ttu-id="d106e-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="d106e-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="d106e-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106e-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="d106e-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-146">Not supported</span></span> | <span data-ttu-id="d106e-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106e-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="d106e-148">event</span><span class="sxs-lookup"><span data-stu-id="d106e-148">event</span></span>](../resources/event.md) | <span data-ttu-id="d106e-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-149">Calendars.Read</span></span> | <span data-ttu-id="d106e-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-150">Calendars.Read</span></span> | <span data-ttu-id="d106e-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-151">Calendars.Read</span></span> |
|[<span data-ttu-id="d106e-152">group</span><span class="sxs-lookup"><span data-stu-id="d106e-152">group</span></span>](../resources/group.md) | <span data-ttu-id="d106e-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-153">Group.Read.All</span></span> | <span data-ttu-id="d106e-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-154">Not supported</span></span> | <span data-ttu-id="d106e-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-155">Group.Read.All</span></span> |
|[<span data-ttu-id="d106e-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="d106e-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="d106e-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-157">Group.Read.All</span></span> | <span data-ttu-id="d106e-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-158">Not supported</span></span> | <span data-ttu-id="d106e-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-159">Not supported</span></span> |
|[<span data-ttu-id="d106e-160">list</span><span class="sxs-lookup"><span data-stu-id="d106e-160">list</span></span>](../resources/list.md) | <span data-ttu-id="d106e-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106e-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="d106e-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-162">Not supported</span></span> | <span data-ttu-id="d106e-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106e-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="d106e-164">message</span><span class="sxs-lookup"><span data-stu-id="d106e-164">message</span></span>](../resources/message.md) | <span data-ttu-id="d106e-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d106e-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d106e-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d106e-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="d106e-168">printer</span><span class="sxs-lookup"><span data-stu-id="d106e-168">printer</span></span>](../resources/printer.md) | <span data-ttu-id="d106e-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-169">Not supported</span></span> | <span data-ttu-id="d106e-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-170">Not supported</span></span> | <span data-ttu-id="d106e-171">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106e-171">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="d106e-172">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="d106e-172">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="d106e-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-173">Not supported</span></span> | <span data-ttu-id="d106e-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-174">Not supported</span></span> | <span data-ttu-id="d106e-175">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106e-175">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="d106e-176">security alert</span><span class="sxs-lookup"><span data-stu-id="d106e-176">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="d106e-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106e-177">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="d106e-178">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d106e-178">Not supported</span></span> | <span data-ttu-id="d106e-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106e-179">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="d106e-180">user</span><span class="sxs-lookup"><span data-stu-id="d106e-180">user</span></span>](../resources/user.md) | <span data-ttu-id="d106e-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-181">User.Read.All</span></span> | <span data-ttu-id="d106e-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-182">User.Read.All</span></span> | <span data-ttu-id="d106e-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d106e-183">User.Read.All</span></span> |

> <span data-ttu-id="d106e-184">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d106e-184">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="d106e-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="d106e-185">driveItem</span></span>

<span data-ttu-id="d106e-186">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d106e-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="d106e-187">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="d106e-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="d106e-188">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="d106e-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="d106e-189">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="d106e-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="d106e-190">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="d106e-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="d106e-191">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="d106e-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

<span data-ttu-id="d106e-192">OneDrive для бизнеса и SharePoint поддерживают отправку уведомлений приложений о событиях безопасности, которые происходят в **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="d106e-192">OneDrive for Business and SharePoint support sending your application notifications of security events that occur on a **driveItem**.</span></span> <span data-ttu-id="d106e-193">Чтобы подписаться на эти события, добавьте заголовок `prefer:includesecuritywebhooks` в запрос на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="d106e-193">To subscribe to these events, add the `prefer:includesecuritywebhooks` header to your request to create a subscription.</span></span> <span data-ttu-id="d106e-194">После создания подписки вы будете получать уведомления об изменениях разрешений для элемента.</span><span class="sxs-lookup"><span data-stu-id="d106e-194">After the subscription is created, you will receive notifications when the permissions on an item change.</span></span> <span data-ttu-id="d106e-195">Этот заголовок можно использовать в SharePoint и OneDrive для бизнеса, но не в учетных записях потребителей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d106e-195">This header is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="d106e-196">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="d106e-196">contact, event, and message</span></span>

<span data-ttu-id="d106e-197">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="d106e-197">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="d106e-198">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="d106e-198">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="d106e-199">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="d106e-199">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="d106e-200">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d106e-200">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="d106e-201">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="d106e-201">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="d106e-202">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d106e-202">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="d106e-203">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="d106e-203">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="d106e-204">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d106e-204">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="d106e-205">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d106e-205">Request headers</span></span>

| <span data-ttu-id="d106e-206">Имя</span><span class="sxs-lookup"><span data-stu-id="d106e-206">Name</span></span>       | <span data-ttu-id="d106e-207">Тип</span><span class="sxs-lookup"><span data-stu-id="d106e-207">Type</span></span> | <span data-ttu-id="d106e-208">Описание</span><span class="sxs-lookup"><span data-stu-id="d106e-208">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d106e-209">Authorization</span><span class="sxs-lookup"><span data-stu-id="d106e-209">Authorization</span></span>  | <span data-ttu-id="d106e-210">string</span><span class="sxs-lookup"><span data-stu-id="d106e-210">string</span></span>  | <span data-ttu-id="d106e-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d106e-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d106e-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="d106e-213">Response</span></span>

<span data-ttu-id="d106e-214">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d106e-214">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="d106e-215">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="d106e-215">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="d106e-216">Пример</span><span class="sxs-lookup"><span data-stu-id="d106e-216">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d106e-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="d106e-217">Request</span></span>

<span data-ttu-id="d106e-218">Ниже представлен пример запроса на отправку уведомления об изменениях при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="d106e-218">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="d106e-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="d106e-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="d106e-220">C#</span><span class="sxs-lookup"><span data-stu-id="d106e-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d106e-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d106e-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d106e-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d106e-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d106e-223">Java</span><span class="sxs-lookup"><span data-stu-id="d106e-223">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="d106e-224">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d106e-224">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="d106e-225">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="d106e-225">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="d106e-226">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="d106e-226">Resources examples</span></span>

<span data-ttu-id="d106e-227">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="d106e-227">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="d106e-228">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="d106e-228">Resource type</span></span> | <span data-ttu-id="d106e-229">Примеры</span><span class="sxs-lookup"><span data-stu-id="d106e-229">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="d106e-230">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="d106e-230">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="d106e-231">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="d106e-231">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="d106e-232">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="d106e-232">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="d106e-233">Контакты</span><span class="sxs-lookup"><span data-stu-id="d106e-233">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="d106e-234">Беседы</span><span class="sxs-lookup"><span data-stu-id="d106e-234">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="d106e-235">Диски</span><span class="sxs-lookup"><span data-stu-id="d106e-235">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="d106e-236">События</span><span class="sxs-lookup"><span data-stu-id="d106e-236">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="d106e-237">Группы</span><span class="sxs-lookup"><span data-stu-id="d106e-237">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="d106e-238">Список</span><span class="sxs-lookup"><span data-stu-id="d106e-238">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="d106e-239">Почта</span><span class="sxs-lookup"><span data-stu-id="d106e-239">Mail</span></span>](../resources/message.md)|<span data-ttu-id="d106e-240">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="d106e-240">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="d106e-241">printer</span><span class="sxs-lookup"><span data-stu-id="d106e-241">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="d106e-242">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="d106e-242">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="d106e-243">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="d106e-243">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|
|[<span data-ttu-id="d106e-244">Пользователи</span><span class="sxs-lookup"><span data-stu-id="d106e-244">Users</span></span>](../resources/user.md)|`users`|

> <span data-ttu-id="d106e-245">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="d106e-245">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="d106e-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="d106e-246">Response</span></span>

<span data-ttu-id="d106e-p111">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d106e-p111">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="d106e-249">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="d106e-249">Notification endpoint validation</span></span>

<span data-ttu-id="d106e-250">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="d106e-250">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="d106e-251">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="d106e-251">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

