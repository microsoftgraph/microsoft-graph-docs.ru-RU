---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 0feb2d351211e4c39f76c0f5d13898fbcf30b8c6
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742239"
---
# <a name="update-subscription"></a><span data-ttu-id="5b4e6-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="5b4e6-103">Update subscription</span></span>

<span data-ttu-id="5b4e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b4e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b4e6-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="5b4e6-106">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="5b4e6-107">Чтобы избежать отсутствия уведомлений об изменениях, приложение должно правильно обновить свои подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="5b4e6-108">В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b4e6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b4e6-109">Permissions</span></span>

<span data-ttu-id="5b4e6-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="5b4e6-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b4e6-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b4e6-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="5b4e6-112">Supported resource</span></span> | <span data-ttu-id="5b4e6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b4e6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b4e6-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b4e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b4e6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b4e6-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="5b4e6-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="5b4e6-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="5b4e6-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-117">Not supported</span></span> | <span data-ttu-id="5b4e6-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-118">Not supported</span></span> | <span data-ttu-id="5b4e6-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="5b4e6-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5b4e6-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="5b4e6-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="5b4e6-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-122">Not supported</span></span> | <span data-ttu-id="5b4e6-123">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-123">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5b4e6-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="5b4e6-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="5b4e6-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-125">Not supported</span></span> | <span data-ttu-id="5b4e6-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-126">Not supported</span></span> | <span data-ttu-id="5b4e6-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5b4e6-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5b4e6-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="5b4e6-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b4e6-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="5b4e6-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-130">Not supported</span></span> | <span data-ttu-id="5b4e6-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="5b4e6-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="5b4e6-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="5b4e6-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-133">Not supported</span></span> | <span data-ttu-id="5b4e6-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-134">Not supported</span></span> | <span data-ttu-id="5b4e6-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="5b4e6-136">contact</span><span class="sxs-lookup"><span data-stu-id="5b4e6-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5b4e6-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-137">Contacts.Read</span></span> | <span data-ttu-id="5b4e6-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-138">Contacts.Read</span></span> | <span data-ttu-id="5b4e6-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-139">Contacts.Read</span></span> |
|<span data-ttu-id="5b4e6-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="5b4e6-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="5b4e6-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-141">Not supported</span></span> | <span data-ttu-id="5b4e6-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5b4e6-142">Files.ReadWrite</span></span> | <span data-ttu-id="5b4e6-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-143">Not supported</span></span> |
|<span data-ttu-id="5b4e6-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="5b4e6-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="5b4e6-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="5b4e6-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-146">Not supported</span></span> | <span data-ttu-id="5b4e6-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="5b4e6-148">event</span><span class="sxs-lookup"><span data-stu-id="5b4e6-148">event</span></span>](../resources/event.md) | <span data-ttu-id="5b4e6-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-149">Calendars.Read</span></span> | <span data-ttu-id="5b4e6-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-150">Calendars.Read</span></span> | <span data-ttu-id="5b4e6-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-151">Calendars.Read</span></span> |
|[<span data-ttu-id="5b4e6-152">group</span><span class="sxs-lookup"><span data-stu-id="5b4e6-152">group</span></span>](../resources/group.md) | <span data-ttu-id="5b4e6-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-153">Group.Read.All</span></span> | <span data-ttu-id="5b4e6-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-154">Not supported</span></span> | <span data-ttu-id="5b4e6-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-155">Group.Read.All</span></span> |
|[<span data-ttu-id="5b4e6-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="5b4e6-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="5b4e6-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-157">Group.Read.All</span></span> | <span data-ttu-id="5b4e6-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-158">Not supported</span></span> | <span data-ttu-id="5b4e6-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-159">Not supported</span></span> |
|[<span data-ttu-id="5b4e6-160">list</span><span class="sxs-lookup"><span data-stu-id="5b4e6-160">list</span></span>](../resources/list.md) | <span data-ttu-id="5b4e6-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="5b4e6-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-162">Not supported</span></span> | <span data-ttu-id="5b4e6-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="5b4e6-164">message</span><span class="sxs-lookup"><span data-stu-id="5b4e6-164">message</span></span>](../resources/message.md) | <span data-ttu-id="5b4e6-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5b4e6-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5b4e6-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5b4e6-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="5b4e6-168">presence</span><span class="sxs-lookup"><span data-stu-id="5b4e6-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="5b4e6-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-169">Presence.Read.All</span></span> | <span data-ttu-id="5b4e6-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-170">Not supported</span></span> | <span data-ttu-id="5b4e6-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-171">Not supported</span></span> |
|[<span data-ttu-id="5b4e6-172">security alert</span><span class="sxs-lookup"><span data-stu-id="5b4e6-172">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="5b4e6-173">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-173">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="5b4e6-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b4e6-174">Not supported</span></span> | <span data-ttu-id="5b4e6-175">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-175">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="5b4e6-176">user</span><span class="sxs-lookup"><span data-stu-id="5b4e6-176">user</span></span>](../resources/user.md) | <span data-ttu-id="5b4e6-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-177">User.Read.All</span></span> | <span data-ttu-id="5b4e6-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-178">User.Read.All</span></span> | <span data-ttu-id="5b4e6-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4e6-179">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="5b4e6-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="5b4e6-180">chatMessage</span></span>

<span data-ttu-id="5b4e6-181">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов (**инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="5b4e6-181">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="5b4e6-182">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="5b4e6-182">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="5b4e6-183">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="5b4e6-183">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="5b4e6-184">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-184">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="5b4e6-185">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="5b4e6-185">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="5b4e6-186">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="5b4e6-186">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="5b4e6-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="5b4e6-187">driveItem</span></span>

<span data-ttu-id="5b4e6-188">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-188">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="5b4e6-189">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="5b4e6-190">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-190">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="5b4e6-191">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-191">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="5b4e6-192">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-192">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="5b4e6-193">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-193">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="5b4e6-194">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="5b4e6-194">contact, event, and message</span></span>

<span data-ttu-id="5b4e6-195">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-195">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="5b4e6-196">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-196">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="5b4e6-197">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-197">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="5b4e6-198">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-198">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="5b4e6-199">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="5b4e6-199">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="5b4e6-200">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-200">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="5b4e6-201">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-201">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="5b4e6-202">presence</span><span class="sxs-lookup"><span data-stu-id="5b4e6-202">presence</span></span>

<span data-ttu-id="5b4e6-203">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="5b4e6-203">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="5b4e6-204">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="5b4e6-204">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="5b4e6-205">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b4e6-205">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5b4e6-206">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b4e6-206">Request headers</span></span>

| <span data-ttu-id="5b4e6-207">Имя</span><span class="sxs-lookup"><span data-stu-id="5b4e6-207">Name</span></span>       | <span data-ttu-id="5b4e6-208">Тип</span><span class="sxs-lookup"><span data-stu-id="5b4e6-208">Type</span></span> | <span data-ttu-id="5b4e6-209">Описание</span><span class="sxs-lookup"><span data-stu-id="5b4e6-209">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5b4e6-210">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b4e6-210">Authorization</span></span>  | <span data-ttu-id="5b4e6-211">string</span><span class="sxs-lookup"><span data-stu-id="5b4e6-211">string</span></span>  | <span data-ttu-id="5b4e6-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5b4e6-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b4e6-214">Response</span></span>

<span data-ttu-id="5b4e6-215">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-215">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="5b4e6-216">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="5b4e6-216">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="5b4e6-217">Пример</span><span class="sxs-lookup"><span data-stu-id="5b4e6-217">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5b4e6-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b4e6-218">Request</span></span>

<span data-ttu-id="5b4e6-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-219">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b4e6-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b4e6-220">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5b4e6-221">C#</span><span class="sxs-lookup"><span data-stu-id="5b4e6-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b4e6-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b4e6-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b4e6-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b4e6-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5b4e6-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b4e6-224">Response</span></span>

<span data-ttu-id="5b4e6-225">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4e6-225">Here is an example of the response.</span></span>
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


