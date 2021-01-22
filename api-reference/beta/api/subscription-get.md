---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 1c5187eb36ace429d97c71a127a7c61768a4971d
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934709"
---
# <a name="get-subscription"></a><span data-ttu-id="6e281-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="6e281-103">Get subscription</span></span>

<span data-ttu-id="6e281-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e281-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e281-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="6e281-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e281-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e281-106">Permissions</span></span>

<span data-ttu-id="6e281-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6e281-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6e281-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e281-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e281-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="6e281-109">Supported resource</span></span> | <span data-ttu-id="6e281-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e281-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e281-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e281-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e281-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e281-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6e281-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="6e281-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="6e281-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-114">Not supported</span></span> | <span data-ttu-id="6e281-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-115">Not supported</span></span> | <span data-ttu-id="6e281-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="6e281-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6e281-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6e281-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="6e281-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-119">Not supported</span></span> | <span data-ttu-id="6e281-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6e281-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="6e281-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6e281-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-122">Not supported</span></span> | <span data-ttu-id="6e281-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-123">Not supported</span></span> | <span data-ttu-id="6e281-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6e281-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6e281-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6e281-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e281-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="6e281-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-127">Not supported</span></span> | <span data-ttu-id="6e281-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="6e281-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="6e281-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6e281-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-130">Not supported</span></span> | <span data-ttu-id="6e281-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-131">Not supported</span></span> | <span data-ttu-id="6e281-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6e281-133">contact</span><span class="sxs-lookup"><span data-stu-id="6e281-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6e281-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-134">Contacts.Read</span></span> | <span data-ttu-id="6e281-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-135">Contacts.Read</span></span> | <span data-ttu-id="6e281-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-136">Contacts.Read</span></span> |
|<span data-ttu-id="6e281-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="6e281-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6e281-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-138">Not supported</span></span> | <span data-ttu-id="6e281-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e281-139">Files.ReadWrite</span></span> | <span data-ttu-id="6e281-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-140">Not supported</span></span> |
|<span data-ttu-id="6e281-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6e281-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6e281-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="6e281-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-143">Not supported</span></span> | <span data-ttu-id="6e281-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6e281-145">event</span><span class="sxs-lookup"><span data-stu-id="6e281-145">event</span></span>](../resources/event.md) | <span data-ttu-id="6e281-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-146">Calendars.Read</span></span> | <span data-ttu-id="6e281-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-147">Calendars.Read</span></span> | <span data-ttu-id="6e281-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-148">Calendars.Read</span></span> |
|[<span data-ttu-id="6e281-149">group</span><span class="sxs-lookup"><span data-stu-id="6e281-149">group</span></span>](../resources/group.md) | <span data-ttu-id="6e281-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-150">Group.Read.All</span></span> | <span data-ttu-id="6e281-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-151">Not supported</span></span> | <span data-ttu-id="6e281-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-152">Group.Read.All</span></span> |
|[<span data-ttu-id="6e281-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="6e281-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6e281-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-154">Group.Read.All</span></span> | <span data-ttu-id="6e281-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-155">Not supported</span></span> | <span data-ttu-id="6e281-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-156">Not supported</span></span> |
|[<span data-ttu-id="6e281-157">list</span><span class="sxs-lookup"><span data-stu-id="6e281-157">list</span></span>](../resources/list.md) | <span data-ttu-id="6e281-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6e281-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-159">Not supported</span></span> | <span data-ttu-id="6e281-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6e281-161">message</span><span class="sxs-lookup"><span data-stu-id="6e281-161">message</span></span>](../resources/message.md) | <span data-ttu-id="6e281-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6e281-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6e281-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6e281-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6e281-165">presence</span><span class="sxs-lookup"><span data-stu-id="6e281-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="6e281-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-166">Presence.Read.All</span></span> | <span data-ttu-id="6e281-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-167">Not supported</span></span> | <span data-ttu-id="6e281-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-168">Not supported</span></span> |
|[<span data-ttu-id="6e281-169">printer</span><span class="sxs-lookup"><span data-stu-id="6e281-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="6e281-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-170">Not supported</span></span> | <span data-ttu-id="6e281-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-171">Not supported</span></span> | <span data-ttu-id="6e281-172">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="6e281-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6e281-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="6e281-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-174">Not supported</span></span> | <span data-ttu-id="6e281-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-175">Not supported</span></span> | <span data-ttu-id="6e281-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="6e281-177">security alert</span><span class="sxs-lookup"><span data-stu-id="6e281-177">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6e281-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6e281-179">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-179">Not supported</span></span> | <span data-ttu-id="6e281-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e281-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6e281-181">todoTask</span><span class="sxs-lookup"><span data-stu-id="6e281-181">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="6e281-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e281-182">Tasks.ReadWrite</span></span> | <span data-ttu-id="6e281-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e281-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="6e281-184">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e281-184">Not supported</span></span> |
|[<span data-ttu-id="6e281-185">user</span><span class="sxs-lookup"><span data-stu-id="6e281-185">user</span></span>](../resources/user.md) | <span data-ttu-id="6e281-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-186">User.Read.All</span></span> | <span data-ttu-id="6e281-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-187">User.Read.All</span></span> | <span data-ttu-id="6e281-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e281-188">User.Read.All</span></span> |

> <span data-ttu-id="6e281-189">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="6e281-189">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="6e281-190">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6e281-190">chatMessage</span></span>

<span data-ttu-id="6e281-191">**Подписки chatMessage** с делегными разрешениями не поддерживают данные ресурсов **(includeResourceData** должен быть) и `false` не требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="6e281-191">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="6e281-192">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="6e281-192">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="6e281-193">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="6e281-193">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="6e281-194">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="6e281-194">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="6e281-195">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="6e281-195">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="6e281-196">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="6e281-196">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="6e281-197">В будущем корпорация Майкрософт может потребовать от вас или ваших клиентов оплаты дополнительных платежей в зависимости от объема данных, доступных через API.</span><span class="sxs-lookup"><span data-stu-id="6e281-197">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="6e281-198">driveItem</span><span class="sxs-lookup"><span data-stu-id="6e281-198">driveItem</span></span>

<span data-ttu-id="6e281-199">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6e281-199">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="6e281-200">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6e281-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6e281-201">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="6e281-201">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6e281-202">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="6e281-202">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6e281-203">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="6e281-203">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6e281-204">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="6e281-204">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6e281-205">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="6e281-205">contact, event, and message</span></span>

<span data-ttu-id="6e281-206">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="6e281-206">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6e281-207">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6e281-207">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6e281-208">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="6e281-208">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6e281-209">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e281-209">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6e281-210">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="6e281-210">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6e281-211">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6e281-211">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6e281-212">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="6e281-212">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="6e281-213">presence</span><span class="sxs-lookup"><span data-stu-id="6e281-213">presence</span></span>

<span data-ttu-id="6e281-214">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="6e281-214">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="6e281-215">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="6e281-215">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="6e281-216">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e281-216">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e281-217">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6e281-217">Optional query parameters</span></span>

<span data-ttu-id="6e281-218">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6e281-218">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e281-219">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e281-219">Request headers</span></span>

| <span data-ttu-id="6e281-220">Имя</span><span class="sxs-lookup"><span data-stu-id="6e281-220">Name</span></span>       | <span data-ttu-id="6e281-221">Тип</span><span class="sxs-lookup"><span data-stu-id="6e281-221">Type</span></span> | <span data-ttu-id="6e281-222">Описание</span><span class="sxs-lookup"><span data-stu-id="6e281-222">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="6e281-223">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e281-223">Authorization</span></span>  | <span data-ttu-id="6e281-224">string</span><span class="sxs-lookup"><span data-stu-id="6e281-224">string</span></span>  | <span data-ttu-id="6e281-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e281-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e281-227">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e281-227">Request body</span></span>

<span data-ttu-id="6e281-228">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e281-228">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e281-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e281-229">Response</span></span>

<span data-ttu-id="6e281-230">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e281-230">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e281-231">Пример</span><span class="sxs-lookup"><span data-stu-id="6e281-231">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6e281-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e281-232">Request</span></span>

<span data-ttu-id="6e281-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e281-233">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e281-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e281-234">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="6e281-235">C#</span><span class="sxs-lookup"><span data-stu-id="6e281-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e281-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e281-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e281-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e281-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e281-238">Java</span><span class="sxs-lookup"><span data-stu-id="6e281-238">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6e281-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e281-239">Response</span></span>

<span data-ttu-id="6e281-240">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6e281-240">Here is an example of the response.</span></span>
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


