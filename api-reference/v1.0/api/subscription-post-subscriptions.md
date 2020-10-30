---
title: Создание подписки
description: Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменении данных в Microsoft Graph.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f17bac57c20cba3df51274347be202bc3b9d8e21
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782723"
---
# <a name="create-subscription"></a><span data-ttu-id="c2b2f-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="c2b2f-103">Create subscription</span></span>

<span data-ttu-id="c2b2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2b2f-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2b2f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2b2f-106">Permissions</span></span>

 <span data-ttu-id="c2b2f-107">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="c2b2f-108">Например, чтобы получать уведомления об изменениях в сообщениях, приложению необходимо разрешение `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-108">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="c2b2f-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c2b2f-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2b2f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2b2f-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="c2b2f-111">Supported resource</span></span> | <span data-ttu-id="c2b2f-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c2b2f-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2b2f-114">Application</span><span class="sxs-lookup"><span data-stu-id="c2b2f-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="c2b2f-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="c2b2f-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-116">Not supported</span></span> | <span data-ttu-id="c2b2f-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-117">Not supported</span></span> | <span data-ttu-id="c2b2f-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="c2b2f-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="c2b2f-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-120">Not supported</span></span> | <span data-ttu-id="c2b2f-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-121">Not supported</span></span> | <span data-ttu-id="c2b2f-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c2b2f-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="c2b2f-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-124">Not supported</span></span> | <span data-ttu-id="c2b2f-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-125">Not supported</span></span> | <span data-ttu-id="c2b2f-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c2b2f-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="c2b2f-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-128">Not supported</span></span> | <span data-ttu-id="c2b2f-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-129">Not supported</span></span> | <span data-ttu-id="c2b2f-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="c2b2f-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="c2b2f-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-132">Not supported</span></span> | <span data-ttu-id="c2b2f-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-133">Not supported</span></span> | <span data-ttu-id="c2b2f-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="c2b2f-135">contact</span><span class="sxs-lookup"><span data-stu-id="c2b2f-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c2b2f-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-136">Contacts.Read</span></span> | <span data-ttu-id="c2b2f-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-137">Contacts.Read</span></span> | <span data-ttu-id="c2b2f-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-138">Contacts.Read</span></span> |
|<span data-ttu-id="c2b2f-139">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="c2b2f-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-140">Not supported</span></span> | <span data-ttu-id="c2b2f-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2b2f-141">Files.ReadWrite</span></span> | <span data-ttu-id="c2b2f-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-142">Not supported</span></span> |
|<span data-ttu-id="c2b2f-143">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="c2b2f-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="c2b2f-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="c2b2f-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-145">Not supported</span></span> | <span data-ttu-id="c2b2f-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="c2b2f-147">event</span><span class="sxs-lookup"><span data-stu-id="c2b2f-147">event</span></span>](../resources/event.md) | <span data-ttu-id="c2b2f-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-148">Calendars.Read</span></span> | <span data-ttu-id="c2b2f-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-149">Calendars.Read</span></span> | <span data-ttu-id="c2b2f-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-150">Calendars.Read</span></span> |
|[<span data-ttu-id="c2b2f-151">group</span><span class="sxs-lookup"><span data-stu-id="c2b2f-151">group</span></span>](../resources/group.md) | <span data-ttu-id="c2b2f-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-152">Group.Read.All</span></span> | <span data-ttu-id="c2b2f-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-153">Not supported</span></span> | <span data-ttu-id="c2b2f-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-154">Group.Read.All</span></span> |
|[<span data-ttu-id="c2b2f-155">group conversation</span><span class="sxs-lookup"><span data-stu-id="c2b2f-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="c2b2f-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-156">Group.Read.All</span></span> | <span data-ttu-id="c2b2f-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-157">Not supported</span></span> | <span data-ttu-id="c2b2f-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-158">Not supported</span></span> |
|[<span data-ttu-id="c2b2f-159">list</span><span class="sxs-lookup"><span data-stu-id="c2b2f-159">list</span></span>](../resources/list.md) | <span data-ttu-id="c2b2f-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="c2b2f-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-161">Not supported</span></span> | <span data-ttu-id="c2b2f-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="c2b2f-163">message</span><span class="sxs-lookup"><span data-stu-id="c2b2f-163">message</span></span>](../resources/message.md) | <span data-ttu-id="c2b2f-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c2b2f-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c2b2f-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c2b2f-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="c2b2f-167">security alert</span><span class="sxs-lookup"><span data-stu-id="c2b2f-167">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="c2b2f-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-168">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="c2b2f-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2b2f-169">Not supported</span></span> | <span data-ttu-id="c2b2f-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-170">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="c2b2f-171">user</span><span class="sxs-lookup"><span data-stu-id="c2b2f-171">user</span></span>](../resources/user.md) | <span data-ttu-id="c2b2f-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-172">User.Read.All</span></span> | <span data-ttu-id="c2b2f-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-173">User.Read.All</span></span> | <span data-ttu-id="c2b2f-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b2f-174">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="c2b2f-175">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c2b2f-175">chatMessage</span></span>

<span data-ttu-id="c2b2f-176">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="c2b2f-176">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="c2b2f-177">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="c2b2f-177">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="c2b2f-178">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-178">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="c2b2f-179">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c2b2f-179">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="c2b2f-180">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="c2b2f-180">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

> <span data-ttu-id="c2b2f-181">**Примечание.** `/chats/getAllMessages` возвращает только сообщения из чатов, принадлежащих клиенту.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-181">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="c2b2f-182">Если цепочка чата инициирована пользователем из-за пределов клиента, она не принадлежит клиенту и для нее не создаются уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-182">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="c2b2f-183">driveItem</span><span class="sxs-lookup"><span data-stu-id="c2b2f-183">driveItem</span></span>

<span data-ttu-id="c2b2f-184">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-184">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="c2b2f-185">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-185">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="c2b2f-186">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-186">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="c2b2f-187">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-187">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="c2b2f-188">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-188">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="c2b2f-189">Нельзя подписаться на экземпляры **drive** или **driveItem** , не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-189">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="c2b2f-190">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="c2b2f-190">contact, event, and message</span></span>

<span data-ttu-id="c2b2f-191">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-191">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="c2b2f-192">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="c2b2f-193">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-193">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="c2b2f-194">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-194">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="c2b2f-195">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="c2b2f-195">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="c2b2f-196">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-196">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="c2b2f-197">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-197">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="c2b2f-198">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2b2f-198">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="c2b2f-199">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2b2f-199">Request headers</span></span>

| <span data-ttu-id="c2b2f-200">Имя</span><span class="sxs-lookup"><span data-stu-id="c2b2f-200">Name</span></span>       | <span data-ttu-id="c2b2f-201">Тип</span><span class="sxs-lookup"><span data-stu-id="c2b2f-201">Type</span></span> | <span data-ttu-id="c2b2f-202">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b2f-202">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c2b2f-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2b2f-203">Authorization</span></span>  | <span data-ttu-id="c2b2f-204">string</span><span class="sxs-lookup"><span data-stu-id="c2b2f-204">string</span></span>  | <span data-ttu-id="c2b2f-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c2b2f-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b2f-207">Response</span></span>

<span data-ttu-id="c2b2f-208">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-208">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="c2b2f-209">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="c2b2f-209">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="c2b2f-210">Пример</span><span class="sxs-lookup"><span data-stu-id="c2b2f-210">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c2b2f-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2b2f-211">Request</span></span>

<span data-ttu-id="c2b2f-212">Ниже представлен пример запроса на отправку уведомления об изменениях при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-212">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2b2f-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2b2f-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
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
# <a name="c"></a>[<span data-ttu-id="c2b2f-214">C#</span><span class="sxs-lookup"><span data-stu-id="c2b2f-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2b2f-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2b2f-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2b2f-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2b2f-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2b2f-217">Java</span><span class="sxs-lookup"><span data-stu-id="c2b2f-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c2b2f-218">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-218">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="c2b2f-219">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-219">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="c2b2f-220">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="c2b2f-220">Resources examples</span></span>

<span data-ttu-id="c2b2f-221">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-221">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="c2b2f-222">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="c2b2f-222">Resource type</span></span> | <span data-ttu-id="c2b2f-223">Примеры</span><span class="sxs-lookup"><span data-stu-id="c2b2f-223">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="c2b2f-224">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="c2b2f-224">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="c2b2f-225">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="c2b2f-225">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c2b2f-226">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="c2b2f-226">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="c2b2f-227">Контакты</span><span class="sxs-lookup"><span data-stu-id="c2b2f-227">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="c2b2f-228">Беседы</span><span class="sxs-lookup"><span data-stu-id="c2b2f-228">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="c2b2f-229">Диски</span><span class="sxs-lookup"><span data-stu-id="c2b2f-229">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="c2b2f-230">События</span><span class="sxs-lookup"><span data-stu-id="c2b2f-230">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="c2b2f-231">Группы</span><span class="sxs-lookup"><span data-stu-id="c2b2f-231">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="c2b2f-232">Список</span><span class="sxs-lookup"><span data-stu-id="c2b2f-232">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="c2b2f-233">Почта</span><span class="sxs-lookup"><span data-stu-id="c2b2f-233">Mail</span></span>](../resources/message.md)|<span data-ttu-id="c2b2f-234">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="c2b2f-234">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="c2b2f-235">Пользователи</span><span class="sxs-lookup"><span data-stu-id="c2b2f-235">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="c2b2f-236">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="c2b2f-236">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="c2b2f-237">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-237">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="c2b2f-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b2f-238">Response</span></span>

<span data-ttu-id="c2b2f-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2b2f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="c2b2f-242">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="c2b2f-242">Notification endpoint validation</span></span>

<span data-ttu-id="c2b2f-243">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="c2b2f-243">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="c2b2f-244">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="c2b2f-244">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

