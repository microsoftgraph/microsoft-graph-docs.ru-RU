---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: a2a2b112974e25840127a1deabfcb893c53dac1f
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193404"
---
# <a name="create-subscription"></a><span data-ttu-id="84651-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="84651-103">Create subscription</span></span>

<span data-ttu-id="84651-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84651-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84651-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="84651-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="84651-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84651-106">Permissions</span></span>

<span data-ttu-id="84651-107">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="84651-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="84651-108">Например, чтобы получать уведомления об изменениях для сообщений, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="84651-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="84651-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="84651-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="84651-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84651-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84651-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="84651-111">Supported resource</span></span> | <span data-ttu-id="84651-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84651-112">Delegated (work or school account)</span></span> | <span data-ttu-id="84651-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84651-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84651-114">Application</span><span class="sxs-lookup"><span data-stu-id="84651-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="84651-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="84651-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="84651-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-116">Not supported</span></span> | <span data-ttu-id="84651-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-117">Not supported</span></span> | <span data-ttu-id="84651-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="84651-119">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="84651-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="84651-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84651-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="84651-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-121">Not supported</span></span> | <span data-ttu-id="84651-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="84651-123">[chatMessage](../resources/chatmessage.md) (/теамс/жеталлмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="84651-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="84651-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-124">Not supported</span></span> | <span data-ttu-id="84651-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-125">Not supported</span></span> | <span data-ttu-id="84651-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="84651-127">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="84651-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="84651-128">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84651-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="84651-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-129">Not supported</span></span> | <span data-ttu-id="84651-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="84651-131">[chatMessage](../resources/chatmessage.md) (/ЧАТС/жеталлмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="84651-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="84651-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-132">Not supported</span></span> | <span data-ttu-id="84651-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-133">Not supported</span></span> | <span data-ttu-id="84651-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="84651-135">contact</span><span class="sxs-lookup"><span data-stu-id="84651-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="84651-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="84651-136">Contacts.Read</span></span> | <span data-ttu-id="84651-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="84651-137">Contacts.Read</span></span> | <span data-ttu-id="84651-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="84651-138">Contacts.Read</span></span> |
|<span data-ttu-id="84651-139">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="84651-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="84651-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-140">Not supported</span></span> | <span data-ttu-id="84651-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84651-141">Files.ReadWrite</span></span> | <span data-ttu-id="84651-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-142">Not supported</span></span> |
|<span data-ttu-id="84651-143">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="84651-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="84651-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84651-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="84651-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-145">Not supported</span></span> | <span data-ttu-id="84651-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84651-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="84651-147">event</span><span class="sxs-lookup"><span data-stu-id="84651-147">event</span></span>](../resources/event.md) | <span data-ttu-id="84651-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="84651-148">Calendars.Read</span></span> | <span data-ttu-id="84651-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="84651-149">Calendars.Read</span></span> | <span data-ttu-id="84651-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="84651-150">Calendars.Read</span></span> |
|[<span data-ttu-id="84651-151">group</span><span class="sxs-lookup"><span data-stu-id="84651-151">group</span></span>](../resources/group.md) | <span data-ttu-id="84651-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-152">Group.Read.All</span></span> | <span data-ttu-id="84651-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-153">Not supported</span></span> | <span data-ttu-id="84651-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-154">Group.Read.All</span></span> |
|[<span data-ttu-id="84651-155">group conversation</span><span class="sxs-lookup"><span data-stu-id="84651-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="84651-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-156">Group.Read.All</span></span> | <span data-ttu-id="84651-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-157">Not supported</span></span> | <span data-ttu-id="84651-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-158">Not supported</span></span> |
|[<span data-ttu-id="84651-159">list</span><span class="sxs-lookup"><span data-stu-id="84651-159">list</span></span>](../resources/list.md) | <span data-ttu-id="84651-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84651-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="84651-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-161">Not supported</span></span> | <span data-ttu-id="84651-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84651-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="84651-163">message</span><span class="sxs-lookup"><span data-stu-id="84651-163">message</span></span>](../resources/message.md) | <span data-ttu-id="84651-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="84651-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="84651-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="84651-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="84651-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="84651-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="84651-167">presence</span><span class="sxs-lookup"><span data-stu-id="84651-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="84651-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-168">Presence.Read.All</span></span> | <span data-ttu-id="84651-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-169">Not supported</span></span> | <span data-ttu-id="84651-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-170">Not supported</span></span> |
|[<span data-ttu-id="84651-171">security alert</span><span class="sxs-lookup"><span data-stu-id="84651-171">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="84651-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84651-172">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="84651-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="84651-173">Not supported</span></span> | <span data-ttu-id="84651-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84651-174">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="84651-175">user</span><span class="sxs-lookup"><span data-stu-id="84651-175">user</span></span>](../resources/user.md) | <span data-ttu-id="84651-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-176">User.Read.All</span></span> | <span data-ttu-id="84651-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-177">User.Read.All</span></span> | <span data-ttu-id="84651-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="84651-178">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="84651-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="84651-179">chatMessage</span></span>

<span data-ttu-id="84651-180">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов (**инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="84651-180">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="84651-181">подписки **chatMessage** с разрешениями приложений включают данные ресурсов и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="84651-181">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="84651-182">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="84651-182">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="84651-183">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="84651-183">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="84651-184">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="84651-184">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="84651-185">**Примечание:** `/teams/getAllMessages` и `/chats/getAllMessages` доступны пользователям, у которых есть  
 [необходимые лицензии](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="84651-185">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="84651-186">driveItem</span><span class="sxs-lookup"><span data-stu-id="84651-186">driveItem</span></span>

<span data-ttu-id="84651-187">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="84651-187">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="84651-188">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="84651-188">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="84651-189">В личном хранилище OneDrive можно подписаться на корневую папку или любую подпапку на этом диске.</span><span class="sxs-lookup"><span data-stu-id="84651-189">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="84651-190">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="84651-190">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="84651-191">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="84651-191">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="84651-192">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="84651-192">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="84651-193">контакты, события и сообщения</span><span class="sxs-lookup"><span data-stu-id="84651-193">contact, event, and message</span></span>

<span data-ttu-id="84651-194">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="84651-194">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="84651-195">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="84651-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="84651-196">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="84651-196">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="84651-197">Например, нельзя использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="84651-197">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="84651-198">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="84651-198">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="84651-199">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="84651-199">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="84651-200">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="84651-200">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="84651-201">presence</span><span class="sxs-lookup"><span data-stu-id="84651-201">presence</span></span>

<span data-ttu-id="84651-202">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="84651-202">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="84651-203">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="84651-203">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="84651-204">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84651-204">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="84651-205">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84651-205">Request headers</span></span>

| <span data-ttu-id="84651-206">Имя</span><span class="sxs-lookup"><span data-stu-id="84651-206">Name</span></span>       | <span data-ttu-id="84651-207">Тип</span><span class="sxs-lookup"><span data-stu-id="84651-207">Type</span></span> | <span data-ttu-id="84651-208">Описание</span><span class="sxs-lookup"><span data-stu-id="84651-208">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="84651-209">Authorization</span><span class="sxs-lookup"><span data-stu-id="84651-209">Authorization</span></span>  | <span data-ttu-id="84651-210">string</span><span class="sxs-lookup"><span data-stu-id="84651-210">string</span></span>  | <span data-ttu-id="84651-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84651-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="84651-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="84651-213">Response</span></span>

<span data-ttu-id="84651-214">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84651-214">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="84651-215">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="84651-215">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="84651-216">Пример</span><span class="sxs-lookup"><span data-stu-id="84651-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="84651-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="84651-217">Request</span></span>

<span data-ttu-id="84651-218">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84651-218">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="84651-219">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="84651-219">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="84651-220">Этот запрос создает подписку на уведомления об изменениях новой почты, полученной в текущий момент, когда пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="84651-220">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="84651-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="84651-221">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="84651-222">C#</span><span class="sxs-lookup"><span data-stu-id="84651-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84651-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84651-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84651-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84651-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="84651-225">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84651-225">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="84651-226">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="84651-226">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="84651-227">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="84651-227">Resources examples</span></span>

<span data-ttu-id="84651-228">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="84651-228">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="84651-229">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="84651-229">Resource type</span></span> | <span data-ttu-id="84651-230">Примеры</span><span class="sxs-lookup"><span data-stu-id="84651-230">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="84651-231">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="84651-231">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="84651-232">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="84651-232">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="84651-233">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span><span class="sxs-lookup"><span data-stu-id="84651-233">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span></span> |
|[<span data-ttu-id="84651-234">Контакты</span><span class="sxs-lookup"><span data-stu-id="84651-234">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="84651-235">Беседы</span><span class="sxs-lookup"><span data-stu-id="84651-235">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="84651-236">Drives</span><span class="sxs-lookup"><span data-stu-id="84651-236">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="84651-237">События</span><span class="sxs-lookup"><span data-stu-id="84651-237">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="84651-238">Groups</span><span class="sxs-lookup"><span data-stu-id="84651-238">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="84651-239">List</span><span class="sxs-lookup"><span data-stu-id="84651-239">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="84651-240">Почта</span><span class="sxs-lookup"><span data-stu-id="84651-240">Mail</span></span>](../resources/message.md)|<span data-ttu-id="84651-241">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="84651-241">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="84651-242">Знак</span><span class="sxs-lookup"><span data-stu-id="84651-242">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="84651-243">`/communications/presences/{id}` (один пользователь) `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="84651-243">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="84651-244">Users</span><span class="sxs-lookup"><span data-stu-id="84651-244">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="84651-245">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="84651-245">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="84651-246">**Примечание:** Любой путь, начинающийся с, `me` можно также использовать `users/{id}` вместо `me` целевого определенного пользователя вместо текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="84651-246">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="84651-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="84651-247">Response</span></span>

<span data-ttu-id="84651-248">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84651-248">The following example shows the response.</span></span> 

><span data-ttu-id="84651-p112">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84651-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="84651-251">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="84651-251">Notification endpoint validation</span></span>

<span data-ttu-id="84651-252">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="84651-252">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="84651-253">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="84651-253">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


