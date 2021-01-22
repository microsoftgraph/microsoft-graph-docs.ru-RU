---
title: Создание подписки
description: Подписывает приложение прослушиватель на получение уведомлений об изменениях при изменении данных ресурса Microsoft Graph.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 9efe9120d71f12955f1495cca954d9e873b3da35
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934564"
---
# <a name="create-subscription"></a><span data-ttu-id="665fb-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="665fb-103">Create subscription</span></span>

<span data-ttu-id="665fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="665fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="665fb-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="665fb-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="665fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="665fb-106">Permissions</span></span>

<span data-ttu-id="665fb-107">Для создания подписки требуется разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="665fb-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="665fb-108">Например, чтобы получать уведомления об изменениях в сообщениях, приложению необходимо разрешение Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="665fb-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="665fb-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="665fb-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="665fb-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="665fb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="665fb-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="665fb-111">Supported resource</span></span> | <span data-ttu-id="665fb-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="665fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="665fb-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="665fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="665fb-114">Application</span><span class="sxs-lookup"><span data-stu-id="665fb-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="665fb-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="665fb-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="665fb-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-116">Not supported</span></span> | <span data-ttu-id="665fb-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-117">Not supported</span></span> | <span data-ttu-id="665fb-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="665fb-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="665fb-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="665fb-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="665fb-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-121">Not supported</span></span> | <span data-ttu-id="665fb-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="665fb-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="665fb-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="665fb-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-124">Not supported</span></span> | <span data-ttu-id="665fb-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-125">Not supported</span></span> | <span data-ttu-id="665fb-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="665fb-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="665fb-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="665fb-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="665fb-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="665fb-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-129">Not supported</span></span> | <span data-ttu-id="665fb-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="665fb-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="665fb-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="665fb-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-132">Not supported</span></span> | <span data-ttu-id="665fb-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-133">Not supported</span></span> | <span data-ttu-id="665fb-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="665fb-135">contact</span><span class="sxs-lookup"><span data-stu-id="665fb-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="665fb-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-136">Contacts.Read</span></span> | <span data-ttu-id="665fb-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-137">Contacts.Read</span></span> | <span data-ttu-id="665fb-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-138">Contacts.Read</span></span> |
|<span data-ttu-id="665fb-139">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="665fb-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="665fb-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-140">Not supported</span></span> | <span data-ttu-id="665fb-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="665fb-141">Files.ReadWrite</span></span> | <span data-ttu-id="665fb-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-142">Not supported</span></span> |
|<span data-ttu-id="665fb-143">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="665fb-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="665fb-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="665fb-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-145">Not supported</span></span> | <span data-ttu-id="665fb-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="665fb-147">event</span><span class="sxs-lookup"><span data-stu-id="665fb-147">event</span></span>](../resources/event.md) | <span data-ttu-id="665fb-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-148">Calendars.Read</span></span> | <span data-ttu-id="665fb-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-149">Calendars.Read</span></span> | <span data-ttu-id="665fb-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-150">Calendars.Read</span></span> |
|[<span data-ttu-id="665fb-151">group</span><span class="sxs-lookup"><span data-stu-id="665fb-151">group</span></span>](../resources/group.md) | <span data-ttu-id="665fb-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-152">Group.Read.All</span></span> | <span data-ttu-id="665fb-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-153">Not supported</span></span> | <span data-ttu-id="665fb-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-154">Group.Read.All</span></span> |
|[<span data-ttu-id="665fb-155">group conversation</span><span class="sxs-lookup"><span data-stu-id="665fb-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="665fb-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-156">Group.Read.All</span></span> | <span data-ttu-id="665fb-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-157">Not supported</span></span> | <span data-ttu-id="665fb-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-158">Not supported</span></span> |
|[<span data-ttu-id="665fb-159">list</span><span class="sxs-lookup"><span data-stu-id="665fb-159">list</span></span>](../resources/list.md) | <span data-ttu-id="665fb-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="665fb-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-161">Not supported</span></span> | <span data-ttu-id="665fb-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="665fb-163">message</span><span class="sxs-lookup"><span data-stu-id="665fb-163">message</span></span>](../resources/message.md) | <span data-ttu-id="665fb-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="665fb-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="665fb-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="665fb-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="665fb-167">presence</span><span class="sxs-lookup"><span data-stu-id="665fb-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="665fb-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-168">Presence.Read.All</span></span> | <span data-ttu-id="665fb-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-169">Not supported</span></span> | <span data-ttu-id="665fb-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-170">Not supported</span></span> |
|[<span data-ttu-id="665fb-171">printer</span><span class="sxs-lookup"><span data-stu-id="665fb-171">printer</span></span>](../resources/printer.md) | <span data-ttu-id="665fb-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-172">Not supported</span></span> | <span data-ttu-id="665fb-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-173">Not supported</span></span> | <span data-ttu-id="665fb-174">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-174">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="665fb-175">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="665fb-175">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="665fb-176">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-176">Not supported</span></span> | <span data-ttu-id="665fb-177">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-177">Not supported</span></span> | <span data-ttu-id="665fb-178">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-178">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="665fb-179">security alert</span><span class="sxs-lookup"><span data-stu-id="665fb-179">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="665fb-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-180">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="665fb-181">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-181">Not supported</span></span> | <span data-ttu-id="665fb-182">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665fb-182">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="665fb-183">todoTask</span><span class="sxs-lookup"><span data-stu-id="665fb-183">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="665fb-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="665fb-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="665fb-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="665fb-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="665fb-186">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="665fb-186">Not supported</span></span> |
|[<span data-ttu-id="665fb-187">user</span><span class="sxs-lookup"><span data-stu-id="665fb-187">user</span></span>](../resources/user.md) | <span data-ttu-id="665fb-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-188">User.Read.All</span></span> | <span data-ttu-id="665fb-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-189">User.Read.All</span></span> | <span data-ttu-id="665fb-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="665fb-190">User.Read.All</span></span> |

> <span data-ttu-id="665fb-191">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="665fb-191">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="665fb-192">chatMessage</span><span class="sxs-lookup"><span data-stu-id="665fb-192">chatMessage</span></span>

<span data-ttu-id="665fb-193">**Подписки chatMessage** с делегными разрешениями не поддерживают данные ресурсов **(includeResourceData** должен быть) и `false` не требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="665fb-193">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="665fb-194">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="665fb-194">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="665fb-195">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="665fb-195">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="665fb-196">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="665fb-196">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="665fb-197">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="665fb-197">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="665fb-198">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="665fb-198">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="665fb-199">В будущем корпорация Майкрософт может потребовать от вас или ваших клиентов оплаты дополнительных платежей в зависимости от объема данных, доступных через API.</span><span class="sxs-lookup"><span data-stu-id="665fb-199">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

> <span data-ttu-id="665fb-200">**Примечание.** `/chats/getAllMessages` возвращает только сообщения из чатов, владельцем клиента.</span><span class="sxs-lookup"><span data-stu-id="665fb-200">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="665fb-201">Если поток чата инициировался пользователем за пределами клиента, этот поток чата не принадлежит арендатору и не создает уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="665fb-201">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="665fb-202">driveItem</span><span class="sxs-lookup"><span data-stu-id="665fb-202">driveItem</span></span>

<span data-ttu-id="665fb-203">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="665fb-203">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="665fb-204">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="665fb-204">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="665fb-205">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="665fb-205">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="665fb-206">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="665fb-206">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="665fb-207">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="665fb-207">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="665fb-208">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="665fb-208">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="665fb-209">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="665fb-209">contact, event, and message</span></span>

<span data-ttu-id="665fb-210">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="665fb-210">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="665fb-211">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="665fb-211">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="665fb-212">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="665fb-212">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="665fb-213">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="665fb-213">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="665fb-214">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="665fb-214">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="665fb-215">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="665fb-215">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="665fb-216">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="665fb-216">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="665fb-217">presence</span><span class="sxs-lookup"><span data-stu-id="665fb-217">presence</span></span>

<span data-ttu-id="665fb-218">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="665fb-218">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="665fb-219">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="665fb-219">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="665fb-220">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="665fb-220">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="665fb-221">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="665fb-221">Request headers</span></span>

| <span data-ttu-id="665fb-222">Имя</span><span class="sxs-lookup"><span data-stu-id="665fb-222">Name</span></span>       | <span data-ttu-id="665fb-223">Тип</span><span class="sxs-lookup"><span data-stu-id="665fb-223">Type</span></span> | <span data-ttu-id="665fb-224">Описание</span><span class="sxs-lookup"><span data-stu-id="665fb-224">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="665fb-225">Authorization</span><span class="sxs-lookup"><span data-stu-id="665fb-225">Authorization</span></span>  | <span data-ttu-id="665fb-226">string</span><span class="sxs-lookup"><span data-stu-id="665fb-226">string</span></span>  | <span data-ttu-id="665fb-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="665fb-p111">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="665fb-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="665fb-229">Response</span></span>

<span data-ttu-id="665fb-230">В случае успеха этот метод возвращает код отклика и `201 Created` объект [подписки](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="665fb-230">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="665fb-231">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="665fb-231">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="665fb-232">Пример</span><span class="sxs-lookup"><span data-stu-id="665fb-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="665fb-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="665fb-233">Request</span></span>

<span data-ttu-id="665fb-234">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="665fb-234">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="665fb-235">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="665fb-235">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="665fb-236">Этот запрос создает подписку для уведомлений об изменениях о новых сообщениях, полученных текущим пользователем, выписав его.</span><span class="sxs-lookup"><span data-stu-id="665fb-236">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="665fb-237">HTTP</span><span class="sxs-lookup"><span data-stu-id="665fb-237">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="665fb-238">C#</span><span class="sxs-lookup"><span data-stu-id="665fb-238">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="665fb-239">JavaScript</span><span class="sxs-lookup"><span data-stu-id="665fb-239">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="665fb-240">Objective-C</span><span class="sxs-lookup"><span data-stu-id="665fb-240">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="665fb-241">Java</span><span class="sxs-lookup"><span data-stu-id="665fb-241">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="665fb-242">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="665fb-242">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="665fb-243">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="665fb-243">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="665fb-244">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="665fb-244">Resources examples</span></span>

<span data-ttu-id="665fb-245">Ниже следующую допустимую величину свойства ресурса.</span><span class="sxs-lookup"><span data-stu-id="665fb-245">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="665fb-246">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="665fb-246">Resource type</span></span> | <span data-ttu-id="665fb-247">Примеры</span><span class="sxs-lookup"><span data-stu-id="665fb-247">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="665fb-248">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="665fb-248">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="665fb-249">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="665fb-249">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="665fb-250">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="665fb-250">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="665fb-251">Контакты</span><span class="sxs-lookup"><span data-stu-id="665fb-251">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="665fb-252">Беседы</span><span class="sxs-lookup"><span data-stu-id="665fb-252">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="665fb-253">Диски</span><span class="sxs-lookup"><span data-stu-id="665fb-253">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="665fb-254">События</span><span class="sxs-lookup"><span data-stu-id="665fb-254">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="665fb-255">Группы</span><span class="sxs-lookup"><span data-stu-id="665fb-255">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="665fb-256">Список</span><span class="sxs-lookup"><span data-stu-id="665fb-256">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="665fb-257">Почта</span><span class="sxs-lookup"><span data-stu-id="665fb-257">Mail</span></span>](../resources/message.md)|<span data-ttu-id="665fb-258">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="665fb-258">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="665fb-259">Присутствие</span><span class="sxs-lookup"><span data-stu-id="665fb-259">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="665fb-260">`/communications/presences/{id}` (один пользователь), `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="665fb-260">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="665fb-261">printer</span><span class="sxs-lookup"><span data-stu-id="665fb-261">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="665fb-262">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="665fb-262">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|<span data-ttu-id="665fb-263">[пользователи](../resources/user.md);</span><span class="sxs-lookup"><span data-stu-id="665fb-263">[Users](../resources/user.md)</span></span>|`users`|
|[<span data-ttu-id="665fb-264">todoTask</span><span class="sxs-lookup"><span data-stu-id="665fb-264">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="665fb-265">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="665fb-265">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="665fb-266">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="665fb-266">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="665fb-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="665fb-267">Response</span></span>

<span data-ttu-id="665fb-268">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="665fb-268">The following example shows the response.</span></span> 

><span data-ttu-id="665fb-p114">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="665fb-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="665fb-271">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="665fb-271">Notification endpoint validation</span></span>

<span data-ttu-id="665fb-272">Конечная точка уведомлений о подписке (указанная в свойстве **notificationUrl)** должна отвечать на запрос проверки, как описано в описании в настройках уведомлений об изменениях данных [пользователя.](/graph/webhooks#notification-endpoint-validation)</span><span class="sxs-lookup"><span data-stu-id="665fb-272">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="665fb-273">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="665fb-273">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


