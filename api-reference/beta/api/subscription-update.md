---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 4313b3f64bc4e16afc5ac0c1dce4d4fe476b09fd
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51031039"
---
# <a name="update-subscription"></a><span data-ttu-id="966f1-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="966f1-103">Update subscription</span></span>

<span data-ttu-id="966f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="966f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="966f1-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="966f1-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="966f1-106">В таблице в разделе [Разрешения](#permissions) перечислены ресурсы, поддерживаюющие подписку на изменение уведомлений.</span><span class="sxs-lookup"><span data-stu-id="966f1-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="966f1-107">Срок действия подписки истекает по истечении времени, которое зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="966f1-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="966f1-108">Чтобы избежать пропуска уведомлений об изменениях, приложение должно продлить подписки заблаговременно до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="966f1-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="966f1-109">См. [подписку](../resources/subscription.md) на максимальную длину подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="966f1-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="966f1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="966f1-110">Permissions</span></span>

<span data-ttu-id="966f1-111">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="966f1-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="966f1-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="966f1-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="966f1-113">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="966f1-113">Supported resource</span></span> | <span data-ttu-id="966f1-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="966f1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="966f1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="966f1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="966f1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="966f1-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="966f1-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="966f1-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="966f1-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-118">Not supported</span></span> | <span data-ttu-id="966f1-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-119">Not supported</span></span> | <span data-ttu-id="966f1-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="966f1-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="966f1-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="966f1-122">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-122">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="966f1-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-123">Not supported</span></span> | <span data-ttu-id="966f1-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="966f1-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="966f1-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="966f1-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-126">Not supported</span></span> | <span data-ttu-id="966f1-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-127">Not supported</span></span> | <span data-ttu-id="966f1-128">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-128">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="966f1-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="966f1-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="966f1-130">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="966f1-130">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="966f1-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-131">Not supported</span></span> | <span data-ttu-id="966f1-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-132">Chat.Read.All</span></span>  |
|<span data-ttu-id="966f1-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="966f1-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="966f1-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-134">Not supported</span></span> | <span data-ttu-id="966f1-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-135">Not supported</span></span> | <span data-ttu-id="966f1-136">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-136">Chat.Read.All</span></span>  |
|[<span data-ttu-id="966f1-137">contact</span><span class="sxs-lookup"><span data-stu-id="966f1-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="966f1-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-138">Contacts.Read</span></span> | <span data-ttu-id="966f1-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-139">Contacts.Read</span></span> | <span data-ttu-id="966f1-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-140">Contacts.Read</span></span> |
|<span data-ttu-id="966f1-141">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="966f1-141">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="966f1-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-142">Not supported</span></span> | <span data-ttu-id="966f1-143">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="966f1-143">Files.ReadWrite</span></span> | <span data-ttu-id="966f1-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-144">Not supported</span></span> |
|<span data-ttu-id="966f1-145">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="966f1-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="966f1-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-146">Files.ReadWrite.All</span></span> | <span data-ttu-id="966f1-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-147">Not supported</span></span> | <span data-ttu-id="966f1-148">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-148">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="966f1-149">event</span><span class="sxs-lookup"><span data-stu-id="966f1-149">event</span></span>](../resources/event.md) | <span data-ttu-id="966f1-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-150">Calendars.Read</span></span> | <span data-ttu-id="966f1-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-151">Calendars.Read</span></span> | <span data-ttu-id="966f1-152">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-152">Calendars.Read</span></span> |
|[<span data-ttu-id="966f1-153">group</span><span class="sxs-lookup"><span data-stu-id="966f1-153">group</span></span>](../resources/group.md) | <span data-ttu-id="966f1-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-154">Group.Read.All</span></span> | <span data-ttu-id="966f1-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-155">Not supported</span></span> | <span data-ttu-id="966f1-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-156">Group.Read.All</span></span> |
|[<span data-ttu-id="966f1-157">group conversation</span><span class="sxs-lookup"><span data-stu-id="966f1-157">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="966f1-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-158">Group.Read.All</span></span> | <span data-ttu-id="966f1-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-159">Not supported</span></span> | <span data-ttu-id="966f1-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-160">Not supported</span></span> |
|[<span data-ttu-id="966f1-161">list</span><span class="sxs-lookup"><span data-stu-id="966f1-161">list</span></span>](../resources/list.md) | <span data-ttu-id="966f1-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-162">Sites.ReadWrite.All</span></span> | <span data-ttu-id="966f1-163">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-163">Not supported</span></span> | <span data-ttu-id="966f1-164">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-164">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="966f1-165">message</span><span class="sxs-lookup"><span data-stu-id="966f1-165">message</span></span>](../resources/message.md) | <span data-ttu-id="966f1-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="966f1-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-167">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="966f1-168">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="966f1-168">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="966f1-169">presence</span><span class="sxs-lookup"><span data-stu-id="966f1-169">presence</span></span>](../resources/presence.md) | <span data-ttu-id="966f1-170">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-170">Presence.Read.All</span></span> | <span data-ttu-id="966f1-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-171">Not supported</span></span> | <span data-ttu-id="966f1-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-172">Not supported</span></span> |
|[<span data-ttu-id="966f1-173">printer</span><span class="sxs-lookup"><span data-stu-id="966f1-173">printer</span></span>](../resources/printer.md) | <span data-ttu-id="966f1-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-174">Not supported</span></span> | <span data-ttu-id="966f1-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-175">Not supported</span></span> | <span data-ttu-id="966f1-176">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-176">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="966f1-177">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="966f1-177">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="966f1-178">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-178">Not supported</span></span> | <span data-ttu-id="966f1-179">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-179">Not supported</span></span> | <span data-ttu-id="966f1-180">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-180">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="966f1-181">security alert</span><span class="sxs-lookup"><span data-stu-id="966f1-181">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="966f1-182">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-182">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="966f1-183">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-183">Not supported</span></span> | <span data-ttu-id="966f1-184">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="966f1-184">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="966f1-185">todoTask</span><span class="sxs-lookup"><span data-stu-id="966f1-185">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="966f1-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="966f1-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="966f1-187">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="966f1-187">Tasks.ReadWrite</span></span> | <span data-ttu-id="966f1-188">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="966f1-188">Not supported</span></span> |
|[<span data-ttu-id="966f1-189">user</span><span class="sxs-lookup"><span data-stu-id="966f1-189">user</span></span>](../resources/user.md) | <span data-ttu-id="966f1-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-190">User.Read.All</span></span> | <span data-ttu-id="966f1-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-191">User.Read.All</span></span> | <span data-ttu-id="966f1-192">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="966f1-192">User.Read.All</span></span> |

> <span data-ttu-id="966f1-193">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="966f1-193">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="966f1-194">driveItem</span><span class="sxs-lookup"><span data-stu-id="966f1-194">driveItem</span></span>

<span data-ttu-id="966f1-195">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="966f1-195">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="966f1-196">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="966f1-196">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="966f1-197">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="966f1-197">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="966f1-198">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="966f1-198">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="966f1-199">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="966f1-199">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="966f1-200">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="966f1-200">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="966f1-201">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="966f1-201">contact, event, and message</span></span>

<span data-ttu-id="966f1-202">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="966f1-202">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="966f1-203">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="966f1-203">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="966f1-204">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="966f1-204">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="966f1-205">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="966f1-205">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="966f1-206">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="966f1-206">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="966f1-207">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="966f1-207">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="966f1-208">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="966f1-208">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="966f1-209">presence</span><span class="sxs-lookup"><span data-stu-id="966f1-209">presence</span></span>

<span data-ttu-id="966f1-210">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="966f1-210">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="966f1-211">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="966f1-211">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="966f1-212">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="966f1-212">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="966f1-213">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="966f1-213">Request headers</span></span>

| <span data-ttu-id="966f1-214">Имя</span><span class="sxs-lookup"><span data-stu-id="966f1-214">Name</span></span>       | <span data-ttu-id="966f1-215">Тип</span><span class="sxs-lookup"><span data-stu-id="966f1-215">Type</span></span> | <span data-ttu-id="966f1-216">Описание</span><span class="sxs-lookup"><span data-stu-id="966f1-216">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="966f1-217">Authorization</span><span class="sxs-lookup"><span data-stu-id="966f1-217">Authorization</span></span>  | <span data-ttu-id="966f1-218">string</span><span class="sxs-lookup"><span data-stu-id="966f1-218">string</span></span>  | <span data-ttu-id="966f1-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="966f1-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="966f1-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="966f1-221">Response</span></span>

<span data-ttu-id="966f1-222">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="966f1-222">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="966f1-223">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="966f1-223">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="966f1-224">Пример</span><span class="sxs-lookup"><span data-stu-id="966f1-224">Example</span></span>

##### <a name="request"></a><span data-ttu-id="966f1-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="966f1-225">Request</span></span>

<span data-ttu-id="966f1-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="966f1-226">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="966f1-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="966f1-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="966f1-228">C#</span><span class="sxs-lookup"><span data-stu-id="966f1-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="966f1-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="966f1-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="966f1-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="966f1-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="966f1-231">Java</span><span class="sxs-lookup"><span data-stu-id="966f1-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="966f1-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="966f1-232">Response</span></span>

<span data-ttu-id="966f1-233">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="966f1-233">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false,
  "notificationContentType": "application/json"
}
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


