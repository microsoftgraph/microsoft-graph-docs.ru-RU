---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 855c0463c75bd57e49b2de990a8de69965c34b48
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034270"
---
# <a name="update-subscription"></a><span data-ttu-id="294e7-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="294e7-103">Update subscription</span></span>

<span data-ttu-id="294e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="294e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="294e7-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="294e7-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="294e7-106">Срок действия подписок истекает через некоторое время, которое зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="294e7-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="294e7-107">Чтобы избежать отсутствующих уведомлений об изменениях, приложение должно продлевать подписки ранее до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="294e7-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="294e7-108">Максимальная [длина](../resources/subscription.md) подписки для каждого типа ресурса см. в подписке.</span><span class="sxs-lookup"><span data-stu-id="294e7-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="294e7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="294e7-109">Permissions</span></span>

<span data-ttu-id="294e7-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="294e7-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="294e7-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="294e7-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="294e7-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="294e7-112">Supported resource</span></span> | <span data-ttu-id="294e7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="294e7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="294e7-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="294e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="294e7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="294e7-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="294e7-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="294e7-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="294e7-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-117">Not supported</span></span> | <span data-ttu-id="294e7-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-118">Not supported</span></span> | <span data-ttu-id="294e7-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="294e7-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="294e7-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="294e7-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="294e7-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-122">Not supported</span></span> | <span data-ttu-id="294e7-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="294e7-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="294e7-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="294e7-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-125">Not supported</span></span> | <span data-ttu-id="294e7-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-126">Not supported</span></span> | <span data-ttu-id="294e7-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="294e7-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="294e7-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="294e7-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="294e7-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="294e7-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-130">Not supported</span></span> | <span data-ttu-id="294e7-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="294e7-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="294e7-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="294e7-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-133">Not supported</span></span> | <span data-ttu-id="294e7-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-134">Not supported</span></span> | <span data-ttu-id="294e7-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="294e7-136">contact</span><span class="sxs-lookup"><span data-stu-id="294e7-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="294e7-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-137">Contacts.Read</span></span> | <span data-ttu-id="294e7-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-138">Contacts.Read</span></span> | <span data-ttu-id="294e7-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-139">Contacts.Read</span></span> |
|<span data-ttu-id="294e7-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="294e7-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="294e7-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-141">Not supported</span></span> | <span data-ttu-id="294e7-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="294e7-142">Files.ReadWrite</span></span> | <span data-ttu-id="294e7-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-143">Not supported</span></span> |
|<span data-ttu-id="294e7-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="294e7-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="294e7-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="294e7-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-146">Not supported</span></span> | <span data-ttu-id="294e7-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="294e7-148">event</span><span class="sxs-lookup"><span data-stu-id="294e7-148">event</span></span>](../resources/event.md) | <span data-ttu-id="294e7-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-149">Calendars.Read</span></span> | <span data-ttu-id="294e7-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-150">Calendars.Read</span></span> | <span data-ttu-id="294e7-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-151">Calendars.Read</span></span> |
|[<span data-ttu-id="294e7-152">group</span><span class="sxs-lookup"><span data-stu-id="294e7-152">group</span></span>](../resources/group.md) | <span data-ttu-id="294e7-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-153">Group.Read.All</span></span> | <span data-ttu-id="294e7-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-154">Not supported</span></span> | <span data-ttu-id="294e7-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-155">Group.Read.All</span></span> |
|[<span data-ttu-id="294e7-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="294e7-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="294e7-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-157">Group.Read.All</span></span> | <span data-ttu-id="294e7-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-158">Not supported</span></span> | <span data-ttu-id="294e7-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-159">Not supported</span></span> |
|[<span data-ttu-id="294e7-160">list</span><span class="sxs-lookup"><span data-stu-id="294e7-160">list</span></span>](../resources/list.md) | <span data-ttu-id="294e7-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="294e7-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-162">Not supported</span></span> | <span data-ttu-id="294e7-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="294e7-164">message</span><span class="sxs-lookup"><span data-stu-id="294e7-164">message</span></span>](../resources/message.md) | <span data-ttu-id="294e7-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="294e7-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="294e7-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="294e7-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="294e7-168">presence</span><span class="sxs-lookup"><span data-stu-id="294e7-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="294e7-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-169">Presence.Read.All</span></span> | <span data-ttu-id="294e7-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-170">Not supported</span></span> | <span data-ttu-id="294e7-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-171">Not supported</span></span> |
|[<span data-ttu-id="294e7-172">printer</span><span class="sxs-lookup"><span data-stu-id="294e7-172">printer</span></span>](../resources/printer.md) | <span data-ttu-id="294e7-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-173">Not supported</span></span> | <span data-ttu-id="294e7-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-174">Not supported</span></span> | <span data-ttu-id="294e7-175">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-175">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="294e7-176">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="294e7-176">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="294e7-177">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-177">Not supported</span></span> | <span data-ttu-id="294e7-178">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-178">Not supported</span></span> | <span data-ttu-id="294e7-179">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-179">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="294e7-180">security alert</span><span class="sxs-lookup"><span data-stu-id="294e7-180">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="294e7-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-181">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="294e7-182">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-182">Not supported</span></span> | <span data-ttu-id="294e7-183">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294e7-183">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="294e7-184">todoTask</span><span class="sxs-lookup"><span data-stu-id="294e7-184">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="294e7-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="294e7-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="294e7-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="294e7-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="294e7-187">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="294e7-187">Not supported</span></span> |
|[<span data-ttu-id="294e7-188">user</span><span class="sxs-lookup"><span data-stu-id="294e7-188">user</span></span>](../resources/user.md) | <span data-ttu-id="294e7-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-189">User.Read.All</span></span> | <span data-ttu-id="294e7-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-190">User.Read.All</span></span> | <span data-ttu-id="294e7-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e7-191">User.Read.All</span></span> |

> <span data-ttu-id="294e7-192">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="294e7-192">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="294e7-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="294e7-193">driveItem</span></span>

<span data-ttu-id="294e7-194">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="294e7-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="294e7-195">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="294e7-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="294e7-196">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="294e7-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="294e7-197">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="294e7-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="294e7-198">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="294e7-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="294e7-199">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="294e7-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="294e7-200">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="294e7-200">contact, event, and message</span></span>

<span data-ttu-id="294e7-201">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="294e7-201">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="294e7-202">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="294e7-202">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="294e7-203">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="294e7-203">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="294e7-204">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="294e7-204">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="294e7-205">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="294e7-205">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="294e7-206">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="294e7-206">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="294e7-207">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="294e7-207">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="294e7-208">presence</span><span class="sxs-lookup"><span data-stu-id="294e7-208">presence</span></span>

<span data-ttu-id="294e7-209">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="294e7-209">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="294e7-210">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="294e7-210">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="294e7-211">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="294e7-211">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="294e7-212">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="294e7-212">Request headers</span></span>

| <span data-ttu-id="294e7-213">Имя</span><span class="sxs-lookup"><span data-stu-id="294e7-213">Name</span></span>       | <span data-ttu-id="294e7-214">Тип</span><span class="sxs-lookup"><span data-stu-id="294e7-214">Type</span></span> | <span data-ttu-id="294e7-215">Описание</span><span class="sxs-lookup"><span data-stu-id="294e7-215">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="294e7-216">Authorization</span><span class="sxs-lookup"><span data-stu-id="294e7-216">Authorization</span></span>  | <span data-ttu-id="294e7-217">string</span><span class="sxs-lookup"><span data-stu-id="294e7-217">string</span></span>  | <span data-ttu-id="294e7-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="294e7-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="294e7-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="294e7-220">Response</span></span>

<span data-ttu-id="294e7-221">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="294e7-221">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="294e7-222">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="294e7-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="294e7-223">Пример</span><span class="sxs-lookup"><span data-stu-id="294e7-223">Example</span></span>

##### <a name="request"></a><span data-ttu-id="294e7-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="294e7-224">Request</span></span>

<span data-ttu-id="294e7-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="294e7-225">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="294e7-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="294e7-226">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="294e7-227">C#</span><span class="sxs-lookup"><span data-stu-id="294e7-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="294e7-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="294e7-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="294e7-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="294e7-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="294e7-230">Java</span><span class="sxs-lookup"><span data-stu-id="294e7-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="294e7-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="294e7-231">Response</span></span>

<span data-ttu-id="294e7-232">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="294e7-232">Here is an example of the response.</span></span>
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


