---
title: Создание подписки
description: Подписывает приложение прослушиватель на получение уведомлений об изменениях при изменении данных ресурса Microsoft Graph.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 68e748a054812350c7aad029d604e87aa77b7345
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034277"
---
# <a name="create-subscription"></a><span data-ttu-id="7c57a-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="7c57a-103">Create subscription</span></span>

<span data-ttu-id="7c57a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c57a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c57a-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7c57a-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c57a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c57a-106">Permissions</span></span>

<span data-ttu-id="7c57a-107">Для создания подписки требуется разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="7c57a-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="7c57a-108">Например, чтобы получать уведомления об изменениях в сообщениях, приложению необходимо разрешение Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="7c57a-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="7c57a-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7c57a-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="7c57a-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c57a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c57a-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="7c57a-111">Supported resource</span></span> | <span data-ttu-id="7c57a-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c57a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7c57a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c57a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c57a-114">Application</span><span class="sxs-lookup"><span data-stu-id="7c57a-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="7c57a-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="7c57a-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="7c57a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-116">Not supported</span></span> | <span data-ttu-id="7c57a-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-117">Not supported</span></span> | <span data-ttu-id="7c57a-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="7c57a-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7c57a-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="7c57a-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="7c57a-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-121">Not supported</span></span> | <span data-ttu-id="7c57a-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7c57a-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="7c57a-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="7c57a-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-124">Not supported</span></span> | <span data-ttu-id="7c57a-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-125">Not supported</span></span> | <span data-ttu-id="7c57a-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="7c57a-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="7c57a-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="7c57a-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c57a-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="7c57a-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-129">Not supported</span></span> | <span data-ttu-id="7c57a-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="7c57a-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="7c57a-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="7c57a-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-132">Not supported</span></span> | <span data-ttu-id="7c57a-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-133">Not supported</span></span> | <span data-ttu-id="7c57a-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="7c57a-135">contact</span><span class="sxs-lookup"><span data-stu-id="7c57a-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="7c57a-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-136">Contacts.Read</span></span> | <span data-ttu-id="7c57a-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-137">Contacts.Read</span></span> | <span data-ttu-id="7c57a-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-138">Contacts.Read</span></span> |
|<span data-ttu-id="7c57a-139">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="7c57a-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="7c57a-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-140">Not supported</span></span> | <span data-ttu-id="7c57a-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c57a-141">Files.ReadWrite</span></span> | <span data-ttu-id="7c57a-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-142">Not supported</span></span> |
|<span data-ttu-id="7c57a-143">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="7c57a-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="7c57a-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="7c57a-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-145">Not supported</span></span> | <span data-ttu-id="7c57a-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="7c57a-147">event</span><span class="sxs-lookup"><span data-stu-id="7c57a-147">event</span></span>](../resources/event.md) | <span data-ttu-id="7c57a-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-148">Calendars.Read</span></span> | <span data-ttu-id="7c57a-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-149">Calendars.Read</span></span> | <span data-ttu-id="7c57a-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-150">Calendars.Read</span></span> |
|[<span data-ttu-id="7c57a-151">group</span><span class="sxs-lookup"><span data-stu-id="7c57a-151">group</span></span>](../resources/group.md) | <span data-ttu-id="7c57a-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-152">Group.Read.All</span></span> | <span data-ttu-id="7c57a-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-153">Not supported</span></span> | <span data-ttu-id="7c57a-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-154">Group.Read.All</span></span> |
|[<span data-ttu-id="7c57a-155">group conversation</span><span class="sxs-lookup"><span data-stu-id="7c57a-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="7c57a-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-156">Group.Read.All</span></span> | <span data-ttu-id="7c57a-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-157">Not supported</span></span> | <span data-ttu-id="7c57a-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-158">Not supported</span></span> |
|[<span data-ttu-id="7c57a-159">list</span><span class="sxs-lookup"><span data-stu-id="7c57a-159">list</span></span>](../resources/list.md) | <span data-ttu-id="7c57a-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="7c57a-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-161">Not supported</span></span> | <span data-ttu-id="7c57a-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="7c57a-163">message</span><span class="sxs-lookup"><span data-stu-id="7c57a-163">message</span></span>](../resources/message.md) | <span data-ttu-id="7c57a-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7c57a-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="7c57a-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7c57a-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="7c57a-167">presence</span><span class="sxs-lookup"><span data-stu-id="7c57a-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="7c57a-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-168">Presence.Read.All</span></span> | <span data-ttu-id="7c57a-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-169">Not supported</span></span> | <span data-ttu-id="7c57a-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-170">Not supported</span></span> |
|[<span data-ttu-id="7c57a-171">printer</span><span class="sxs-lookup"><span data-stu-id="7c57a-171">printer</span></span>](../resources/printer.md) | <span data-ttu-id="7c57a-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-172">Not supported</span></span> | <span data-ttu-id="7c57a-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-173">Not supported</span></span> | <span data-ttu-id="7c57a-174">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-174">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="7c57a-175">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="7c57a-175">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="7c57a-176">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-176">Not supported</span></span> | <span data-ttu-id="7c57a-177">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-177">Not supported</span></span> | <span data-ttu-id="7c57a-178">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-178">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="7c57a-179">security alert</span><span class="sxs-lookup"><span data-stu-id="7c57a-179">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="7c57a-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-180">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="7c57a-181">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-181">Not supported</span></span> | <span data-ttu-id="7c57a-182">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-182">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="7c57a-183">todoTask</span><span class="sxs-lookup"><span data-stu-id="7c57a-183">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="7c57a-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c57a-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="7c57a-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c57a-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="7c57a-186">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c57a-186">Not supported</span></span> |
|[<span data-ttu-id="7c57a-187">user</span><span class="sxs-lookup"><span data-stu-id="7c57a-187">user</span></span>](../resources/user.md) | <span data-ttu-id="7c57a-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-188">User.Read.All</span></span> | <span data-ttu-id="7c57a-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-189">User.Read.All</span></span> | <span data-ttu-id="7c57a-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c57a-190">User.Read.All</span></span> |

> <span data-ttu-id="7c57a-191">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="7c57a-191">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="7c57a-192">driveItem</span><span class="sxs-lookup"><span data-stu-id="7c57a-192">driveItem</span></span>

<span data-ttu-id="7c57a-193">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7c57a-193">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="7c57a-194">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="7c57a-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="7c57a-195">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="7c57a-195">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="7c57a-196">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="7c57a-196">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="7c57a-197">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="7c57a-197">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="7c57a-198">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="7c57a-198">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="7c57a-199">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="7c57a-199">contact, event, and message</span></span>

<span data-ttu-id="7c57a-200">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="7c57a-200">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="7c57a-201">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="7c57a-201">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="7c57a-202">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="7c57a-202">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="7c57a-203">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c57a-203">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="7c57a-204">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="7c57a-204">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="7c57a-205">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="7c57a-205">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="7c57a-206">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="7c57a-206">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="7c57a-207">presence</span><span class="sxs-lookup"><span data-stu-id="7c57a-207">presence</span></span>

<span data-ttu-id="7c57a-208">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="7c57a-208">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="7c57a-209">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="7c57a-209">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="7c57a-210">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c57a-210">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="7c57a-211">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c57a-211">Request headers</span></span>

| <span data-ttu-id="7c57a-212">Имя</span><span class="sxs-lookup"><span data-stu-id="7c57a-212">Name</span></span>       | <span data-ttu-id="7c57a-213">Тип</span><span class="sxs-lookup"><span data-stu-id="7c57a-213">Type</span></span> | <span data-ttu-id="7c57a-214">Описание</span><span class="sxs-lookup"><span data-stu-id="7c57a-214">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7c57a-215">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c57a-215">Authorization</span></span>  | <span data-ttu-id="7c57a-216">string</span><span class="sxs-lookup"><span data-stu-id="7c57a-216">string</span></span>  | <span data-ttu-id="7c57a-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c57a-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7c57a-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c57a-219">Response</span></span>

<span data-ttu-id="7c57a-220">В случае успеха этот метод возвращает код отклика и `201 Created` объект [подписки](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c57a-220">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="7c57a-221">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="7c57a-221">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="7c57a-222">Пример</span><span class="sxs-lookup"><span data-stu-id="7c57a-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c57a-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c57a-223">Request</span></span>

<span data-ttu-id="7c57a-224">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c57a-224">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="7c57a-225">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="7c57a-225">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="7c57a-226">Этот запрос создает подписку для уведомлений об изменениях о новых сообщениях, полученных текущим пользователем, выписав его.</span><span class="sxs-lookup"><span data-stu-id="7c57a-226">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c57a-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c57a-227">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7c57a-228">C#</span><span class="sxs-lookup"><span data-stu-id="7c57a-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c57a-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c57a-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c57a-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c57a-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c57a-231">Java</span><span class="sxs-lookup"><span data-stu-id="7c57a-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7c57a-232">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c57a-232">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="7c57a-233">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="7c57a-233">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="7c57a-234">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="7c57a-234">Resources examples</span></span>

<span data-ttu-id="7c57a-235">Ниже следующую допустимую величину свойства ресурса.</span><span class="sxs-lookup"><span data-stu-id="7c57a-235">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="7c57a-236">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="7c57a-236">Resource type</span></span> | <span data-ttu-id="7c57a-237">Примеры</span><span class="sxs-lookup"><span data-stu-id="7c57a-237">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="7c57a-238">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="7c57a-238">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="7c57a-239">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="7c57a-239">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7c57a-240">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="7c57a-240">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="7c57a-241">Контакты</span><span class="sxs-lookup"><span data-stu-id="7c57a-241">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="7c57a-242">Беседы</span><span class="sxs-lookup"><span data-stu-id="7c57a-242">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="7c57a-243">Диски</span><span class="sxs-lookup"><span data-stu-id="7c57a-243">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="7c57a-244">События</span><span class="sxs-lookup"><span data-stu-id="7c57a-244">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="7c57a-245">Группы</span><span class="sxs-lookup"><span data-stu-id="7c57a-245">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="7c57a-246">Список</span><span class="sxs-lookup"><span data-stu-id="7c57a-246">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="7c57a-247">Почта</span><span class="sxs-lookup"><span data-stu-id="7c57a-247">Mail</span></span>](../resources/message.md)|<span data-ttu-id="7c57a-248">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="7c57a-248">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="7c57a-249">Присутствие</span><span class="sxs-lookup"><span data-stu-id="7c57a-249">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="7c57a-250">`/communications/presences/{id}` (один пользователь), `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="7c57a-250">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="7c57a-251">printer</span><span class="sxs-lookup"><span data-stu-id="7c57a-251">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="7c57a-252">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="7c57a-252">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="7c57a-253">Пользователи</span><span class="sxs-lookup"><span data-stu-id="7c57a-253">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="7c57a-254">todoTask</span><span class="sxs-lookup"><span data-stu-id="7c57a-254">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="7c57a-255">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="7c57a-255">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="7c57a-256">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c57a-256">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="7c57a-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c57a-257">Response</span></span>

<span data-ttu-id="7c57a-258">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c57a-258">The following example shows the response.</span></span> 

><span data-ttu-id="7c57a-p111">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c57a-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "latestSupportedTlsVersion": "v1_2"
}
```

### <a name="notification-endpoint-validation"></a><span data-ttu-id="7c57a-261">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="7c57a-261">Notification endpoint validation</span></span>

<span data-ttu-id="7c57a-262">Конечная точка уведомлений о подписке (указанная в свойстве **notificationUrl)** должна отвечать на запрос проверки, как описано в описании в настройках уведомлений об изменениях данных [пользователя.](/graph/webhooks#notification-endpoint-validation)</span><span class="sxs-lookup"><span data-stu-id="7c57a-262">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="7c57a-263">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="7c57a-263">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


