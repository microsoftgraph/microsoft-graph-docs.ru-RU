---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5518091d21a3ed2e1c05a8bc95c70b62d7cb82eb
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934840"
---
# <a name="delete-subscription"></a><span data-ttu-id="fcd97-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="fcd97-103">Delete subscription</span></span>

<span data-ttu-id="fcd97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcd97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcd97-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="fcd97-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcd97-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcd97-106">Permissions</span></span>

<span data-ttu-id="fcd97-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fcd97-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="fcd97-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcd97-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fcd97-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="fcd97-109">Supported resource</span></span> | <span data-ttu-id="fcd97-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcd97-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fcd97-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcd97-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcd97-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="fcd97-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="fcd97-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="fcd97-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="fcd97-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-114">Not supported</span></span> | <span data-ttu-id="fcd97-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-115">Not supported</span></span> | <span data-ttu-id="fcd97-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="fcd97-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="fcd97-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="fcd97-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="fcd97-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-119">Not supported</span></span> | <span data-ttu-id="fcd97-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="fcd97-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="fcd97-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="fcd97-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-122">Not supported</span></span> | <span data-ttu-id="fcd97-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-123">Not supported</span></span> | <span data-ttu-id="fcd97-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="fcd97-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="fcd97-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="fcd97-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcd97-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="fcd97-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-127">Not supported</span></span> | <span data-ttu-id="fcd97-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="fcd97-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="fcd97-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="fcd97-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-130">Not supported</span></span> | <span data-ttu-id="fcd97-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-131">Not supported</span></span> | <span data-ttu-id="fcd97-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="fcd97-133">contact</span><span class="sxs-lookup"><span data-stu-id="fcd97-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="fcd97-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-134">Contacts.Read</span></span> | <span data-ttu-id="fcd97-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-135">Contacts.Read</span></span> | <span data-ttu-id="fcd97-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-136">Contacts.Read</span></span> |
|<span data-ttu-id="fcd97-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="fcd97-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="fcd97-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-138">Not supported</span></span> | <span data-ttu-id="fcd97-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcd97-139">Files.ReadWrite</span></span> | <span data-ttu-id="fcd97-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-140">Not supported</span></span> |
|<span data-ttu-id="fcd97-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="fcd97-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="fcd97-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="fcd97-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-143">Not supported</span></span> | <span data-ttu-id="fcd97-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="fcd97-145">event</span><span class="sxs-lookup"><span data-stu-id="fcd97-145">event</span></span>](../resources/event.md) | <span data-ttu-id="fcd97-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-146">Calendars.Read</span></span> | <span data-ttu-id="fcd97-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-147">Calendars.Read</span></span> | <span data-ttu-id="fcd97-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-148">Calendars.Read</span></span> |
|[<span data-ttu-id="fcd97-149">group</span><span class="sxs-lookup"><span data-stu-id="fcd97-149">group</span></span>](../resources/group.md) | <span data-ttu-id="fcd97-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-150">Group.Read.All</span></span> | <span data-ttu-id="fcd97-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-151">Not supported</span></span> | <span data-ttu-id="fcd97-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-152">Group.Read.All</span></span> |
|[<span data-ttu-id="fcd97-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="fcd97-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="fcd97-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-154">Group.Read.All</span></span> | <span data-ttu-id="fcd97-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-155">Not supported</span></span> | <span data-ttu-id="fcd97-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-156">Not supported</span></span> |
|[<span data-ttu-id="fcd97-157">list</span><span class="sxs-lookup"><span data-stu-id="fcd97-157">list</span></span>](../resources/list.md) | <span data-ttu-id="fcd97-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="fcd97-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-159">Not supported</span></span> | <span data-ttu-id="fcd97-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="fcd97-161">message</span><span class="sxs-lookup"><span data-stu-id="fcd97-161">message</span></span>](../resources/message.md) | <span data-ttu-id="fcd97-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="fcd97-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="fcd97-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fcd97-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="fcd97-165">presence</span><span class="sxs-lookup"><span data-stu-id="fcd97-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="fcd97-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-166">Presence.Read.All</span></span> | <span data-ttu-id="fcd97-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-167">Not supported</span></span> | <span data-ttu-id="fcd97-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-168">Not supported</span></span> |
|[<span data-ttu-id="fcd97-169">printer</span><span class="sxs-lookup"><span data-stu-id="fcd97-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="fcd97-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-170">Not supported</span></span> | <span data-ttu-id="fcd97-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-171">Not supported</span></span> | <span data-ttu-id="fcd97-172">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="fcd97-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="fcd97-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="fcd97-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-174">Not supported</span></span> | <span data-ttu-id="fcd97-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-175">Not supported</span></span> | <span data-ttu-id="fcd97-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="fcd97-177">security alert</span><span class="sxs-lookup"><span data-stu-id="fcd97-177">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="fcd97-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="fcd97-179">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-179">Not supported</span></span> | <span data-ttu-id="fcd97-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="fcd97-181">todoTask</span><span class="sxs-lookup"><span data-stu-id="fcd97-181">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="fcd97-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcd97-182">Tasks.ReadWrite</span></span> | <span data-ttu-id="fcd97-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcd97-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="fcd97-184">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fcd97-184">Not supported</span></span> |
|[<span data-ttu-id="fcd97-185">user</span><span class="sxs-lookup"><span data-stu-id="fcd97-185">user</span></span>](../resources/user.md) | <span data-ttu-id="fcd97-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-186">User.Read.All</span></span> | <span data-ttu-id="fcd97-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-187">User.Read.All</span></span> | <span data-ttu-id="fcd97-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcd97-188">User.Read.All</span></span> |

> <span data-ttu-id="fcd97-189">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="fcd97-189">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="fcd97-190">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fcd97-190">chatMessage</span></span>

<span data-ttu-id="fcd97-191">**Подписки chatMessage** с делегными разрешениями не поддерживают данные ресурсов **(includeResourceData** должен быть) и `false` не требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="fcd97-191">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="fcd97-192">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="fcd97-192">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="fcd97-193">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="fcd97-193">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="fcd97-194">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="fcd97-194">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="fcd97-195">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="fcd97-195">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="fcd97-196">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="fcd97-196">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="fcd97-197">В будущем корпорация Майкрософт может потребовать от вас или ваших клиентов оплаты дополнительных платежей в зависимости от объема данных, доступных через API.</span><span class="sxs-lookup"><span data-stu-id="fcd97-197">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="fcd97-198">driveItem</span><span class="sxs-lookup"><span data-stu-id="fcd97-198">driveItem</span></span>

<span data-ttu-id="fcd97-199">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fcd97-199">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="fcd97-200">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="fcd97-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="fcd97-201">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="fcd97-201">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="fcd97-202">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="fcd97-202">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="fcd97-203">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="fcd97-203">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="fcd97-204">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="fcd97-204">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="fcd97-205">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="fcd97-205">contact, event, and message</span></span>

<span data-ttu-id="fcd97-206">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="fcd97-206">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="fcd97-207">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="fcd97-207">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="fcd97-208">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="fcd97-208">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="fcd97-209">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="fcd97-209">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="fcd97-210">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="fcd97-210">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="fcd97-211">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="fcd97-211">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="fcd97-212">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="fcd97-212">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="fcd97-213">presence</span><span class="sxs-lookup"><span data-stu-id="fcd97-213">presence</span></span>

<span data-ttu-id="fcd97-214">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="fcd97-214">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="fcd97-215">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="fcd97-215">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="fcd97-216">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcd97-216">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="fcd97-217">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcd97-217">Request headers</span></span>

| <span data-ttu-id="fcd97-218">Имя</span><span class="sxs-lookup"><span data-stu-id="fcd97-218">Name</span></span>       | <span data-ttu-id="fcd97-219">Тип</span><span class="sxs-lookup"><span data-stu-id="fcd97-219">Type</span></span> | <span data-ttu-id="fcd97-220">Описание</span><span class="sxs-lookup"><span data-stu-id="fcd97-220">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fcd97-221">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcd97-221">Authorization</span></span>  | <span data-ttu-id="fcd97-222">string</span><span class="sxs-lookup"><span data-stu-id="fcd97-222">string</span></span>  | <span data-ttu-id="fcd97-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcd97-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcd97-225">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcd97-225">Request body</span></span>

<span data-ttu-id="fcd97-226">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcd97-226">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcd97-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcd97-227">Response</span></span>

<span data-ttu-id="fcd97-228">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fcd97-228">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="fcd97-229">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="fcd97-229">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="fcd97-230">Пример</span><span class="sxs-lookup"><span data-stu-id="fcd97-230">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fcd97-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcd97-231">Request</span></span>

<span data-ttu-id="fcd97-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcd97-232">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fcd97-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcd97-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="fcd97-234">C#</span><span class="sxs-lookup"><span data-stu-id="fcd97-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcd97-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcd97-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcd97-236">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcd97-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fcd97-237">Java</span><span class="sxs-lookup"><span data-stu-id="fcd97-237">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fcd97-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcd97-238">Response</span></span>

<span data-ttu-id="fcd97-239">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fcd97-239">Here is an example of the response.</span></span>
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


