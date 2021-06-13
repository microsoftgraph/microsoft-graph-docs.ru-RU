---
title: Создание подписки
description: Подписывает приложение-слушатель для получения уведомлений об изменениях при изменении данных о Graph microsoft.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: b471d13836faa74ba6f77ab395e9a8ad3c87e4ad
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911874"
---
# <a name="create-subscription"></a><span data-ttu-id="26b46-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="26b46-103">Create subscription</span></span>

<span data-ttu-id="26b46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26b46-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="26b46-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="26b46-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="26b46-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="26b46-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26b46-107">Permissions</span></span>

<span data-ttu-id="26b46-108">Для создания подписки требуется разрешение на чтение на ресурс.</span><span class="sxs-lookup"><span data-stu-id="26b46-108">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="26b46-109">Например, чтобы получать уведомления об изменениях в сообщениях, вашему приложению необходимо разрешение Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="26b46-109">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

<span data-ttu-id="26b46-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="26b46-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="26b46-111">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26b46-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26b46-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="26b46-112">Supported resource</span></span> | <span data-ttu-id="26b46-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26b46-113">Delegated (work or school account)</span></span> | <span data-ttu-id="26b46-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26b46-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26b46-115">Application</span><span class="sxs-lookup"><span data-stu-id="26b46-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="26b46-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="26b46-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="26b46-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-117">Not supported</span></span> | <span data-ttu-id="26b46-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-118">Not supported</span></span> | <span data-ttu-id="26b46-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="26b46-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="26b46-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="26b46-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="26b46-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-122">Not supported</span></span> | <span data-ttu-id="26b46-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="26b46-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="26b46-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="26b46-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-125">Not supported</span></span> | <span data-ttu-id="26b46-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-126">Not supported</span></span> | <span data-ttu-id="26b46-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="26b46-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="26b46-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="26b46-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b46-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="26b46-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-130">Not supported</span></span> | <span data-ttu-id="26b46-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="26b46-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="26b46-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="26b46-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-133">Not supported</span></span> | <span data-ttu-id="26b46-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-134">Not supported</span></span> | <span data-ttu-id="26b46-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="26b46-136">contact</span><span class="sxs-lookup"><span data-stu-id="26b46-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="26b46-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-137">Contacts.Read</span></span> | <span data-ttu-id="26b46-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-138">Contacts.Read</span></span> | <span data-ttu-id="26b46-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-139">Contacts.Read</span></span> |
|<span data-ttu-id="26b46-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="26b46-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="26b46-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-141">Not supported</span></span> | <span data-ttu-id="26b46-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b46-142">Files.ReadWrite</span></span> | <span data-ttu-id="26b46-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-143">Not supported</span></span> |
|<span data-ttu-id="26b46-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="26b46-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="26b46-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="26b46-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-146">Not supported</span></span> | <span data-ttu-id="26b46-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="26b46-148">event</span><span class="sxs-lookup"><span data-stu-id="26b46-148">event</span></span>](../resources/event.md) | <span data-ttu-id="26b46-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-149">Calendars.Read</span></span> | <span data-ttu-id="26b46-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-150">Calendars.Read</span></span> | <span data-ttu-id="26b46-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-151">Calendars.Read</span></span> |
|[<span data-ttu-id="26b46-152">group</span><span class="sxs-lookup"><span data-stu-id="26b46-152">group</span></span>](../resources/group.md) | <span data-ttu-id="26b46-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-153">Group.Read.All</span></span> | <span data-ttu-id="26b46-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-154">Not supported</span></span> | <span data-ttu-id="26b46-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-155">Group.Read.All</span></span> |
|[<span data-ttu-id="26b46-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="26b46-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="26b46-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-157">Group.Read.All</span></span> | <span data-ttu-id="26b46-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-158">Not supported</span></span> | <span data-ttu-id="26b46-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-159">Not supported</span></span> |
|[<span data-ttu-id="26b46-160">list</span><span class="sxs-lookup"><span data-stu-id="26b46-160">list</span></span>](../resources/list.md) | <span data-ttu-id="26b46-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="26b46-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-162">Not supported</span></span> | <span data-ttu-id="26b46-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="26b46-164">message</span><span class="sxs-lookup"><span data-stu-id="26b46-164">message</span></span>](../resources/message.md) | <span data-ttu-id="26b46-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="26b46-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="26b46-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="26b46-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="26b46-168">presence</span><span class="sxs-lookup"><span data-stu-id="26b46-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="26b46-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-169">Presence.Read.All</span></span> | <span data-ttu-id="26b46-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-170">Not supported</span></span> | <span data-ttu-id="26b46-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-171">Not supported</span></span> |
|[<span data-ttu-id="26b46-172">printer</span><span class="sxs-lookup"><span data-stu-id="26b46-172">printer</span></span>](../resources/printer.md) | <span data-ttu-id="26b46-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-173">Not supported</span></span> | <span data-ttu-id="26b46-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-174">Not supported</span></span> | <span data-ttu-id="26b46-175">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-175">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="26b46-176">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="26b46-176">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="26b46-177">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-177">Not supported</span></span> | <span data-ttu-id="26b46-178">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-178">Not supported</span></span> | <span data-ttu-id="26b46-179">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-179">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="26b46-180">security alert</span><span class="sxs-lookup"><span data-stu-id="26b46-180">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="26b46-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-181">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="26b46-182">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-182">Not supported</span></span> | <span data-ttu-id="26b46-183">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b46-183">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="26b46-184">todoTask</span><span class="sxs-lookup"><span data-stu-id="26b46-184">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="26b46-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b46-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="26b46-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b46-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="26b46-187">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="26b46-187">Not supported</span></span> |
|[<span data-ttu-id="26b46-188">user</span><span class="sxs-lookup"><span data-stu-id="26b46-188">user</span></span>](../resources/user.md) | <span data-ttu-id="26b46-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-189">User.Read.All</span></span> | <span data-ttu-id="26b46-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-190">User.Read.All</span></span> | <span data-ttu-id="26b46-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b46-191">User.Read.All</span></span> |

> <span data-ttu-id="26b46-192">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="26b46-192">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="26b46-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="26b46-193">driveItem</span></span>

<span data-ttu-id="26b46-194">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="26b46-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="26b46-195">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="26b46-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="26b46-196">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="26b46-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="26b46-197">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="26b46-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="26b46-198">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="26b46-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="26b46-199">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="26b46-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

<span data-ttu-id="26b46-200">OneDrive для бизнеса и SharePoint поддержку отправки приложениям уведомлений о событиях безопасности, происходящих на **driveItem.**</span><span class="sxs-lookup"><span data-stu-id="26b46-200">OneDrive for Business and SharePoint support sending your application notifications of security events that occur on a **driveItem**.</span></span> <span data-ttu-id="26b46-201">Чтобы подписаться на эти события, добавьте `prefer:includesecuritywebhooks` заглавную в запрос для создания подписки.</span><span class="sxs-lookup"><span data-stu-id="26b46-201">To subscribe to these events, add the `prefer:includesecuritywebhooks` header to your request to create a subscription.</span></span> <span data-ttu-id="26b46-202">После создания подписки вы будете получать уведомления при изменении разрешений на элемент.</span><span class="sxs-lookup"><span data-stu-id="26b46-202">After the subscription is created, you will receive notifications when the permissions on an item change.</span></span> <span data-ttu-id="26b46-203">Эта заглавная запись применима к SharePoint и OneDrive для бизнеса, но не к OneDrive учетным записям.</span><span class="sxs-lookup"><span data-stu-id="26b46-203">This header is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="26b46-204">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="26b46-204">contact, event, and message</span></span>

<span data-ttu-id="26b46-205">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="26b46-205">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="26b46-206">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="26b46-206">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="26b46-207">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="26b46-207">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="26b46-208">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="26b46-208">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="26b46-209">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="26b46-209">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="26b46-210">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="26b46-210">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="26b46-211">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="26b46-211">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="26b46-212">presence</span><span class="sxs-lookup"><span data-stu-id="26b46-212">presence</span></span>

<span data-ttu-id="26b46-213">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="26b46-213">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="26b46-214">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="26b46-214">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="26b46-215">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26b46-215">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="26b46-216">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26b46-216">Request headers</span></span>

| <span data-ttu-id="26b46-217">Имя</span><span class="sxs-lookup"><span data-stu-id="26b46-217">Name</span></span>       | <span data-ttu-id="26b46-218">Тип</span><span class="sxs-lookup"><span data-stu-id="26b46-218">Type</span></span> | <span data-ttu-id="26b46-219">Описание</span><span class="sxs-lookup"><span data-stu-id="26b46-219">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="26b46-220">Authorization</span><span class="sxs-lookup"><span data-stu-id="26b46-220">Authorization</span></span>  | <span data-ttu-id="26b46-221">string</span><span class="sxs-lookup"><span data-stu-id="26b46-221">string</span></span>  | <span data-ttu-id="26b46-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26b46-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="26b46-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b46-224">Response</span></span>

<span data-ttu-id="26b46-225">В случае успешного использования этот метод возвращает код отклика и объект подписки `201 Created` в тексте [](../resources/subscription.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="26b46-225">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="26b46-226">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="26b46-226">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="26b46-227">Пример</span><span class="sxs-lookup"><span data-stu-id="26b46-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="26b46-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="26b46-228">Request</span></span>

<span data-ttu-id="26b46-229">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26b46-229">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="26b46-230">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="26b46-230">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="26b46-231">Этот запрос создает подписку на уведомления об изменениях о новой почте, полученной в настоящее время подписанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="26b46-231">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="26b46-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b46-232">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="26b46-233">C#</span><span class="sxs-lookup"><span data-stu-id="26b46-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b46-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b46-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b46-235">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b46-235">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26b46-236">Java</span><span class="sxs-lookup"><span data-stu-id="26b46-236">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="26b46-237">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26b46-237">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="26b46-238">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="26b46-238">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="26b46-239">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="26b46-239">Resources examples</span></span>

<span data-ttu-id="26b46-240">Ниже приводится допустимые значения для свойства ресурса.</span><span class="sxs-lookup"><span data-stu-id="26b46-240">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="26b46-241">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="26b46-241">Resource type</span></span> | <span data-ttu-id="26b46-242">Примеры</span><span class="sxs-lookup"><span data-stu-id="26b46-242">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="26b46-243">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="26b46-243">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="26b46-244">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="26b46-244">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="26b46-245">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="26b46-245">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="26b46-246">Контакты</span><span class="sxs-lookup"><span data-stu-id="26b46-246">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="26b46-247">Беседы</span><span class="sxs-lookup"><span data-stu-id="26b46-247">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="26b46-248">Диски</span><span class="sxs-lookup"><span data-stu-id="26b46-248">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="26b46-249">События</span><span class="sxs-lookup"><span data-stu-id="26b46-249">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="26b46-250">Группы</span><span class="sxs-lookup"><span data-stu-id="26b46-250">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="26b46-251">Список</span><span class="sxs-lookup"><span data-stu-id="26b46-251">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="26b46-252">Почта</span><span class="sxs-lookup"><span data-stu-id="26b46-252">Mail</span></span>](../resources/message.md)|<span data-ttu-id="26b46-253">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="26b46-253">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="26b46-254">Присутствие</span><span class="sxs-lookup"><span data-stu-id="26b46-254">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="26b46-255">`/communications/presences/{id}` (один пользователь), `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="26b46-255">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="26b46-256">printer</span><span class="sxs-lookup"><span data-stu-id="26b46-256">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="26b46-257">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="26b46-257">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="26b46-258">Пользователи</span><span class="sxs-lookup"><span data-stu-id="26b46-258">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="26b46-259">todoTask</span><span class="sxs-lookup"><span data-stu-id="26b46-259">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="26b46-260">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="26b46-260">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="26b46-261">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="26b46-261">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="26b46-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b46-262">Response</span></span>

<span data-ttu-id="26b46-263">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26b46-263">The following example shows the response.</span></span> 

><span data-ttu-id="26b46-264">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26b46-264">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="26b46-265">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="26b46-265">Notification endpoint validation</span></span>

<span data-ttu-id="26b46-266">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl)** должна быть способна отвечать на запрос проверки, как описано в настройках уведомлений об изменениях в пользовательских [данных.](/graph/webhooks#notification-endpoint-validation)</span><span class="sxs-lookup"><span data-stu-id="26b46-266">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="26b46-267">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="26b46-267">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


