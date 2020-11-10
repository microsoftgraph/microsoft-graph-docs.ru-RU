---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 07d98cb570b13d3e28b44979e92b34f6c8e8724e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972060"
---
# <a name="get-subscription"></a><span data-ttu-id="cdd6b-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="cdd6b-103">Get subscription</span></span>

<span data-ttu-id="cdd6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdd6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdd6b-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdd6b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdd6b-106">Permissions</span></span>

<span data-ttu-id="cdd6b-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="cdd6b-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdd6b-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="cdd6b-109">Supported resource</span></span> | <span data-ttu-id="cdd6b-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdd6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cdd6b-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdd6b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdd6b-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="cdd6b-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="cdd6b-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="cdd6b-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="cdd6b-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-114">Not supported</span></span> | <span data-ttu-id="cdd6b-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-115">Not supported</span></span> | <span data-ttu-id="cdd6b-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="cdd6b-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="cdd6b-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="cdd6b-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="cdd6b-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-119">Not supported</span></span> | <span data-ttu-id="cdd6b-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="cdd6b-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="cdd6b-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="cdd6b-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-122">Not supported</span></span> | <span data-ttu-id="cdd6b-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-123">Not supported</span></span> | <span data-ttu-id="cdd6b-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="cdd6b-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="cdd6b-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="cdd6b-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdd6b-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="cdd6b-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-127">Not supported</span></span> | <span data-ttu-id="cdd6b-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="cdd6b-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="cdd6b-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="cdd6b-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-130">Not supported</span></span> | <span data-ttu-id="cdd6b-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-131">Not supported</span></span> | <span data-ttu-id="cdd6b-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="cdd6b-133">contact</span><span class="sxs-lookup"><span data-stu-id="cdd6b-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="cdd6b-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-134">Contacts.Read</span></span> | <span data-ttu-id="cdd6b-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-135">Contacts.Read</span></span> | <span data-ttu-id="cdd6b-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-136">Contacts.Read</span></span> |
|<span data-ttu-id="cdd6b-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="cdd6b-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="cdd6b-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-138">Not supported</span></span> | <span data-ttu-id="cdd6b-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdd6b-139">Files.ReadWrite</span></span> | <span data-ttu-id="cdd6b-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-140">Not supported</span></span> |
|<span data-ttu-id="cdd6b-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="cdd6b-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="cdd6b-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="cdd6b-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-143">Not supported</span></span> | <span data-ttu-id="cdd6b-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="cdd6b-145">event</span><span class="sxs-lookup"><span data-stu-id="cdd6b-145">event</span></span>](../resources/event.md) | <span data-ttu-id="cdd6b-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-146">Calendars.Read</span></span> | <span data-ttu-id="cdd6b-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-147">Calendars.Read</span></span> | <span data-ttu-id="cdd6b-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-148">Calendars.Read</span></span> |
|[<span data-ttu-id="cdd6b-149">group</span><span class="sxs-lookup"><span data-stu-id="cdd6b-149">group</span></span>](../resources/group.md) | <span data-ttu-id="cdd6b-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-150">Group.Read.All</span></span> | <span data-ttu-id="cdd6b-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-151">Not supported</span></span> | <span data-ttu-id="cdd6b-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-152">Group.Read.All</span></span> |
|[<span data-ttu-id="cdd6b-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="cdd6b-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="cdd6b-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-154">Group.Read.All</span></span> | <span data-ttu-id="cdd6b-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-155">Not supported</span></span> | <span data-ttu-id="cdd6b-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-156">Not supported</span></span> |
|[<span data-ttu-id="cdd6b-157">list</span><span class="sxs-lookup"><span data-stu-id="cdd6b-157">list</span></span>](../resources/list.md) | <span data-ttu-id="cdd6b-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="cdd6b-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-159">Not supported</span></span> | <span data-ttu-id="cdd6b-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="cdd6b-161">message</span><span class="sxs-lookup"><span data-stu-id="cdd6b-161">message</span></span>](../resources/message.md) | <span data-ttu-id="cdd6b-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="cdd6b-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="cdd6b-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cdd6b-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="cdd6b-165">presence</span><span class="sxs-lookup"><span data-stu-id="cdd6b-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="cdd6b-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-166">Presence.Read.All</span></span> | <span data-ttu-id="cdd6b-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-167">Not supported</span></span> | <span data-ttu-id="cdd6b-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-168">Not supported</span></span> |
|[<span data-ttu-id="cdd6b-169">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="cdd6b-169">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="cdd6b-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-170">Not supported</span></span> | <span data-ttu-id="cdd6b-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-171">Not supported</span></span> | <span data-ttu-id="cdd6b-172">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-172">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="cdd6b-173">security alert</span><span class="sxs-lookup"><span data-stu-id="cdd6b-173">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="cdd6b-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-174">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="cdd6b-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cdd6b-175">Not supported</span></span> | <span data-ttu-id="cdd6b-176">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-176">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="cdd6b-177">user</span><span class="sxs-lookup"><span data-stu-id="cdd6b-177">user</span></span>](../resources/user.md) | <span data-ttu-id="cdd6b-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-178">User.Read.All</span></span> | <span data-ttu-id="cdd6b-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-179">User.Read.All</span></span> | <span data-ttu-id="cdd6b-180">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdd6b-180">User.Read.All</span></span> |

> <span data-ttu-id="cdd6b-181">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-181">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="cdd6b-182">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cdd6b-182">chatMessage</span></span>

<span data-ttu-id="cdd6b-183">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов ( **инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-183">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="cdd6b-184">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-184">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="cdd6b-185">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-185">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="cdd6b-186">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-186">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="cdd6b-187">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-187">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="cdd6b-188">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-188">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="cdd6b-189">driveItem</span><span class="sxs-lookup"><span data-stu-id="cdd6b-189">driveItem</span></span>

<span data-ttu-id="cdd6b-190">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-190">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="cdd6b-191">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-191">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="cdd6b-192">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-192">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="cdd6b-193">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-193">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="cdd6b-194">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-194">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="cdd6b-195">Нельзя подписаться на экземпляры **drive** или **driveItem** , не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-195">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="cdd6b-196">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="cdd6b-196">contact, event, and message</span></span>

<span data-ttu-id="cdd6b-197">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-197">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="cdd6b-198">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-198">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="cdd6b-199">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-199">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="cdd6b-200">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-200">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="cdd6b-201">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="cdd6b-201">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="cdd6b-202">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-202">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="cdd6b-203">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-203">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="cdd6b-204">presence</span><span class="sxs-lookup"><span data-stu-id="cdd6b-204">presence</span></span>

<span data-ttu-id="cdd6b-205">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-205">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="cdd6b-206">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="cdd6b-206">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="cdd6b-207">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdd6b-207">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdd6b-208">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cdd6b-208">Optional query parameters</span></span>

<span data-ttu-id="cdd6b-209">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-209">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdd6b-210">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdd6b-210">Request headers</span></span>

| <span data-ttu-id="cdd6b-211">Имя</span><span class="sxs-lookup"><span data-stu-id="cdd6b-211">Name</span></span>       | <span data-ttu-id="cdd6b-212">Тип</span><span class="sxs-lookup"><span data-stu-id="cdd6b-212">Type</span></span> | <span data-ttu-id="cdd6b-213">Описание</span><span class="sxs-lookup"><span data-stu-id="cdd6b-213">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="cdd6b-214">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdd6b-214">Authorization</span></span>  | <span data-ttu-id="cdd6b-215">string</span><span class="sxs-lookup"><span data-stu-id="cdd6b-215">string</span></span>  | <span data-ttu-id="cdd6b-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdd6b-218">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdd6b-218">Request body</span></span>

<span data-ttu-id="cdd6b-219">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-219">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdd6b-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdd6b-220">Response</span></span>

<span data-ttu-id="cdd6b-221">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-221">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdd6b-222">Пример</span><span class="sxs-lookup"><span data-stu-id="cdd6b-222">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cdd6b-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdd6b-223">Request</span></span>

<span data-ttu-id="cdd6b-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-224">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdd6b-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd6b-225">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="cdd6b-226">C#</span><span class="sxs-lookup"><span data-stu-id="cdd6b-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdd6b-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdd6b-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdd6b-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdd6b-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdd6b-229">Java</span><span class="sxs-lookup"><span data-stu-id="cdd6b-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cdd6b-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdd6b-230">Response</span></span>

<span data-ttu-id="cdd6b-231">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cdd6b-231">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


