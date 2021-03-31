---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: fe4c987c86aaf9c63b7133e323b2d1ed6977da99
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469481"
---
# <a name="delete-subscription"></a><span data-ttu-id="04b64-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="04b64-103">Delete subscription</span></span>

<span data-ttu-id="04b64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04b64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04b64-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="04b64-105">Delete a subscription.</span></span>

<span data-ttu-id="04b64-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="04b64-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="04b64-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04b64-107">Permissions</span></span>

<span data-ttu-id="04b64-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="04b64-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="04b64-109">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b64-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04b64-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="04b64-110">Supported resource</span></span> | <span data-ttu-id="04b64-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b64-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04b64-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04b64-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="04b64-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="04b64-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="04b64-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="04b64-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-115">Not supported</span></span> | <span data-ttu-id="04b64-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-116">Not supported</span></span> | <span data-ttu-id="04b64-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="04b64-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="04b64-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="04b64-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="04b64-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-120">Not supported</span></span> | <span data-ttu-id="04b64-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="04b64-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="04b64-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="04b64-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-123">Not supported</span></span> | <span data-ttu-id="04b64-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-124">Not supported</span></span> | <span data-ttu-id="04b64-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="04b64-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="04b64-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="04b64-127">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04b64-127">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="04b64-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-128">Not supported</span></span> | <span data-ttu-id="04b64-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="04b64-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="04b64-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="04b64-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-131">Not supported</span></span> | <span data-ttu-id="04b64-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-132">Not supported</span></span> | <span data-ttu-id="04b64-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="04b64-134">contact</span><span class="sxs-lookup"><span data-stu-id="04b64-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="04b64-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-135">Contacts.Read</span></span> | <span data-ttu-id="04b64-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-136">Contacts.Read</span></span> | <span data-ttu-id="04b64-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-137">Contacts.Read</span></span> |
|<span data-ttu-id="04b64-138">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="04b64-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="04b64-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-139">Not supported</span></span> | <span data-ttu-id="04b64-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04b64-140">Files.ReadWrite</span></span> | <span data-ttu-id="04b64-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-141">Not supported</span></span> |
|<span data-ttu-id="04b64-142">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="04b64-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="04b64-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="04b64-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-144">Not supported</span></span> | <span data-ttu-id="04b64-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="04b64-146">event</span><span class="sxs-lookup"><span data-stu-id="04b64-146">event</span></span>](../resources/event.md) | <span data-ttu-id="04b64-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-147">Calendars.Read</span></span> | <span data-ttu-id="04b64-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-148">Calendars.Read</span></span> | <span data-ttu-id="04b64-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-149">Calendars.Read</span></span> |
|[<span data-ttu-id="04b64-150">group</span><span class="sxs-lookup"><span data-stu-id="04b64-150">group</span></span>](../resources/group.md) | <span data-ttu-id="04b64-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-151">Group.Read.All</span></span> | <span data-ttu-id="04b64-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-152">Not supported</span></span> | <span data-ttu-id="04b64-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-153">Group.Read.All</span></span> |
|[<span data-ttu-id="04b64-154">group conversation</span><span class="sxs-lookup"><span data-stu-id="04b64-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="04b64-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-155">Group.Read.All</span></span> | <span data-ttu-id="04b64-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-156">Not supported</span></span> | <span data-ttu-id="04b64-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-157">Not supported</span></span> |
|[<span data-ttu-id="04b64-158">list</span><span class="sxs-lookup"><span data-stu-id="04b64-158">list</span></span>](../resources/list.md) | <span data-ttu-id="04b64-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="04b64-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-160">Not supported</span></span> | <span data-ttu-id="04b64-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="04b64-162">message</span><span class="sxs-lookup"><span data-stu-id="04b64-162">message</span></span>](../resources/message.md) | <span data-ttu-id="04b64-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="04b64-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="04b64-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="04b64-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="04b64-166">presence</span><span class="sxs-lookup"><span data-stu-id="04b64-166">presence</span></span>](../resources/presence.md) | <span data-ttu-id="04b64-167">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-167">Presence.Read.All</span></span> | <span data-ttu-id="04b64-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-168">Not supported</span></span> | <span data-ttu-id="04b64-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-169">Not supported</span></span> |
|[<span data-ttu-id="04b64-170">printer</span><span class="sxs-lookup"><span data-stu-id="04b64-170">printer</span></span>](../resources/printer.md) | <span data-ttu-id="04b64-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-171">Not supported</span></span> | <span data-ttu-id="04b64-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-172">Not supported</span></span> | <span data-ttu-id="04b64-173">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-173">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="04b64-174">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="04b64-174">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="04b64-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-175">Not supported</span></span> | <span data-ttu-id="04b64-176">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-176">Not supported</span></span> | <span data-ttu-id="04b64-177">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-177">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="04b64-178">security alert</span><span class="sxs-lookup"><span data-stu-id="04b64-178">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="04b64-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-179">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="04b64-180">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-180">Not supported</span></span> | <span data-ttu-id="04b64-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b64-181">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="04b64-182">todoTask</span><span class="sxs-lookup"><span data-stu-id="04b64-182">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="04b64-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04b64-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="04b64-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04b64-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="04b64-185">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04b64-185">Not supported</span></span> |
|[<span data-ttu-id="04b64-186">user</span><span class="sxs-lookup"><span data-stu-id="04b64-186">user</span></span>](../resources/user.md) | <span data-ttu-id="04b64-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-187">User.Read.All</span></span> | <span data-ttu-id="04b64-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-188">User.Read.All</span></span> | <span data-ttu-id="04b64-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="04b64-189">User.Read.All</span></span> |

> <span data-ttu-id="04b64-190">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="04b64-190">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="04b64-191">driveItem</span><span class="sxs-lookup"><span data-stu-id="04b64-191">driveItem</span></span>

<span data-ttu-id="04b64-192">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="04b64-192">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="04b64-193">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="04b64-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="04b64-194">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="04b64-194">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="04b64-195">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="04b64-195">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="04b64-196">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="04b64-196">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="04b64-197">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="04b64-197">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="04b64-198">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="04b64-198">contact, event, and message</span></span>

<span data-ttu-id="04b64-199">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="04b64-199">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="04b64-200">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="04b64-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="04b64-201">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="04b64-201">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="04b64-202">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="04b64-202">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="04b64-203">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="04b64-203">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="04b64-204">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="04b64-204">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="04b64-205">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="04b64-205">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="04b64-206">presence</span><span class="sxs-lookup"><span data-stu-id="04b64-206">presence</span></span>

<span data-ttu-id="04b64-207">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="04b64-207">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="04b64-208">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="04b64-208">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="04b64-209">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b64-209">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="04b64-210">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04b64-210">Request headers</span></span>

| <span data-ttu-id="04b64-211">Имя</span><span class="sxs-lookup"><span data-stu-id="04b64-211">Name</span></span>       | <span data-ttu-id="04b64-212">Тип</span><span class="sxs-lookup"><span data-stu-id="04b64-212">Type</span></span> | <span data-ttu-id="04b64-213">Описание</span><span class="sxs-lookup"><span data-stu-id="04b64-213">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04b64-214">Authorization</span><span class="sxs-lookup"><span data-stu-id="04b64-214">Authorization</span></span>  | <span data-ttu-id="04b64-215">string</span><span class="sxs-lookup"><span data-stu-id="04b64-215">string</span></span>  | <span data-ttu-id="04b64-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b64-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04b64-218">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04b64-218">Request body</span></span>

<span data-ttu-id="04b64-219">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04b64-219">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04b64-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b64-220">Response</span></span>

<span data-ttu-id="04b64-221">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04b64-221">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="04b64-222">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="04b64-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="04b64-223">Пример</span><span class="sxs-lookup"><span data-stu-id="04b64-223">Example</span></span>

##### <a name="request"></a><span data-ttu-id="04b64-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b64-224">Request</span></span>

<span data-ttu-id="04b64-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04b64-225">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04b64-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="04b64-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="04b64-227">C#</span><span class="sxs-lookup"><span data-stu-id="04b64-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04b64-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04b64-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04b64-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04b64-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04b64-230">Java</span><span class="sxs-lookup"><span data-stu-id="04b64-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04b64-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b64-231">Response</span></span>

<span data-ttu-id="04b64-232">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04b64-232">Here is an example of the response.</span></span>
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


