---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: cae0586eefdf9413cf38130cce7bb6e7f99ec0bd
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782590"
---
# <a name="create-subscription"></a><span data-ttu-id="6a516-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="6a516-103">Create subscription</span></span>

<span data-ttu-id="6a516-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a516-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a516-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6a516-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a516-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a516-106">Permissions</span></span>

<span data-ttu-id="6a516-107">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="6a516-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="6a516-108">Например, чтобы получать уведомления об изменениях для сообщений, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="6a516-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="6a516-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6a516-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6a516-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a516-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a516-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="6a516-111">Supported resource</span></span> | <span data-ttu-id="6a516-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a516-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a516-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a516-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a516-114">Application</span><span class="sxs-lookup"><span data-stu-id="6a516-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="6a516-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="6a516-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="6a516-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-116">Not supported</span></span> | <span data-ttu-id="6a516-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-117">Not supported</span></span> | <span data-ttu-id="6a516-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="6a516-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6a516-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6a516-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a516-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="6a516-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-121">Not supported</span></span> | <span data-ttu-id="6a516-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6a516-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="6a516-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6a516-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-124">Not supported</span></span> | <span data-ttu-id="6a516-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-125">Not supported</span></span> | <span data-ttu-id="6a516-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6a516-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6a516-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6a516-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a516-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="6a516-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-129">Not supported</span></span> | <span data-ttu-id="6a516-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="6a516-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="6a516-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6a516-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-132">Not supported</span></span> | <span data-ttu-id="6a516-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-133">Not supported</span></span> | <span data-ttu-id="6a516-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6a516-135">contact</span><span class="sxs-lookup"><span data-stu-id="6a516-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6a516-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-136">Contacts.Read</span></span> | <span data-ttu-id="6a516-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-137">Contacts.Read</span></span> | <span data-ttu-id="6a516-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-138">Contacts.Read</span></span> |
|<span data-ttu-id="6a516-139">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="6a516-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6a516-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-140">Not supported</span></span> | <span data-ttu-id="6a516-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a516-141">Files.ReadWrite</span></span> | <span data-ttu-id="6a516-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-142">Not supported</span></span> |
|<span data-ttu-id="6a516-143">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6a516-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6a516-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a516-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="6a516-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-145">Not supported</span></span> | <span data-ttu-id="6a516-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a516-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6a516-147">event</span><span class="sxs-lookup"><span data-stu-id="6a516-147">event</span></span>](../resources/event.md) | <span data-ttu-id="6a516-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-148">Calendars.Read</span></span> | <span data-ttu-id="6a516-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-149">Calendars.Read</span></span> | <span data-ttu-id="6a516-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-150">Calendars.Read</span></span> |
|[<span data-ttu-id="6a516-151">group</span><span class="sxs-lookup"><span data-stu-id="6a516-151">group</span></span>](../resources/group.md) | <span data-ttu-id="6a516-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-152">Group.Read.All</span></span> | <span data-ttu-id="6a516-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-153">Not supported</span></span> | <span data-ttu-id="6a516-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-154">Group.Read.All</span></span> |
|[<span data-ttu-id="6a516-155">group conversation</span><span class="sxs-lookup"><span data-stu-id="6a516-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6a516-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-156">Group.Read.All</span></span> | <span data-ttu-id="6a516-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-157">Not supported</span></span> | <span data-ttu-id="6a516-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-158">Not supported</span></span> |
|[<span data-ttu-id="6a516-159">list</span><span class="sxs-lookup"><span data-stu-id="6a516-159">list</span></span>](../resources/list.md) | <span data-ttu-id="6a516-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a516-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6a516-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-161">Not supported</span></span> | <span data-ttu-id="6a516-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a516-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6a516-163">message</span><span class="sxs-lookup"><span data-stu-id="6a516-163">message</span></span>](../resources/message.md) | <span data-ttu-id="6a516-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6a516-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6a516-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a516-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6a516-167">presence</span><span class="sxs-lookup"><span data-stu-id="6a516-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="6a516-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-168">Presence.Read.All</span></span> | <span data-ttu-id="6a516-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-169">Not supported</span></span> | <span data-ttu-id="6a516-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-170">Not supported</span></span> |
|[<span data-ttu-id="6a516-171">security alert</span><span class="sxs-lookup"><span data-stu-id="6a516-171">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6a516-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a516-172">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6a516-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a516-173">Not supported</span></span> | <span data-ttu-id="6a516-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a516-174">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6a516-175">user</span><span class="sxs-lookup"><span data-stu-id="6a516-175">user</span></span>](../resources/user.md) | <span data-ttu-id="6a516-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-176">User.Read.All</span></span> | <span data-ttu-id="6a516-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-177">User.Read.All</span></span> | <span data-ttu-id="6a516-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a516-178">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="6a516-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6a516-179">chatMessage</span></span>

<span data-ttu-id="6a516-180">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов ( **инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="6a516-180">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="6a516-181">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="6a516-181">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="6a516-182">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="6a516-182">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="6a516-183">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="6a516-183">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="6a516-184">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="6a516-184">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="6a516-185">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="6a516-185">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

> <span data-ttu-id="6a516-186">**Примечание:** `/chats/getAllMessages` Возвращает только сообщения из чатов, принадлежащие клиенту.</span><span class="sxs-lookup"><span data-stu-id="6a516-186">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="6a516-187">Если поток чата инициирован пользователем вне клиента, этот поток чата не принадлежит клиенту и не создает уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="6a516-187">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="6a516-188">driveItem</span><span class="sxs-lookup"><span data-stu-id="6a516-188">driveItem</span></span>

<span data-ttu-id="6a516-189">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6a516-189">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="6a516-190">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6a516-190">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6a516-191">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="6a516-191">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6a516-192">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="6a516-192">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6a516-193">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="6a516-193">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6a516-194">Нельзя подписаться на экземпляры **drive** или **driveItem** , не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="6a516-194">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6a516-195">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="6a516-195">contact, event, and message</span></span>

<span data-ttu-id="6a516-196">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="6a516-196">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6a516-197">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6a516-197">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6a516-198">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="6a516-198">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6a516-199">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a516-199">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6a516-200">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="6a516-200">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6a516-201">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6a516-201">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6a516-202">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="6a516-202">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="6a516-203">presence</span><span class="sxs-lookup"><span data-stu-id="6a516-203">presence</span></span>

<span data-ttu-id="6a516-204">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="6a516-204">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="6a516-205">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="6a516-205">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a516-206">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a516-206">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="6a516-207">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a516-207">Request headers</span></span>

| <span data-ttu-id="6a516-208">Имя</span><span class="sxs-lookup"><span data-stu-id="6a516-208">Name</span></span>       | <span data-ttu-id="6a516-209">Тип</span><span class="sxs-lookup"><span data-stu-id="6a516-209">Type</span></span> | <span data-ttu-id="6a516-210">Описание</span><span class="sxs-lookup"><span data-stu-id="6a516-210">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a516-211">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a516-211">Authorization</span></span>  | <span data-ttu-id="6a516-212">string</span><span class="sxs-lookup"><span data-stu-id="6a516-212">string</span></span>  | <span data-ttu-id="6a516-p110">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a516-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6a516-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a516-215">Response</span></span>

<span data-ttu-id="6a516-216">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a516-216">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="6a516-217">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="6a516-217">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="6a516-218">Пример</span><span class="sxs-lookup"><span data-stu-id="6a516-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a516-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a516-219">Request</span></span>

<span data-ttu-id="6a516-220">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a516-220">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="6a516-221">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="6a516-221">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="6a516-222">Этот запрос создает подписку на уведомления об изменениях новой почты, полученной в текущий момент, когда пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="6a516-222">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a516-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a516-223">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6a516-224">C#</span><span class="sxs-lookup"><span data-stu-id="6a516-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a516-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a516-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a516-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a516-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="6a516-227">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a516-227">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="6a516-228">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="6a516-228">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="6a516-229">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="6a516-229">Resources examples</span></span>

<span data-ttu-id="6a516-230">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="6a516-230">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="6a516-231">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="6a516-231">Resource type</span></span> | <span data-ttu-id="6a516-232">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a516-232">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="6a516-233">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="6a516-233">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="6a516-234">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="6a516-234">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6a516-235">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span><span class="sxs-lookup"><span data-stu-id="6a516-235">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span></span> |
|[<span data-ttu-id="6a516-236">Контакты</span><span class="sxs-lookup"><span data-stu-id="6a516-236">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="6a516-237">Беседы</span><span class="sxs-lookup"><span data-stu-id="6a516-237">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="6a516-238">Диски</span><span class="sxs-lookup"><span data-stu-id="6a516-238">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="6a516-239">События</span><span class="sxs-lookup"><span data-stu-id="6a516-239">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="6a516-240">Группы</span><span class="sxs-lookup"><span data-stu-id="6a516-240">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="6a516-241">Список</span><span class="sxs-lookup"><span data-stu-id="6a516-241">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="6a516-242">Почта</span><span class="sxs-lookup"><span data-stu-id="6a516-242">Mail</span></span>](../resources/message.md)|<span data-ttu-id="6a516-243">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="6a516-243">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="6a516-244">Знак</span><span class="sxs-lookup"><span data-stu-id="6a516-244">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="6a516-245">`/communications/presences/{id}` (один пользователь) `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="6a516-245">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="6a516-246">Пользователи</span><span class="sxs-lookup"><span data-stu-id="6a516-246">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="6a516-247">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="6a516-247">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="6a516-248">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="6a516-248">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="6a516-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a516-249">Response</span></span>

<span data-ttu-id="6a516-250">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a516-250">The following example shows the response.</span></span> 

><span data-ttu-id="6a516-p113">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a516-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="6a516-253">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="6a516-253">Notification endpoint validation</span></span>

<span data-ttu-id="6a516-254">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="6a516-254">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="6a516-255">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="6a516-255">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


