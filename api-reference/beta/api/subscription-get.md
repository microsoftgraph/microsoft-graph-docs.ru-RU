---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: a9ede7680a12864d3b5d0013fac90a4717c8e3b3
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51031018"
---
# <a name="get-subscription"></a><span data-ttu-id="01bc8-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="01bc8-103">Get subscription</span></span>

<span data-ttu-id="01bc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01bc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01bc8-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="01bc8-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="01bc8-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="01bc8-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="01bc8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01bc8-107">Permissions</span></span>

<span data-ttu-id="01bc8-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="01bc8-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="01bc8-109">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01bc8-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01bc8-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="01bc8-110">Supported resource</span></span> | <span data-ttu-id="01bc8-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01bc8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01bc8-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01bc8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01bc8-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="01bc8-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="01bc8-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="01bc8-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="01bc8-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-115">Not supported</span></span> | <span data-ttu-id="01bc8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-116">Not supported</span></span> | <span data-ttu-id="01bc8-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="01bc8-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="01bc8-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="01bc8-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="01bc8-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-120">Not supported</span></span> | <span data-ttu-id="01bc8-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="01bc8-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="01bc8-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="01bc8-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-123">Not supported</span></span> | <span data-ttu-id="01bc8-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-124">Not supported</span></span> | <span data-ttu-id="01bc8-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="01bc8-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="01bc8-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="01bc8-127">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01bc8-127">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="01bc8-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-128">Not supported</span></span> | <span data-ttu-id="01bc8-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="01bc8-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="01bc8-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="01bc8-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-131">Not supported</span></span> | <span data-ttu-id="01bc8-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-132">Not supported</span></span> | <span data-ttu-id="01bc8-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="01bc8-134">contact</span><span class="sxs-lookup"><span data-stu-id="01bc8-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="01bc8-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-135">Contacts.Read</span></span> | <span data-ttu-id="01bc8-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-136">Contacts.Read</span></span> | <span data-ttu-id="01bc8-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-137">Contacts.Read</span></span> |
|<span data-ttu-id="01bc8-138">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="01bc8-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="01bc8-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-139">Not supported</span></span> | <span data-ttu-id="01bc8-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01bc8-140">Files.ReadWrite</span></span> | <span data-ttu-id="01bc8-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-141">Not supported</span></span> |
|<span data-ttu-id="01bc8-142">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="01bc8-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="01bc8-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="01bc8-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-144">Not supported</span></span> | <span data-ttu-id="01bc8-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="01bc8-146">event</span><span class="sxs-lookup"><span data-stu-id="01bc8-146">event</span></span>](../resources/event.md) | <span data-ttu-id="01bc8-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-147">Calendars.Read</span></span> | <span data-ttu-id="01bc8-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-148">Calendars.Read</span></span> | <span data-ttu-id="01bc8-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-149">Calendars.Read</span></span> |
|[<span data-ttu-id="01bc8-150">group</span><span class="sxs-lookup"><span data-stu-id="01bc8-150">group</span></span>](../resources/group.md) | <span data-ttu-id="01bc8-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-151">Group.Read.All</span></span> | <span data-ttu-id="01bc8-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-152">Not supported</span></span> | <span data-ttu-id="01bc8-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-153">Group.Read.All</span></span> |
|[<span data-ttu-id="01bc8-154">group conversation</span><span class="sxs-lookup"><span data-stu-id="01bc8-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="01bc8-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-155">Group.Read.All</span></span> | <span data-ttu-id="01bc8-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-156">Not supported</span></span> | <span data-ttu-id="01bc8-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-157">Not supported</span></span> |
|[<span data-ttu-id="01bc8-158">list</span><span class="sxs-lookup"><span data-stu-id="01bc8-158">list</span></span>](../resources/list.md) | <span data-ttu-id="01bc8-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="01bc8-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-160">Not supported</span></span> | <span data-ttu-id="01bc8-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="01bc8-162">message</span><span class="sxs-lookup"><span data-stu-id="01bc8-162">message</span></span>](../resources/message.md) | <span data-ttu-id="01bc8-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="01bc8-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="01bc8-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01bc8-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="01bc8-166">presence</span><span class="sxs-lookup"><span data-stu-id="01bc8-166">presence</span></span>](../resources/presence.md) | <span data-ttu-id="01bc8-167">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-167">Presence.Read.All</span></span> | <span data-ttu-id="01bc8-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-168">Not supported</span></span> | <span data-ttu-id="01bc8-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-169">Not supported</span></span> |
|[<span data-ttu-id="01bc8-170">printer</span><span class="sxs-lookup"><span data-stu-id="01bc8-170">printer</span></span>](../resources/printer.md) | <span data-ttu-id="01bc8-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-171">Not supported</span></span> | <span data-ttu-id="01bc8-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-172">Not supported</span></span> | <span data-ttu-id="01bc8-173">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-173">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="01bc8-174">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="01bc8-174">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="01bc8-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-175">Not supported</span></span> | <span data-ttu-id="01bc8-176">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-176">Not supported</span></span> | <span data-ttu-id="01bc8-177">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-177">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="01bc8-178">security alert</span><span class="sxs-lookup"><span data-stu-id="01bc8-178">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="01bc8-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-179">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="01bc8-180">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-180">Not supported</span></span> | <span data-ttu-id="01bc8-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-181">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="01bc8-182">todoTask</span><span class="sxs-lookup"><span data-stu-id="01bc8-182">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="01bc8-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01bc8-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="01bc8-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01bc8-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="01bc8-185">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01bc8-185">Not supported</span></span> |
|[<span data-ttu-id="01bc8-186">user</span><span class="sxs-lookup"><span data-stu-id="01bc8-186">user</span></span>](../resources/user.md) | <span data-ttu-id="01bc8-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-187">User.Read.All</span></span> | <span data-ttu-id="01bc8-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-188">User.Read.All</span></span> | <span data-ttu-id="01bc8-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="01bc8-189">User.Read.All</span></span> |

> <span data-ttu-id="01bc8-190">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="01bc8-190">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="01bc8-191">driveItem</span><span class="sxs-lookup"><span data-stu-id="01bc8-191">driveItem</span></span>

<span data-ttu-id="01bc8-192">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="01bc8-192">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="01bc8-193">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="01bc8-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="01bc8-194">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="01bc8-194">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="01bc8-195">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="01bc8-195">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="01bc8-196">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="01bc8-196">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="01bc8-197">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="01bc8-197">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="01bc8-198">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="01bc8-198">contact, event, and message</span></span>

<span data-ttu-id="01bc8-199">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="01bc8-199">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="01bc8-200">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="01bc8-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="01bc8-201">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="01bc8-201">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="01bc8-202">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="01bc8-202">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="01bc8-203">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="01bc8-203">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="01bc8-204">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="01bc8-204">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="01bc8-205">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="01bc8-205">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="01bc8-206">presence</span><span class="sxs-lookup"><span data-stu-id="01bc8-206">presence</span></span>

<span data-ttu-id="01bc8-207">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="01bc8-207">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="01bc8-208">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="01bc8-208">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="01bc8-209">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01bc8-209">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01bc8-210">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01bc8-210">Optional query parameters</span></span>

<span data-ttu-id="01bc8-211">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01bc8-211">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01bc8-212">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01bc8-212">Request headers</span></span>

| <span data-ttu-id="01bc8-213">Имя</span><span class="sxs-lookup"><span data-stu-id="01bc8-213">Name</span></span>       | <span data-ttu-id="01bc8-214">Тип</span><span class="sxs-lookup"><span data-stu-id="01bc8-214">Type</span></span> | <span data-ttu-id="01bc8-215">Описание</span><span class="sxs-lookup"><span data-stu-id="01bc8-215">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="01bc8-216">Authorization</span><span class="sxs-lookup"><span data-stu-id="01bc8-216">Authorization</span></span>  | <span data-ttu-id="01bc8-217">string</span><span class="sxs-lookup"><span data-stu-id="01bc8-217">string</span></span>  | <span data-ttu-id="01bc8-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01bc8-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01bc8-220">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01bc8-220">Request body</span></span>

<span data-ttu-id="01bc8-221">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01bc8-221">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01bc8-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="01bc8-222">Response</span></span>

<span data-ttu-id="01bc8-223">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01bc8-223">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01bc8-224">Пример</span><span class="sxs-lookup"><span data-stu-id="01bc8-224">Example</span></span>

##### <a name="request"></a><span data-ttu-id="01bc8-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="01bc8-225">Request</span></span>

<span data-ttu-id="01bc8-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01bc8-226">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01bc8-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="01bc8-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="01bc8-228">C#</span><span class="sxs-lookup"><span data-stu-id="01bc8-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01bc8-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01bc8-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01bc8-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01bc8-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01bc8-231">Java</span><span class="sxs-lookup"><span data-stu-id="01bc8-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="01bc8-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="01bc8-232">Response</span></span>

<span data-ttu-id="01bc8-233">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01bc8-233">Here is an example of the response.</span></span>
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
  "includeResourceData": false,
  "notificationContentType": "application/json"
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


