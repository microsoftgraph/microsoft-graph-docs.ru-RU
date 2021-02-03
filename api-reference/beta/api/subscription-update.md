---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 30bbf91e1e9b1af1d99fee1de638ab6618ac4479
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092696"
---
# <a name="update-subscription"></a><span data-ttu-id="5223f-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="5223f-103">Update subscription</span></span>

<span data-ttu-id="5223f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5223f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5223f-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="5223f-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="5223f-106">В таблице в разделе ["Разрешения"](#permissions) перечислены ресурсы, которые поддерживают подписку на уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="5223f-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="5223f-107">Срок действия подписок истекает через некоторое время, которое зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="5223f-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="5223f-108">Чтобы избежать отсутствующих уведомлений об изменениях, приложение должно продлевать подписки ранее до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="5223f-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="5223f-109">Максимальная [длина](../resources/subscription.md) подписки для каждого типа ресурса см. в подписке.</span><span class="sxs-lookup"><span data-stu-id="5223f-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="5223f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5223f-110">Permissions</span></span>

<span data-ttu-id="5223f-111">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5223f-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="5223f-112">Чтобы узнать больше, в том [числе](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) с осторожностью перед выбором более привилегированных разрешений, найди следующие разрешения в [разрешениях.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="5223f-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5223f-113">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="5223f-113">Supported resource</span></span> | <span data-ttu-id="5223f-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5223f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5223f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5223f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5223f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5223f-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="5223f-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="5223f-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="5223f-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-118">Not supported</span></span> | <span data-ttu-id="5223f-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-119">Not supported</span></span> | <span data-ttu-id="5223f-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="5223f-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5223f-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="5223f-122">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-122">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="5223f-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-123">Not supported</span></span> | <span data-ttu-id="5223f-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5223f-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="5223f-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="5223f-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-126">Not supported</span></span> | <span data-ttu-id="5223f-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-127">Not supported</span></span> | <span data-ttu-id="5223f-128">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-128">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5223f-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5223f-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="5223f-130">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5223f-130">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="5223f-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-131">Not supported</span></span> | <span data-ttu-id="5223f-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-132">Chat.Read.All</span></span>  |
|<span data-ttu-id="5223f-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="5223f-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="5223f-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-134">Not supported</span></span> | <span data-ttu-id="5223f-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-135">Not supported</span></span> | <span data-ttu-id="5223f-136">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-136">Chat.Read.All</span></span>  |
|[<span data-ttu-id="5223f-137">contact</span><span class="sxs-lookup"><span data-stu-id="5223f-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5223f-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-138">Contacts.Read</span></span> | <span data-ttu-id="5223f-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-139">Contacts.Read</span></span> | <span data-ttu-id="5223f-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-140">Contacts.Read</span></span> |
|<span data-ttu-id="5223f-141">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="5223f-141">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="5223f-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-142">Not supported</span></span> | <span data-ttu-id="5223f-143">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5223f-143">Files.ReadWrite</span></span> | <span data-ttu-id="5223f-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-144">Not supported</span></span> |
|<span data-ttu-id="5223f-145">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="5223f-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="5223f-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-146">Files.ReadWrite.All</span></span> | <span data-ttu-id="5223f-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-147">Not supported</span></span> | <span data-ttu-id="5223f-148">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-148">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="5223f-149">event</span><span class="sxs-lookup"><span data-stu-id="5223f-149">event</span></span>](../resources/event.md) | <span data-ttu-id="5223f-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-150">Calendars.Read</span></span> | <span data-ttu-id="5223f-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-151">Calendars.Read</span></span> | <span data-ttu-id="5223f-152">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-152">Calendars.Read</span></span> |
|[<span data-ttu-id="5223f-153">group</span><span class="sxs-lookup"><span data-stu-id="5223f-153">group</span></span>](../resources/group.md) | <span data-ttu-id="5223f-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-154">Group.Read.All</span></span> | <span data-ttu-id="5223f-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-155">Not supported</span></span> | <span data-ttu-id="5223f-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-156">Group.Read.All</span></span> |
|[<span data-ttu-id="5223f-157">group conversation</span><span class="sxs-lookup"><span data-stu-id="5223f-157">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="5223f-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-158">Group.Read.All</span></span> | <span data-ttu-id="5223f-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-159">Not supported</span></span> | <span data-ttu-id="5223f-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-160">Not supported</span></span> |
|[<span data-ttu-id="5223f-161">list</span><span class="sxs-lookup"><span data-stu-id="5223f-161">list</span></span>](../resources/list.md) | <span data-ttu-id="5223f-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-162">Sites.ReadWrite.All</span></span> | <span data-ttu-id="5223f-163">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-163">Not supported</span></span> | <span data-ttu-id="5223f-164">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-164">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="5223f-165">message</span><span class="sxs-lookup"><span data-stu-id="5223f-165">message</span></span>](../resources/message.md) | <span data-ttu-id="5223f-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5223f-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-167">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5223f-168">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5223f-168">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="5223f-169">presence</span><span class="sxs-lookup"><span data-stu-id="5223f-169">presence</span></span>](../resources/presence.md) | <span data-ttu-id="5223f-170">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-170">Presence.Read.All</span></span> | <span data-ttu-id="5223f-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-171">Not supported</span></span> | <span data-ttu-id="5223f-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-172">Not supported</span></span> |
|[<span data-ttu-id="5223f-173">printer</span><span class="sxs-lookup"><span data-stu-id="5223f-173">printer</span></span>](../resources/printer.md) | <span data-ttu-id="5223f-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-174">Not supported</span></span> | <span data-ttu-id="5223f-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-175">Not supported</span></span> | <span data-ttu-id="5223f-176">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-176">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="5223f-177">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5223f-177">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="5223f-178">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-178">Not supported</span></span> | <span data-ttu-id="5223f-179">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-179">Not supported</span></span> | <span data-ttu-id="5223f-180">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-180">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="5223f-181">security alert</span><span class="sxs-lookup"><span data-stu-id="5223f-181">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="5223f-182">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-182">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="5223f-183">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-183">Not supported</span></span> | <span data-ttu-id="5223f-184">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5223f-184">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="5223f-185">todoTask</span><span class="sxs-lookup"><span data-stu-id="5223f-185">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="5223f-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5223f-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="5223f-187">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5223f-187">Tasks.ReadWrite</span></span> | <span data-ttu-id="5223f-188">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5223f-188">Not supported</span></span> |
|[<span data-ttu-id="5223f-189">user</span><span class="sxs-lookup"><span data-stu-id="5223f-189">user</span></span>](../resources/user.md) | <span data-ttu-id="5223f-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-190">User.Read.All</span></span> | <span data-ttu-id="5223f-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-191">User.Read.All</span></span> | <span data-ttu-id="5223f-192">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5223f-192">User.Read.All</span></span> |

> <span data-ttu-id="5223f-193">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="5223f-193">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="5223f-194">driveItem</span><span class="sxs-lookup"><span data-stu-id="5223f-194">driveItem</span></span>

<span data-ttu-id="5223f-195">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5223f-195">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="5223f-196">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="5223f-196">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="5223f-197">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="5223f-197">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="5223f-198">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="5223f-198">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="5223f-199">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="5223f-199">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="5223f-200">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="5223f-200">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="5223f-201">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="5223f-201">contact, event, and message</span></span>

<span data-ttu-id="5223f-202">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="5223f-202">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="5223f-203">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="5223f-203">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="5223f-204">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="5223f-204">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="5223f-205">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5223f-205">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="5223f-206">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="5223f-206">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="5223f-207">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5223f-207">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="5223f-208">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="5223f-208">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="5223f-209">presence</span><span class="sxs-lookup"><span data-stu-id="5223f-209">presence</span></span>

<span data-ttu-id="5223f-210">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="5223f-210">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="5223f-211">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="5223f-211">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="5223f-212">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5223f-212">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5223f-213">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5223f-213">Request headers</span></span>

| <span data-ttu-id="5223f-214">Имя</span><span class="sxs-lookup"><span data-stu-id="5223f-214">Name</span></span>       | <span data-ttu-id="5223f-215">Тип</span><span class="sxs-lookup"><span data-stu-id="5223f-215">Type</span></span> | <span data-ttu-id="5223f-216">Описание</span><span class="sxs-lookup"><span data-stu-id="5223f-216">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5223f-217">Authorization</span><span class="sxs-lookup"><span data-stu-id="5223f-217">Authorization</span></span>  | <span data-ttu-id="5223f-218">string</span><span class="sxs-lookup"><span data-stu-id="5223f-218">string</span></span>  | <span data-ttu-id="5223f-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5223f-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5223f-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="5223f-221">Response</span></span>

<span data-ttu-id="5223f-222">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5223f-222">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="5223f-223">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="5223f-223">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="5223f-224">Пример</span><span class="sxs-lookup"><span data-stu-id="5223f-224">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5223f-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="5223f-225">Request</span></span>

<span data-ttu-id="5223f-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5223f-226">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5223f-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="5223f-227">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5223f-228">C#</span><span class="sxs-lookup"><span data-stu-id="5223f-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5223f-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5223f-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5223f-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5223f-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5223f-231">Java</span><span class="sxs-lookup"><span data-stu-id="5223f-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5223f-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="5223f-232">Response</span></span>

<span data-ttu-id="5223f-233">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5223f-233">Here is an example of the response.</span></span>
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
  "includeResourceData": false
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


