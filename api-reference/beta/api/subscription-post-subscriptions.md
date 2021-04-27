---
title: Создание подписки
description: Подписывает приложение-слушатель для получения уведомлений об изменениях при изменении данных о Graph microsoft.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 7fe6db48038b68d7d2bfe507af60a26846962832
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054877"
---
# <a name="create-subscription"></a><span data-ttu-id="96e70-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="96e70-103">Create subscription</span></span>

<span data-ttu-id="96e70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96e70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96e70-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96e70-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="96e70-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="96e70-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="96e70-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96e70-107">Permissions</span></span>

<span data-ttu-id="96e70-108">Для создания подписки требуется разрешение на чтение на ресурс.</span><span class="sxs-lookup"><span data-stu-id="96e70-108">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="96e70-109">Например, чтобы получать уведомления об изменениях в сообщениях, вашему приложению необходимо разрешение Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="96e70-109">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

<span data-ttu-id="96e70-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="96e70-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="96e70-111">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96e70-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96e70-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="96e70-112">Supported resource</span></span> | <span data-ttu-id="96e70-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96e70-113">Delegated (work or school account)</span></span> | <span data-ttu-id="96e70-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96e70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96e70-115">Application</span><span class="sxs-lookup"><span data-stu-id="96e70-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="96e70-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="96e70-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="96e70-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-117">Not supported</span></span> | <span data-ttu-id="96e70-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-118">Not supported</span></span> | <span data-ttu-id="96e70-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="96e70-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="96e70-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="96e70-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="96e70-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-122">Not supported</span></span> | <span data-ttu-id="96e70-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="96e70-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="96e70-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="96e70-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-125">Not supported</span></span> | <span data-ttu-id="96e70-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-126">Not supported</span></span> | <span data-ttu-id="96e70-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="96e70-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="96e70-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="96e70-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96e70-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="96e70-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-130">Not supported</span></span> | <span data-ttu-id="96e70-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="96e70-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="96e70-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="96e70-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-133">Not supported</span></span> | <span data-ttu-id="96e70-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-134">Not supported</span></span> | <span data-ttu-id="96e70-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="96e70-136">contact</span><span class="sxs-lookup"><span data-stu-id="96e70-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="96e70-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-137">Contacts.Read</span></span> | <span data-ttu-id="96e70-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-138">Contacts.Read</span></span> | <span data-ttu-id="96e70-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-139">Contacts.Read</span></span> |
|<span data-ttu-id="96e70-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="96e70-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="96e70-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-141">Not supported</span></span> | <span data-ttu-id="96e70-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96e70-142">Files.ReadWrite</span></span> | <span data-ttu-id="96e70-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-143">Not supported</span></span> |
|<span data-ttu-id="96e70-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="96e70-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="96e70-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="96e70-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-146">Not supported</span></span> | <span data-ttu-id="96e70-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="96e70-148">event</span><span class="sxs-lookup"><span data-stu-id="96e70-148">event</span></span>](../resources/event.md) | <span data-ttu-id="96e70-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-149">Calendars.Read</span></span> | <span data-ttu-id="96e70-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-150">Calendars.Read</span></span> | <span data-ttu-id="96e70-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-151">Calendars.Read</span></span> |
|[<span data-ttu-id="96e70-152">group</span><span class="sxs-lookup"><span data-stu-id="96e70-152">group</span></span>](../resources/group.md) | <span data-ttu-id="96e70-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-153">Group.Read.All</span></span> | <span data-ttu-id="96e70-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-154">Not supported</span></span> | <span data-ttu-id="96e70-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-155">Group.Read.All</span></span> |
|[<span data-ttu-id="96e70-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="96e70-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="96e70-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-157">Group.Read.All</span></span> | <span data-ttu-id="96e70-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-158">Not supported</span></span> | <span data-ttu-id="96e70-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-159">Not supported</span></span> |
|[<span data-ttu-id="96e70-160">list</span><span class="sxs-lookup"><span data-stu-id="96e70-160">list</span></span>](../resources/list.md) | <span data-ttu-id="96e70-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="96e70-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-162">Not supported</span></span> | <span data-ttu-id="96e70-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="96e70-164">message</span><span class="sxs-lookup"><span data-stu-id="96e70-164">message</span></span>](../resources/message.md) | <span data-ttu-id="96e70-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="96e70-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="96e70-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="96e70-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="96e70-168">presence</span><span class="sxs-lookup"><span data-stu-id="96e70-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="96e70-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-169">Presence.Read.All</span></span> | <span data-ttu-id="96e70-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-170">Not supported</span></span> | <span data-ttu-id="96e70-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-171">Not supported</span></span> |
|[<span data-ttu-id="96e70-172">printer</span><span class="sxs-lookup"><span data-stu-id="96e70-172">printer</span></span>](../resources/printer.md) | <span data-ttu-id="96e70-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-173">Not supported</span></span> | <span data-ttu-id="96e70-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-174">Not supported</span></span> | <span data-ttu-id="96e70-175">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-175">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="96e70-176">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="96e70-176">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="96e70-177">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-177">Not supported</span></span> | <span data-ttu-id="96e70-178">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-178">Not supported</span></span> | <span data-ttu-id="96e70-179">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-179">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="96e70-180">security alert</span><span class="sxs-lookup"><span data-stu-id="96e70-180">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="96e70-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-181">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="96e70-182">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-182">Not supported</span></span> | <span data-ttu-id="96e70-183">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e70-183">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="96e70-184">todoTask</span><span class="sxs-lookup"><span data-stu-id="96e70-184">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="96e70-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96e70-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="96e70-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96e70-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="96e70-187">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="96e70-187">Not supported</span></span> |
|[<span data-ttu-id="96e70-188">user</span><span class="sxs-lookup"><span data-stu-id="96e70-188">user</span></span>](../resources/user.md) | <span data-ttu-id="96e70-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-189">User.Read.All</span></span> | <span data-ttu-id="96e70-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-190">User.Read.All</span></span> | <span data-ttu-id="96e70-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e70-191">User.Read.All</span></span> |

> <span data-ttu-id="96e70-192">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="96e70-192">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="96e70-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="96e70-193">driveItem</span></span>

<span data-ttu-id="96e70-194">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="96e70-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="96e70-195">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="96e70-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="96e70-196">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="96e70-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="96e70-197">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="96e70-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="96e70-198">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="96e70-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="96e70-199">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="96e70-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="96e70-200">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="96e70-200">contact, event, and message</span></span>

<span data-ttu-id="96e70-201">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="96e70-201">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="96e70-202">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="96e70-202">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="96e70-203">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="96e70-203">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="96e70-204">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="96e70-204">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="96e70-205">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="96e70-205">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="96e70-206">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="96e70-206">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="96e70-207">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="96e70-207">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="96e70-208">presence</span><span class="sxs-lookup"><span data-stu-id="96e70-208">presence</span></span>

<span data-ttu-id="96e70-209">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="96e70-209">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="96e70-210">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="96e70-210">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="96e70-211">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96e70-211">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="96e70-212">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96e70-212">Request headers</span></span>

| <span data-ttu-id="96e70-213">Имя</span><span class="sxs-lookup"><span data-stu-id="96e70-213">Name</span></span>       | <span data-ttu-id="96e70-214">Тип</span><span class="sxs-lookup"><span data-stu-id="96e70-214">Type</span></span> | <span data-ttu-id="96e70-215">Описание</span><span class="sxs-lookup"><span data-stu-id="96e70-215">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96e70-216">Authorization</span><span class="sxs-lookup"><span data-stu-id="96e70-216">Authorization</span></span>  | <span data-ttu-id="96e70-217">string</span><span class="sxs-lookup"><span data-stu-id="96e70-217">string</span></span>  | <span data-ttu-id="96e70-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96e70-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="96e70-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="96e70-220">Response</span></span>

<span data-ttu-id="96e70-221">В случае успешного использования этот метод возвращает код отклика и объект подписки `201 Created` в тексте [](../resources/subscription.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="96e70-221">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="96e70-222">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="96e70-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="96e70-223">Пример</span><span class="sxs-lookup"><span data-stu-id="96e70-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="96e70-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="96e70-224">Request</span></span>

<span data-ttu-id="96e70-225">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96e70-225">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="96e70-226">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="96e70-226">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="96e70-227">Этот запрос создает подписку на уведомления об изменениях о новой почте, полученной в настоящее время подписанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="96e70-227">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="96e70-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="96e70-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
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
# <a name="c"></a>[<span data-ttu-id="96e70-229">C#</span><span class="sxs-lookup"><span data-stu-id="96e70-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96e70-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96e70-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96e70-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96e70-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96e70-232">Java</span><span class="sxs-lookup"><span data-stu-id="96e70-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="96e70-233">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96e70-233">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="96e70-234">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="96e70-234">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="96e70-235">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="96e70-235">Resources examples</span></span>

<span data-ttu-id="96e70-236">Ниже приводится допустимые значения для свойства ресурса.</span><span class="sxs-lookup"><span data-stu-id="96e70-236">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="96e70-237">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="96e70-237">Resource type</span></span> | <span data-ttu-id="96e70-238">Примеры</span><span class="sxs-lookup"><span data-stu-id="96e70-238">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="96e70-239">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="96e70-239">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="96e70-240">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="96e70-240">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="96e70-241">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="96e70-241">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="96e70-242">Контакты</span><span class="sxs-lookup"><span data-stu-id="96e70-242">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="96e70-243">Беседы</span><span class="sxs-lookup"><span data-stu-id="96e70-243">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="96e70-244">Диски</span><span class="sxs-lookup"><span data-stu-id="96e70-244">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="96e70-245">События</span><span class="sxs-lookup"><span data-stu-id="96e70-245">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="96e70-246">Группы</span><span class="sxs-lookup"><span data-stu-id="96e70-246">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="96e70-247">Список</span><span class="sxs-lookup"><span data-stu-id="96e70-247">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="96e70-248">Почта</span><span class="sxs-lookup"><span data-stu-id="96e70-248">Mail</span></span>](../resources/message.md)|<span data-ttu-id="96e70-249">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="96e70-249">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="96e70-250">Присутствие</span><span class="sxs-lookup"><span data-stu-id="96e70-250">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="96e70-251">`/communications/presences/{id}` (один пользователь), `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="96e70-251">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="96e70-252">printer</span><span class="sxs-lookup"><span data-stu-id="96e70-252">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="96e70-253">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="96e70-253">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|<span data-ttu-id="96e70-254">[пользователи](../resources/user.md);</span><span class="sxs-lookup"><span data-stu-id="96e70-254">[Users](../resources/user.md)</span></span>|`users`|
|[<span data-ttu-id="96e70-255">todoTask</span><span class="sxs-lookup"><span data-stu-id="96e70-255">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="96e70-256">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="96e70-256">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="96e70-257">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="96e70-257">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="96e70-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="96e70-258">Response</span></span>

<span data-ttu-id="96e70-259">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96e70-259">The following example shows the response.</span></span> 

><span data-ttu-id="96e70-260">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="96e70-260">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="96e70-261">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="96e70-261">Notification endpoint validation</span></span>

<span data-ttu-id="96e70-262">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl)** должна быть способна отвечать на запрос проверки, как описано в настройках уведомлений об изменениях в пользовательских [данных.](/graph/webhooks#notification-endpoint-validation)</span><span class="sxs-lookup"><span data-stu-id="96e70-262">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="96e70-263">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="96e70-263">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


