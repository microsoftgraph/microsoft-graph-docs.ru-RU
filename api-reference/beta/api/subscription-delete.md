---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c6e8b1d203b5a14a4d450b459dbadeb06d2cfe45
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597188"
---
# <a name="delete-subscription"></a><span data-ttu-id="dd0e9-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="dd0e9-103">Delete subscription</span></span>

<span data-ttu-id="dd0e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd0e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd0e9-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd0e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd0e9-106">Permissions</span></span>

<span data-ttu-id="dd0e9-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="dd0e9-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd0e9-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="dd0e9-109">Supported resource</span></span> | <span data-ttu-id="dd0e9-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd0e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd0e9-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd0e9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd0e9-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd0e9-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="dd0e9-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="dd0e9-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="dd0e9-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-114">Not supported</span></span> | <span data-ttu-id="dd0e9-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-115">Not supported</span></span> | <span data-ttu-id="dd0e9-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="dd0e9-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="dd0e9-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="dd0e9-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="dd0e9-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-119">Not supported</span></span> | <span data-ttu-id="dd0e9-120">Чаннелмессаже. Read. Group \*, Чаннелмессаже. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="dd0e9-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="dd0e9-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="dd0e9-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="dd0e9-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-122">Not supported</span></span> | <span data-ttu-id="dd0e9-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-123">Not supported</span></span> | <span data-ttu-id="dd0e9-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="dd0e9-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="dd0e9-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="dd0e9-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd0e9-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="dd0e9-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-127">Not supported</span></span> | <span data-ttu-id="dd0e9-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="dd0e9-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="dd0e9-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="dd0e9-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-130">Not supported</span></span> | <span data-ttu-id="dd0e9-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-131">Not supported</span></span> | <span data-ttu-id="dd0e9-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="dd0e9-133">contact</span><span class="sxs-lookup"><span data-stu-id="dd0e9-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="dd0e9-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-134">Contacts.Read</span></span> | <span data-ttu-id="dd0e9-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-135">Contacts.Read</span></span> | <span data-ttu-id="dd0e9-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-136">Contacts.Read</span></span> |
|<span data-ttu-id="dd0e9-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="dd0e9-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="dd0e9-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-138">Not supported</span></span> | <span data-ttu-id="dd0e9-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd0e9-139">Files.ReadWrite</span></span> | <span data-ttu-id="dd0e9-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-140">Not supported</span></span> |
|<span data-ttu-id="dd0e9-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="dd0e9-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="dd0e9-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="dd0e9-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-143">Not supported</span></span> | <span data-ttu-id="dd0e9-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="dd0e9-145">event</span><span class="sxs-lookup"><span data-stu-id="dd0e9-145">event</span></span>](../resources/event.md) | <span data-ttu-id="dd0e9-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-146">Calendars.Read</span></span> | <span data-ttu-id="dd0e9-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-147">Calendars.Read</span></span> | <span data-ttu-id="dd0e9-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-148">Calendars.Read</span></span> |
|[<span data-ttu-id="dd0e9-149">group</span><span class="sxs-lookup"><span data-stu-id="dd0e9-149">group</span></span>](../resources/group.md) | <span data-ttu-id="dd0e9-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-150">Group.Read.All</span></span> | <span data-ttu-id="dd0e9-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-151">Not supported</span></span> | <span data-ttu-id="dd0e9-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-152">Group.Read.All</span></span> |
|[<span data-ttu-id="dd0e9-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="dd0e9-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="dd0e9-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-154">Group.Read.All</span></span> | <span data-ttu-id="dd0e9-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-155">Not supported</span></span> | <span data-ttu-id="dd0e9-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-156">Not supported</span></span> |
|[<span data-ttu-id="dd0e9-157">list</span><span class="sxs-lookup"><span data-stu-id="dd0e9-157">list</span></span>](../resources/list.md) | <span data-ttu-id="dd0e9-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="dd0e9-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-159">Not supported</span></span> | <span data-ttu-id="dd0e9-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="dd0e9-161">message</span><span class="sxs-lookup"><span data-stu-id="dd0e9-161">message</span></span>](../resources/message.md) | <span data-ttu-id="dd0e9-162">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="dd0e9-163">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="dd0e9-164">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="dd0e9-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="dd0e9-165">presence</span><span class="sxs-lookup"><span data-stu-id="dd0e9-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="dd0e9-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-166">Presence.Read.All</span></span> | <span data-ttu-id="dd0e9-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-167">Not supported</span></span> | <span data-ttu-id="dd0e9-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-168">Not supported</span></span> |
|[<span data-ttu-id="dd0e9-169">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="dd0e9-169">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="dd0e9-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-170">Not supported</span></span> | <span data-ttu-id="dd0e9-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-171">Not supported</span></span> | <span data-ttu-id="dd0e9-172">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-172">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="dd0e9-173">security alert</span><span class="sxs-lookup"><span data-stu-id="dd0e9-173">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="dd0e9-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-174">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="dd0e9-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-175">Not supported</span></span> | <span data-ttu-id="dd0e9-176">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-176">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="dd0e9-177">тодотаск</span><span class="sxs-lookup"><span data-stu-id="dd0e9-177">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="dd0e9-178">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd0e9-178">Tasks.ReadWrite</span></span> | <span data-ttu-id="dd0e9-179">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd0e9-179">Tasks.ReadWrite</span></span> | <span data-ttu-id="dd0e9-180">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dd0e9-180">Not supported</span></span> |
|[<span data-ttu-id="dd0e9-181">user</span><span class="sxs-lookup"><span data-stu-id="dd0e9-181">user</span></span>](../resources/user.md) | <span data-ttu-id="dd0e9-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-182">User.Read.All</span></span> | <span data-ttu-id="dd0e9-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-183">User.Read.All</span></span> | <span data-ttu-id="dd0e9-184">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0e9-184">User.Read.All</span></span> |

> <span data-ttu-id="dd0e9-185">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-185">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="dd0e9-186">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dd0e9-186">chatMessage</span></span>

<span data-ttu-id="dd0e9-187">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов (**инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-187">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="dd0e9-188">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-188">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="dd0e9-189">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-189">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="dd0e9-190">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-190">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="dd0e9-191">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-191">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="dd0e9-192">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-192">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="dd0e9-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="dd0e9-193">driveItem</span></span>

<span data-ttu-id="dd0e9-194">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="dd0e9-195">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="dd0e9-196">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="dd0e9-197">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="dd0e9-198">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="dd0e9-199">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="dd0e9-200">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="dd0e9-200">contact, event, and message</span></span>

<span data-ttu-id="dd0e9-201">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-201">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="dd0e9-202">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-202">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="dd0e9-203">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-203">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="dd0e9-204">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-204">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="dd0e9-205">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="dd0e9-205">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="dd0e9-206">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-206">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="dd0e9-207">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-207">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="dd0e9-208">presence</span><span class="sxs-lookup"><span data-stu-id="dd0e9-208">presence</span></span>

<span data-ttu-id="dd0e9-209">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-209">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="dd0e9-210">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="dd0e9-210">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="dd0e9-211">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd0e9-211">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="dd0e9-212">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd0e9-212">Request headers</span></span>

| <span data-ttu-id="dd0e9-213">Имя</span><span class="sxs-lookup"><span data-stu-id="dd0e9-213">Name</span></span>       | <span data-ttu-id="dd0e9-214">Тип</span><span class="sxs-lookup"><span data-stu-id="dd0e9-214">Type</span></span> | <span data-ttu-id="dd0e9-215">Описание</span><span class="sxs-lookup"><span data-stu-id="dd0e9-215">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dd0e9-216">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd0e9-216">Authorization</span></span>  | <span data-ttu-id="dd0e9-217">string</span><span class="sxs-lookup"><span data-stu-id="dd0e9-217">string</span></span>  | <span data-ttu-id="dd0e9-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd0e9-220">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd0e9-220">Request body</span></span>

<span data-ttu-id="dd0e9-221">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-221">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd0e9-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0e9-222">Response</span></span>

<span data-ttu-id="dd0e9-223">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-223">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="dd0e9-224">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="dd0e9-224">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="dd0e9-225">Пример</span><span class="sxs-lookup"><span data-stu-id="dd0e9-225">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dd0e9-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd0e9-226">Request</span></span>

<span data-ttu-id="dd0e9-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-227">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd0e9-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd0e9-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="dd0e9-229">C#</span><span class="sxs-lookup"><span data-stu-id="dd0e9-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd0e9-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd0e9-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd0e9-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd0e9-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd0e9-232">Java</span><span class="sxs-lookup"><span data-stu-id="dd0e9-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd0e9-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0e9-233">Response</span></span>

<span data-ttu-id="dd0e9-234">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd0e9-234">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


