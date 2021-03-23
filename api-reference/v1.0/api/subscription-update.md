---
<span data-ttu-id="6f7dd-101">заголовок: описание "Обновление подписки": "Обновление подписки путем продления срока ее действия".</span><span class="sxs-lookup"><span data-stu-id="6f7dd-101">title: "Update subscription" description: "Renew a subscription by extending its expiry time."</span></span>
<span data-ttu-id="6f7dd-102">localization_priority: Обычный автор: "Jumaodhiss" ms.prod: ""change-notifications" doc_type: apiPageType</span><span class="sxs-lookup"><span data-stu-id="6f7dd-102">localization_priority: Normal author: "Jumaodhiss" ms.prod: ""change-notifications" doc_type: apiPageType</span></span>
---

# <a name="update-subscription"></a><span data-ttu-id="6f7dd-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="6f7dd-103">Update subscription</span></span>

<span data-ttu-id="6f7dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f7dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f7dd-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="6f7dd-106">В таблице в разделе [Разрешения](#permissions) перечислены ресурсы, поддерживаюющие подписку на изменение уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="6f7dd-107">Срок действия подписки истекает по истечении времени, которое зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="6f7dd-108">Чтобы избежать пропуска уведомлений об изменениях, приложение должно продлить подписки заблаговременно до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="6f7dd-109">См. [подписку](../resources/subscription.md) на максимальную длину подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f7dd-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f7dd-110">Permissions</span></span>

<span data-ttu-id="6f7dd-111">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6f7dd-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f7dd-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f7dd-113">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="6f7dd-113">Supported resource</span></span> | <span data-ttu-id="6f7dd-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f7dd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6f7dd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f7dd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f7dd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f7dd-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6f7dd-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="6f7dd-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="6f7dd-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-118">Not supported</span></span> | <span data-ttu-id="6f7dd-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-119">Not supported</span></span> | <span data-ttu-id="6f7dd-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="6f7dd-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6f7dd-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6f7dd-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-122">ChannelMessage.Read.All</span></span> | <span data-ttu-id="6f7dd-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-123">Not supported</span></span> |  <span data-ttu-id="6f7dd-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6f7dd-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="6f7dd-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6f7dd-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-126">Not supported</span></span> | <span data-ttu-id="6f7dd-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-127">Not supported</span></span> | <span data-ttu-id="6f7dd-128">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-128">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6f7dd-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6f7dd-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6f7dd-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-130">Not supported</span></span> | <span data-ttu-id="6f7dd-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-131">Not supported</span></span> | <span data-ttu-id="6f7dd-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-132">Chat.Read.All</span></span>  |
|<span data-ttu-id="6f7dd-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="6f7dd-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6f7dd-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-134">Not supported</span></span> | <span data-ttu-id="6f7dd-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-135">Not supported</span></span> | <span data-ttu-id="6f7dd-136">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-136">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6f7dd-137">contact</span><span class="sxs-lookup"><span data-stu-id="6f7dd-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6f7dd-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-138">Contacts.Read</span></span> | <span data-ttu-id="6f7dd-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-139">Contacts.Read</span></span> | <span data-ttu-id="6f7dd-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-140">Contacts.Read</span></span> |
|<span data-ttu-id="6f7dd-141">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="6f7dd-141">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6f7dd-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-142">Not supported</span></span> | <span data-ttu-id="6f7dd-143">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f7dd-143">Files.ReadWrite</span></span> | <span data-ttu-id="6f7dd-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-144">Not supported</span></span> |
|<span data-ttu-id="6f7dd-145">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6f7dd-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6f7dd-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-146">Files.ReadWrite.All</span></span> | <span data-ttu-id="6f7dd-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-147">Not supported</span></span> | <span data-ttu-id="6f7dd-148">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-148">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6f7dd-149">event</span><span class="sxs-lookup"><span data-stu-id="6f7dd-149">event</span></span>](../resources/event.md) | <span data-ttu-id="6f7dd-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-150">Calendars.Read</span></span> | <span data-ttu-id="6f7dd-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-151">Calendars.Read</span></span> | <span data-ttu-id="6f7dd-152">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-152">Calendars.Read</span></span> |
|[<span data-ttu-id="6f7dd-153">group</span><span class="sxs-lookup"><span data-stu-id="6f7dd-153">group</span></span>](../resources/group.md) | <span data-ttu-id="6f7dd-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-154">Group.Read.All</span></span> | <span data-ttu-id="6f7dd-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-155">Not supported</span></span> | <span data-ttu-id="6f7dd-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-156">Group.Read.All</span></span> |
|[<span data-ttu-id="6f7dd-157">group conversation</span><span class="sxs-lookup"><span data-stu-id="6f7dd-157">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6f7dd-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-158">Group.Read.All</span></span> | <span data-ttu-id="6f7dd-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-159">Not supported</span></span> | <span data-ttu-id="6f7dd-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-160">Not supported</span></span> |
|[<span data-ttu-id="6f7dd-161">list</span><span class="sxs-lookup"><span data-stu-id="6f7dd-161">list</span></span>](../resources/list.md) | <span data-ttu-id="6f7dd-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-162">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6f7dd-163">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-163">Not supported</span></span> | <span data-ttu-id="6f7dd-164">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-164">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6f7dd-165">message</span><span class="sxs-lookup"><span data-stu-id="6f7dd-165">message</span></span>](../resources/message.md) | <span data-ttu-id="6f7dd-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6f7dd-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-167">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6f7dd-168">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6f7dd-168">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6f7dd-169">printer</span><span class="sxs-lookup"><span data-stu-id="6f7dd-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="6f7dd-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-170">Not supported</span></span> | <span data-ttu-id="6f7dd-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-171">Not supported</span></span> | <span data-ttu-id="6f7dd-172">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="6f7dd-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6f7dd-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="6f7dd-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-174">Not supported</span></span> | <span data-ttu-id="6f7dd-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-175">Not supported</span></span> | <span data-ttu-id="6f7dd-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="6f7dd-177">security alert</span><span class="sxs-lookup"><span data-stu-id="6f7dd-177">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6f7dd-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6f7dd-179">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f7dd-179">Not supported</span></span> | <span data-ttu-id="6f7dd-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6f7dd-181">user</span><span class="sxs-lookup"><span data-stu-id="6f7dd-181">user</span></span>](../resources/user.md) | <span data-ttu-id="6f7dd-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-182">User.Read.All</span></span> | <span data-ttu-id="6f7dd-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-183">User.Read.All</span></span> | <span data-ttu-id="6f7dd-184">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7dd-184">User.Read.All</span></span> |

> <span data-ttu-id="6f7dd-185">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="6f7dd-185">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="6f7dd-186">driveItem</span><span class="sxs-lookup"><span data-stu-id="6f7dd-186">driveItem</span></span>

<span data-ttu-id="6f7dd-187">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-187">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="6f7dd-188">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-188">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6f7dd-189">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-189">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6f7dd-190">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-190">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6f7dd-191">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-191">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6f7dd-192">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-192">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6f7dd-193">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="6f7dd-193">contact, event, and message</span></span>

<span data-ttu-id="6f7dd-194">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-194">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6f7dd-195">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6f7dd-196">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-196">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6f7dd-197">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-197">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6f7dd-198">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="6f7dd-198">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6f7dd-199">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-199">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6f7dd-200">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-200">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="6f7dd-201">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f7dd-201">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6f7dd-202">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f7dd-202">Request headers</span></span>

| <span data-ttu-id="6f7dd-203">Имя</span><span class="sxs-lookup"><span data-stu-id="6f7dd-203">Name</span></span>       | <span data-ttu-id="6f7dd-204">Тип</span><span class="sxs-lookup"><span data-stu-id="6f7dd-204">Type</span></span> | <span data-ttu-id="6f7dd-205">Описание</span><span class="sxs-lookup"><span data-stu-id="6f7dd-205">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6f7dd-206">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f7dd-206">Authorization</span></span>  | <span data-ttu-id="6f7dd-207">string</span><span class="sxs-lookup"><span data-stu-id="6f7dd-207">string</span></span>  | <span data-ttu-id="6f7dd-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6f7dd-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f7dd-210">Response</span></span>

<span data-ttu-id="6f7dd-211">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-211">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="6f7dd-212">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="6f7dd-212">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="6f7dd-213">Пример</span><span class="sxs-lookup"><span data-stu-id="6f7dd-213">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6f7dd-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f7dd-214">Request</span></span>

<span data-ttu-id="6f7dd-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-215">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f7dd-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f7dd-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="6f7dd-217">C#</span><span class="sxs-lookup"><span data-stu-id="6f7dd-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f7dd-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f7dd-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f7dd-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f7dd-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f7dd-220">Java</span><span class="sxs-lookup"><span data-stu-id="6f7dd-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6f7dd-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f7dd-221">Response</span></span>

<span data-ttu-id="6f7dd-222">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f7dd-222">Here is an example of the response.</span></span>
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
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false,
  "notificationContentType": "application/json"
}
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

