---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 43ae2e82c1a9a0af7660151af1bf07062bbef2ec
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000688"
---
# <a name="create-subscription"></a><span data-ttu-id="1324d-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="1324d-103">Create subscription</span></span>

<span data-ttu-id="1324d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1324d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1324d-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1324d-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="1324d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1324d-106">Permissions</span></span>

<span data-ttu-id="1324d-107">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="1324d-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="1324d-108">Например, чтобы получать уведомления об изменениях для сообщений, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="1324d-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="1324d-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1324d-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="1324d-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1324d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1324d-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="1324d-111">Supported resource</span></span> | <span data-ttu-id="1324d-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1324d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1324d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1324d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1324d-114">Application</span><span class="sxs-lookup"><span data-stu-id="1324d-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="1324d-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="1324d-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="1324d-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-116">Not supported</span></span> | <span data-ttu-id="1324d-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-117">Not supported</span></span> | <span data-ttu-id="1324d-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="1324d-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="1324d-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="1324d-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1324d-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="1324d-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-121">Not supported</span></span> | <span data-ttu-id="1324d-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="1324d-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="1324d-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="1324d-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-124">Not supported</span></span> | <span data-ttu-id="1324d-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-125">Not supported</span></span> | <span data-ttu-id="1324d-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="1324d-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="1324d-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="1324d-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1324d-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="1324d-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-129">Not supported</span></span> | <span data-ttu-id="1324d-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="1324d-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="1324d-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="1324d-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-132">Not supported</span></span> | <span data-ttu-id="1324d-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-133">Not supported</span></span> | <span data-ttu-id="1324d-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="1324d-135">contact</span><span class="sxs-lookup"><span data-stu-id="1324d-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="1324d-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-136">Contacts.Read</span></span> | <span data-ttu-id="1324d-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-137">Contacts.Read</span></span> | <span data-ttu-id="1324d-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-138">Contacts.Read</span></span> |
|<span data-ttu-id="1324d-139">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="1324d-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="1324d-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-140">Not supported</span></span> | <span data-ttu-id="1324d-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1324d-141">Files.ReadWrite</span></span> | <span data-ttu-id="1324d-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-142">Not supported</span></span> |
|<span data-ttu-id="1324d-143">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="1324d-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="1324d-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1324d-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="1324d-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-145">Not supported</span></span> | <span data-ttu-id="1324d-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1324d-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="1324d-147">event</span><span class="sxs-lookup"><span data-stu-id="1324d-147">event</span></span>](../resources/event.md) | <span data-ttu-id="1324d-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-148">Calendars.Read</span></span> | <span data-ttu-id="1324d-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-149">Calendars.Read</span></span> | <span data-ttu-id="1324d-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-150">Calendars.Read</span></span> |
|[<span data-ttu-id="1324d-151">group</span><span class="sxs-lookup"><span data-stu-id="1324d-151">group</span></span>](../resources/group.md) | <span data-ttu-id="1324d-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-152">Group.Read.All</span></span> | <span data-ttu-id="1324d-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-153">Not supported</span></span> | <span data-ttu-id="1324d-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-154">Group.Read.All</span></span> |
|[<span data-ttu-id="1324d-155">group conversation</span><span class="sxs-lookup"><span data-stu-id="1324d-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="1324d-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-156">Group.Read.All</span></span> | <span data-ttu-id="1324d-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-157">Not supported</span></span> | <span data-ttu-id="1324d-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-158">Not supported</span></span> |
|[<span data-ttu-id="1324d-159">list</span><span class="sxs-lookup"><span data-stu-id="1324d-159">list</span></span>](../resources/list.md) | <span data-ttu-id="1324d-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1324d-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="1324d-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-161">Not supported</span></span> | <span data-ttu-id="1324d-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1324d-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="1324d-163">message</span><span class="sxs-lookup"><span data-stu-id="1324d-163">message</span></span>](../resources/message.md) | <span data-ttu-id="1324d-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1324d-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1324d-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1324d-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="1324d-167">presence</span><span class="sxs-lookup"><span data-stu-id="1324d-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="1324d-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-168">Presence.Read.All</span></span> | <span data-ttu-id="1324d-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-169">Not supported</span></span> | <span data-ttu-id="1324d-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-170">Not supported</span></span> |
|[<span data-ttu-id="1324d-171">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="1324d-171">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="1324d-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-172">Not supported</span></span> | <span data-ttu-id="1324d-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-173">Not supported</span></span> | <span data-ttu-id="1324d-174">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1324d-174">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="1324d-175">security alert</span><span class="sxs-lookup"><span data-stu-id="1324d-175">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="1324d-176">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1324d-176">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="1324d-177">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1324d-177">Not supported</span></span> | <span data-ttu-id="1324d-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1324d-178">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="1324d-179">user</span><span class="sxs-lookup"><span data-stu-id="1324d-179">user</span></span>](../resources/user.md) | <span data-ttu-id="1324d-180">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-180">User.Read.All</span></span> | <span data-ttu-id="1324d-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-181">User.Read.All</span></span> | <span data-ttu-id="1324d-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1324d-182">User.Read.All</span></span> |

> <span data-ttu-id="1324d-183">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1324d-183">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="1324d-184">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1324d-184">chatMessage</span></span>

<span data-ttu-id="1324d-185">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов ( **инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="1324d-185">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="1324d-186">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="1324d-186">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="1324d-187">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="1324d-187">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="1324d-188">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="1324d-188">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="1324d-189">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="1324d-189">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="1324d-190">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="1324d-190">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

> <span data-ttu-id="1324d-191">**Примечание.** `/chats/getAllMessages` возвращает только сообщения из чатов, принадлежащих клиенту.</span><span class="sxs-lookup"><span data-stu-id="1324d-191">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="1324d-192">Если цепочка чата инициирована пользователем из-за пределов клиента, она не принадлежит клиенту и для нее не создаются уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1324d-192">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="1324d-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="1324d-193">driveItem</span></span>

<span data-ttu-id="1324d-194">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1324d-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="1324d-195">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="1324d-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="1324d-196">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="1324d-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="1324d-197">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="1324d-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="1324d-198">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="1324d-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="1324d-199">Нельзя подписаться на экземпляры **drive** или **driveItem** , не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="1324d-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="1324d-200">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="1324d-200">contact, event, and message</span></span>

<span data-ttu-id="1324d-201">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="1324d-201">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="1324d-202">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="1324d-202">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="1324d-203">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="1324d-203">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="1324d-204">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1324d-204">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="1324d-205">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="1324d-205">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="1324d-206">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1324d-206">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="1324d-207">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="1324d-207">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="1324d-208">presence</span><span class="sxs-lookup"><span data-stu-id="1324d-208">presence</span></span>

<span data-ttu-id="1324d-209">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="1324d-209">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="1324d-210">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="1324d-210">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="1324d-211">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1324d-211">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="1324d-212">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1324d-212">Request headers</span></span>

| <span data-ttu-id="1324d-213">Имя</span><span class="sxs-lookup"><span data-stu-id="1324d-213">Name</span></span>       | <span data-ttu-id="1324d-214">Тип</span><span class="sxs-lookup"><span data-stu-id="1324d-214">Type</span></span> | <span data-ttu-id="1324d-215">Описание</span><span class="sxs-lookup"><span data-stu-id="1324d-215">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1324d-216">Authorization</span><span class="sxs-lookup"><span data-stu-id="1324d-216">Authorization</span></span>  | <span data-ttu-id="1324d-217">string</span><span class="sxs-lookup"><span data-stu-id="1324d-217">string</span></span>  | <span data-ttu-id="1324d-p110">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1324d-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1324d-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="1324d-220">Response</span></span>

<span data-ttu-id="1324d-221">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1324d-221">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="1324d-222">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="1324d-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="1324d-223">Пример</span><span class="sxs-lookup"><span data-stu-id="1324d-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="1324d-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="1324d-224">Request</span></span>

<span data-ttu-id="1324d-225">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1324d-225">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="1324d-226">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="1324d-226">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="1324d-227">Этот запрос создает подписку на уведомления об изменениях новой почты, полученной в текущий момент, когда пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="1324d-227">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="1324d-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="1324d-228">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1324d-229">C#</span><span class="sxs-lookup"><span data-stu-id="1324d-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1324d-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1324d-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1324d-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1324d-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1324d-232">Java</span><span class="sxs-lookup"><span data-stu-id="1324d-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1324d-233">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1324d-233">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="1324d-234">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="1324d-234">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="1324d-235">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="1324d-235">Resources examples</span></span>

<span data-ttu-id="1324d-236">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="1324d-236">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="1324d-237">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="1324d-237">Resource type</span></span> | <span data-ttu-id="1324d-238">Примеры</span><span class="sxs-lookup"><span data-stu-id="1324d-238">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="1324d-239">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="1324d-239">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="1324d-240">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="1324d-240">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="1324d-241">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="1324d-241">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="1324d-242">Контакты</span><span class="sxs-lookup"><span data-stu-id="1324d-242">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="1324d-243">Беседы</span><span class="sxs-lookup"><span data-stu-id="1324d-243">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="1324d-244">Диски</span><span class="sxs-lookup"><span data-stu-id="1324d-244">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="1324d-245">События</span><span class="sxs-lookup"><span data-stu-id="1324d-245">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="1324d-246">Группы</span><span class="sxs-lookup"><span data-stu-id="1324d-246">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="1324d-247">Список</span><span class="sxs-lookup"><span data-stu-id="1324d-247">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="1324d-248">Почта</span><span class="sxs-lookup"><span data-stu-id="1324d-248">Mail</span></span>](../resources/message.md)|<span data-ttu-id="1324d-249">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="1324d-249">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="1324d-250">Знак</span><span class="sxs-lookup"><span data-stu-id="1324d-250">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="1324d-251">`/communications/presences/{id}` (один пользователь) `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="1324d-251">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="1324d-252">принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="1324d-252">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="1324d-253">Пользователи</span><span class="sxs-lookup"><span data-stu-id="1324d-253">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="1324d-254">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="1324d-254">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="1324d-255">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="1324d-255">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="1324d-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="1324d-256">Response</span></span>

<span data-ttu-id="1324d-257">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1324d-257">The following example shows the response.</span></span> 

><span data-ttu-id="1324d-p113">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1324d-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="1324d-260">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="1324d-260">Notification endpoint validation</span></span>

<span data-ttu-id="1324d-261">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="1324d-261">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="1324d-262">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="1324d-262">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


