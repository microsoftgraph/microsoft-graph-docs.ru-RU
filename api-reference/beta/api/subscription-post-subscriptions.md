---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 36555a946aa9092d5cab6e27548a16ba783d738e
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598138"
---
# <a name="create-subscription"></a><span data-ttu-id="e9d54-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="e9d54-103">Create subscription</span></span>

<span data-ttu-id="e9d54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9d54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9d54-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e9d54-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9d54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9d54-106">Permissions</span></span>

<span data-ttu-id="e9d54-107">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="e9d54-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="e9d54-108">Например, чтобы получать уведомления об изменениях для сообщений, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="e9d54-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="e9d54-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e9d54-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e9d54-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9d54-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9d54-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="e9d54-111">Supported resource</span></span> | <span data-ttu-id="e9d54-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9d54-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9d54-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9d54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9d54-114">Application</span><span class="sxs-lookup"><span data-stu-id="e9d54-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="e9d54-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="e9d54-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="e9d54-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-116">Not supported</span></span> | <span data-ttu-id="e9d54-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-117">Not supported</span></span> | <span data-ttu-id="e9d54-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="e9d54-119">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="e9d54-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="e9d54-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="e9d54-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-121">Not supported</span></span> | <span data-ttu-id="e9d54-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e9d54-123">[chatMessage](../resources/chatmessage.md) (/теамс/аллмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="e9d54-123">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="e9d54-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-124">Not supported</span></span> | <span data-ttu-id="e9d54-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-125">Not supported</span></span> | <span data-ttu-id="e9d54-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="e9d54-127">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="e9d54-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="e9d54-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9d54-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="e9d54-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-129">Not supported</span></span> | <span data-ttu-id="e9d54-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="e9d54-131">[chatMessage](../resources/chatmessage.md) (/ЧАТС/аллмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="e9d54-131">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="e9d54-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-132">Not supported</span></span> | <span data-ttu-id="e9d54-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-133">Not supported</span></span> | <span data-ttu-id="e9d54-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="e9d54-135">contact</span><span class="sxs-lookup"><span data-stu-id="e9d54-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e9d54-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-136">Contacts.Read</span></span> | <span data-ttu-id="e9d54-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-137">Contacts.Read</span></span> | <span data-ttu-id="e9d54-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-138">Contacts.Read</span></span> |
|<span data-ttu-id="e9d54-139">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="e9d54-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e9d54-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-140">Not supported</span></span> | <span data-ttu-id="e9d54-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9d54-141">Files.ReadWrite</span></span> | <span data-ttu-id="e9d54-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-142">Not supported</span></span> |
|<span data-ttu-id="e9d54-143">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="e9d54-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e9d54-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="e9d54-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-145">Not supported</span></span> | <span data-ttu-id="e9d54-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e9d54-147">event</span><span class="sxs-lookup"><span data-stu-id="e9d54-147">event</span></span>](../resources/event.md) | <span data-ttu-id="e9d54-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-148">Calendars.Read</span></span> | <span data-ttu-id="e9d54-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-149">Calendars.Read</span></span> | <span data-ttu-id="e9d54-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-150">Calendars.Read</span></span> |
|[<span data-ttu-id="e9d54-151">group</span><span class="sxs-lookup"><span data-stu-id="e9d54-151">group</span></span>](../resources/group.md) | <span data-ttu-id="e9d54-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-152">Group.Read.All</span></span> | <span data-ttu-id="e9d54-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-153">Not supported</span></span> | <span data-ttu-id="e9d54-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-154">Group.Read.All</span></span> |
|[<span data-ttu-id="e9d54-155">group conversation</span><span class="sxs-lookup"><span data-stu-id="e9d54-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e9d54-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-156">Group.Read.All</span></span> | <span data-ttu-id="e9d54-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-157">Not supported</span></span> | <span data-ttu-id="e9d54-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-158">Not supported</span></span> |
|[<span data-ttu-id="e9d54-159">list</span><span class="sxs-lookup"><span data-stu-id="e9d54-159">list</span></span>](../resources/list.md) | <span data-ttu-id="e9d54-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="e9d54-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-161">Not supported</span></span> | <span data-ttu-id="e9d54-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="e9d54-163">message</span><span class="sxs-lookup"><span data-stu-id="e9d54-163">message</span></span>](../resources/message.md) | <span data-ttu-id="e9d54-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e9d54-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e9d54-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e9d54-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="e9d54-167">presence</span><span class="sxs-lookup"><span data-stu-id="e9d54-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="e9d54-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-168">Presence.Read.All</span></span> | <span data-ttu-id="e9d54-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-169">Not supported</span></span> | <span data-ttu-id="e9d54-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-170">Not supported</span></span> |
|[<span data-ttu-id="e9d54-171">security alert</span><span class="sxs-lookup"><span data-stu-id="e9d54-171">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="e9d54-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-172">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e9d54-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e9d54-173">Not supported</span></span> | <span data-ttu-id="e9d54-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-174">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="e9d54-175">user</span><span class="sxs-lookup"><span data-stu-id="e9d54-175">user</span></span>](../resources/user.md) | <span data-ttu-id="e9d54-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-176">User.Read.All</span></span> | <span data-ttu-id="e9d54-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-177">User.Read.All</span></span> | <span data-ttu-id="e9d54-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d54-178">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="e9d54-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e9d54-179">chatMessage</span></span>

<span data-ttu-id="e9d54-180">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов (**инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="e9d54-180">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="e9d54-181">подписки **chatMessage** с разрешениями приложений включают данные ресурсов и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="e9d54-181">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="e9d54-182">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e9d54-182">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="e9d54-183">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="e9d54-183">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="e9d54-184">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="e9d54-184">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="e9d54-185">**Примечание:** `/teams/allMessages` и `/chats/allMessages` в настоящее время находятся в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="e9d54-185">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="e9d54-186">Во время предварительной версии вы можете использовать этот API без сборов в соответствии с [условиями использования API Майкрософт](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="e9d54-186">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="e9d54-187">Однако пользователям приложений, использующих API, может потребоваться подписка на конкретные решения Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e9d54-187">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="e9d54-188">После общедоступной доступности Корпорация Майкрософт может потребовать от вас или ваших клиентов взимать дополнительные сборы на основе объема данных, доступ к которым осуществляется через API.</span><span class="sxs-lookup"><span data-stu-id="e9d54-188">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="e9d54-189">driveItem</span><span class="sxs-lookup"><span data-stu-id="e9d54-189">driveItem</span></span>

<span data-ttu-id="e9d54-190">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e9d54-190">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="e9d54-191">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="e9d54-191">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="e9d54-192">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="e9d54-192">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e9d54-193">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="e9d54-193">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e9d54-194">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="e9d54-194">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="e9d54-195">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="e9d54-195">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="e9d54-196">контакты, события и сообщения</span><span class="sxs-lookup"><span data-stu-id="e9d54-196">contact, event, and message</span></span>

<span data-ttu-id="e9d54-197">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="e9d54-197">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="e9d54-198">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="e9d54-198">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="e9d54-199">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="e9d54-199">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e9d54-200">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9d54-200">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="e9d54-201">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="e9d54-201">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e9d54-202">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e9d54-202">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e9d54-203">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="e9d54-203">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="e9d54-204">presence</span><span class="sxs-lookup"><span data-stu-id="e9d54-204">presence</span></span>

<span data-ttu-id="e9d54-205">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="e9d54-205">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="e9d54-206">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e9d54-206">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="e9d54-207">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9d54-207">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="e9d54-208">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9d54-208">Request headers</span></span>

| <span data-ttu-id="e9d54-209">Имя</span><span class="sxs-lookup"><span data-stu-id="e9d54-209">Name</span></span>       | <span data-ttu-id="e9d54-210">Тип</span><span class="sxs-lookup"><span data-stu-id="e9d54-210">Type</span></span> | <span data-ttu-id="e9d54-211">Описание</span><span class="sxs-lookup"><span data-stu-id="e9d54-211">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e9d54-212">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9d54-212">Authorization</span></span>  | <span data-ttu-id="e9d54-213">string</span><span class="sxs-lookup"><span data-stu-id="e9d54-213">string</span></span>  | <span data-ttu-id="e9d54-p110">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9d54-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e9d54-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9d54-216">Response</span></span>

<span data-ttu-id="e9d54-217">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9d54-217">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="e9d54-218">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="e9d54-218">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="e9d54-219">Пример</span><span class="sxs-lookup"><span data-stu-id="e9d54-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9d54-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9d54-220">Request</span></span>

<span data-ttu-id="e9d54-221">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9d54-221">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="e9d54-222">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="e9d54-222">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="e9d54-223">Этот запрос создает подписку на уведомления об изменениях новой почты, полученной в текущий момент, когда пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="e9d54-223">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9d54-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9d54-224">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e9d54-225">C#</span><span class="sxs-lookup"><span data-stu-id="e9d54-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9d54-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9d54-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9d54-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9d54-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e9d54-228">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="e9d54-228">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="e9d54-229">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="e9d54-229">Resource type</span></span> | <span data-ttu-id="e9d54-230">Примеры</span><span class="sxs-lookup"><span data-stu-id="e9d54-230">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="e9d54-231">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="e9d54-231">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="e9d54-232">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="e9d54-232">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="e9d54-233">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span><span class="sxs-lookup"><span data-stu-id="e9d54-233">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span></span> |
|[<span data-ttu-id="e9d54-234">Контакты</span><span class="sxs-lookup"><span data-stu-id="e9d54-234">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="e9d54-235">Беседы</span><span class="sxs-lookup"><span data-stu-id="e9d54-235">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="e9d54-236">Drives</span><span class="sxs-lookup"><span data-stu-id="e9d54-236">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="e9d54-237">События</span><span class="sxs-lookup"><span data-stu-id="e9d54-237">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="e9d54-238">Группы</span><span class="sxs-lookup"><span data-stu-id="e9d54-238">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="e9d54-239">List</span><span class="sxs-lookup"><span data-stu-id="e9d54-239">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="e9d54-240">Почта</span><span class="sxs-lookup"><span data-stu-id="e9d54-240">Mail</span></span>](../resources/message.md)|<span data-ttu-id="e9d54-241">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="e9d54-241">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="e9d54-242">Знак</span><span class="sxs-lookup"><span data-stu-id="e9d54-242">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="e9d54-243">`/communications/presences/{id}`(один пользователь) `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="e9d54-243">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|<span data-ttu-id="e9d54-244">[пользователи](../resources/user.md);</span><span class="sxs-lookup"><span data-stu-id="e9d54-244">[Users](../resources/user.md)</span></span>|`users`|
|[<span data-ttu-id="e9d54-245">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="e9d54-245">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="e9d54-246">**Примечание:** Любой путь, начинающийся с, `me` можно также использовать `users/{id}` вместо `me` целевого определенного пользователя вместо текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9d54-246">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="e9d54-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9d54-247">Response</span></span>

<span data-ttu-id="e9d54-248">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e9d54-248">The following example shows the response.</span></span> 

><span data-ttu-id="e9d54-p112">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9d54-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="e9d54-251">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="e9d54-251">Notification endpoint validation</span></span>

<span data-ttu-id="e9d54-252">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="e9d54-252">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="e9d54-253">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="e9d54-253">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
