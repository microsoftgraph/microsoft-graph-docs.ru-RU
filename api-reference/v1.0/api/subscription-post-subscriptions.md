---
<span data-ttu-id="2c0ae-101">заголовок: описание "Создание подписки": "Подписывает приложение-прослушиватель для получения уведомлений об изменениях при изменении данных в Microsoft Graph".</span><span class="sxs-lookup"><span data-stu-id="2c0ae-101">title: "Create subscription" description: "Subscribes a listener application to receive change notifications when data on the Microsoft Graph changes."</span></span>
<span data-ttu-id="2c0ae-102">localization_priority. Автор приоритета: "Jumaodhiss" ms.prod: "change-notifications" doc_type: apiPageType</span><span class="sxs-lookup"><span data-stu-id="2c0ae-102">localization_priority: Priority author: "Jumaodhiss" ms.prod: ""change-notifications" doc_type: apiPageType</span></span>
---

# <a name="create-subscription"></a><span data-ttu-id="2c0ae-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="2c0ae-103">Create subscription</span></span>

<span data-ttu-id="2c0ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c0ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c0ae-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="2c0ae-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="2c0ae-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c0ae-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c0ae-107">Permissions</span></span>

<span data-ttu-id="2c0ae-108">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-108">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="2c0ae-109">Например, чтобы получать уведомления об изменениях в сообщениях, приложению необходимо разрешение `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-109">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
<span data-ttu-id="2c0ae-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2c0ae-111">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c0ae-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c0ae-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="2c0ae-112">Supported resource</span></span> | <span data-ttu-id="2c0ae-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2c0ae-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c0ae-115">Application</span><span class="sxs-lookup"><span data-stu-id="2c0ae-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="2c0ae-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="2c0ae-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-117">Not supported</span></span> | <span data-ttu-id="2c0ae-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-118">Not supported</span></span> | <span data-ttu-id="2c0ae-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="2c0ae-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="2c0ae-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-121">ChannelMessage.Read.All</span></span> | <span data-ttu-id="2c0ae-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-122">Not supported</span></span> |  <span data-ttu-id="2c0ae-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2c0ae-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="2c0ae-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-125">Not supported</span></span> | <span data-ttu-id="2c0ae-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-126">Not supported</span></span> | <span data-ttu-id="2c0ae-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2c0ae-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="2c0ae-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-129">Not supported</span></span> | <span data-ttu-id="2c0ae-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-130">Not supported</span></span> | <span data-ttu-id="2c0ae-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="2c0ae-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="2c0ae-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-133">Not supported</span></span> | <span data-ttu-id="2c0ae-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-134">Not supported</span></span> | <span data-ttu-id="2c0ae-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="2c0ae-136">contact</span><span class="sxs-lookup"><span data-stu-id="2c0ae-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2c0ae-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-137">Contacts.Read</span></span> | <span data-ttu-id="2c0ae-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-138">Contacts.Read</span></span> | <span data-ttu-id="2c0ae-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-139">Contacts.Read</span></span> |
|<span data-ttu-id="2c0ae-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2c0ae-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-141">Not supported</span></span> | <span data-ttu-id="2c0ae-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c0ae-142">Files.ReadWrite</span></span> | <span data-ttu-id="2c0ae-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-143">Not supported</span></span> |
|<span data-ttu-id="2c0ae-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="2c0ae-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2c0ae-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="2c0ae-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-146">Not supported</span></span> | <span data-ttu-id="2c0ae-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2c0ae-148">event</span><span class="sxs-lookup"><span data-stu-id="2c0ae-148">event</span></span>](../resources/event.md) | <span data-ttu-id="2c0ae-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-149">Calendars.Read</span></span> | <span data-ttu-id="2c0ae-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-150">Calendars.Read</span></span> | <span data-ttu-id="2c0ae-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-151">Calendars.Read</span></span> |
|[<span data-ttu-id="2c0ae-152">group</span><span class="sxs-lookup"><span data-stu-id="2c0ae-152">group</span></span>](../resources/group.md) | <span data-ttu-id="2c0ae-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-153">Group.Read.All</span></span> | <span data-ttu-id="2c0ae-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-154">Not supported</span></span> | <span data-ttu-id="2c0ae-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-155">Group.Read.All</span></span> |
|[<span data-ttu-id="2c0ae-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="2c0ae-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2c0ae-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-157">Group.Read.All</span></span> | <span data-ttu-id="2c0ae-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-158">Not supported</span></span> | <span data-ttu-id="2c0ae-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-159">Not supported</span></span> |
|[<span data-ttu-id="2c0ae-160">list</span><span class="sxs-lookup"><span data-stu-id="2c0ae-160">list</span></span>](../resources/list.md) | <span data-ttu-id="2c0ae-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="2c0ae-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-162">Not supported</span></span> | <span data-ttu-id="2c0ae-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="2c0ae-164">message</span><span class="sxs-lookup"><span data-stu-id="2c0ae-164">message</span></span>](../resources/message.md) | <span data-ttu-id="2c0ae-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2c0ae-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2c0ae-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2c0ae-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="2c0ae-168">printer</span><span class="sxs-lookup"><span data-stu-id="2c0ae-168">printer</span></span>](../resources/printer.md) | <span data-ttu-id="2c0ae-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-169">Not supported</span></span> | <span data-ttu-id="2c0ae-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-170">Not supported</span></span> | <span data-ttu-id="2c0ae-171">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-171">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="2c0ae-172">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="2c0ae-172">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="2c0ae-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-173">Not supported</span></span> | <span data-ttu-id="2c0ae-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-174">Not supported</span></span> | <span data-ttu-id="2c0ae-175">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-175">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="2c0ae-176">security alert</span><span class="sxs-lookup"><span data-stu-id="2c0ae-176">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="2c0ae-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-177">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2c0ae-178">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2c0ae-178">Not supported</span></span> | <span data-ttu-id="2c0ae-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-179">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="2c0ae-180">user</span><span class="sxs-lookup"><span data-stu-id="2c0ae-180">user</span></span>](../resources/user.md) | <span data-ttu-id="2c0ae-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-181">User.Read.All</span></span> | <span data-ttu-id="2c0ae-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-182">User.Read.All</span></span> | <span data-ttu-id="2c0ae-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c0ae-183">User.Read.All</span></span> |

> <span data-ttu-id="2c0ae-184">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="2c0ae-184">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="2c0ae-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="2c0ae-185">driveItem</span></span>

<span data-ttu-id="2c0ae-186">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="2c0ae-187">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="2c0ae-188">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2c0ae-189">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2c0ae-190">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="2c0ae-191">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="2c0ae-192">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="2c0ae-192">contact, event, and message</span></span>

<span data-ttu-id="2c0ae-193">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-193">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="2c0ae-194">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="2c0ae-195">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-195">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2c0ae-196">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-196">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="2c0ae-197">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="2c0ae-197">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2c0ae-198">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-198">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2c0ae-199">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-199">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="2c0ae-200">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c0ae-200">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="2c0ae-201">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c0ae-201">Request headers</span></span>

| <span data-ttu-id="2c0ae-202">Имя</span><span class="sxs-lookup"><span data-stu-id="2c0ae-202">Name</span></span>       | <span data-ttu-id="2c0ae-203">Тип</span><span class="sxs-lookup"><span data-stu-id="2c0ae-203">Type</span></span> | <span data-ttu-id="2c0ae-204">Описание</span><span class="sxs-lookup"><span data-stu-id="2c0ae-204">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2c0ae-205">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c0ae-205">Authorization</span></span>  | <span data-ttu-id="2c0ae-206">string</span><span class="sxs-lookup"><span data-stu-id="2c0ae-206">string</span></span>  | <span data-ttu-id="2c0ae-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2c0ae-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c0ae-209">Response</span></span>

<span data-ttu-id="2c0ae-210">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-210">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="2c0ae-211">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="2c0ae-211">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="2c0ae-212">Пример</span><span class="sxs-lookup"><span data-stu-id="2c0ae-212">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2c0ae-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c0ae-213">Request</span></span>

<span data-ttu-id="2c0ae-214">Ниже представлен пример запроса на отправку уведомления об изменениях при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-214">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c0ae-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c0ae-215">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c0ae-216">C#</span><span class="sxs-lookup"><span data-stu-id="2c0ae-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c0ae-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c0ae-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c0ae-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c0ae-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c0ae-219">Java</span><span class="sxs-lookup"><span data-stu-id="2c0ae-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2c0ae-220">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-220">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="2c0ae-221">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-221">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="2c0ae-222">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="2c0ae-222">Resources examples</span></span>

<span data-ttu-id="2c0ae-223">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-223">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="2c0ae-224">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="2c0ae-224">Resource type</span></span> | <span data-ttu-id="2c0ae-225">Примеры</span><span class="sxs-lookup"><span data-stu-id="2c0ae-225">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="2c0ae-226">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="2c0ae-226">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="2c0ae-227">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="2c0ae-227">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2c0ae-228">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="2c0ae-228">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="2c0ae-229">Контакты</span><span class="sxs-lookup"><span data-stu-id="2c0ae-229">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="2c0ae-230">Беседы</span><span class="sxs-lookup"><span data-stu-id="2c0ae-230">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="2c0ae-231">Диски</span><span class="sxs-lookup"><span data-stu-id="2c0ae-231">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="2c0ae-232">События</span><span class="sxs-lookup"><span data-stu-id="2c0ae-232">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="2c0ae-233">Группы</span><span class="sxs-lookup"><span data-stu-id="2c0ae-233">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="2c0ae-234">Список</span><span class="sxs-lookup"><span data-stu-id="2c0ae-234">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="2c0ae-235">Почта</span><span class="sxs-lookup"><span data-stu-id="2c0ae-235">Mail</span></span>](../resources/message.md)|<span data-ttu-id="2c0ae-236">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="2c0ae-236">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="2c0ae-237">printer</span><span class="sxs-lookup"><span data-stu-id="2c0ae-237">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="2c0ae-238">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="2c0ae-238">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="2c0ae-239">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="2c0ae-239">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|
|<span data-ttu-id="2c0ae-240">[пользователи](../resources/user.md);</span><span class="sxs-lookup"><span data-stu-id="2c0ae-240">[Users](../resources/user.md)</span></span>|`users`|

> <span data-ttu-id="2c0ae-241">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-241">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="2c0ae-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c0ae-242">Response</span></span>

<span data-ttu-id="2c0ae-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c0ae-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="2c0ae-246">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="2c0ae-246">Notification endpoint validation</span></span>

<span data-ttu-id="2c0ae-247">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="2c0ae-247">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="2c0ae-248">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="2c0ae-248">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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

