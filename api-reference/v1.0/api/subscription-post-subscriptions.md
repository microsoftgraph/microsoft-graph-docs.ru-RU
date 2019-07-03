---
title: Создание подписки
description: Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 1d7b8c65df3aefba65a992d6212d170144f00f2b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450466"
---
# <a name="create-subscription"></a><span data-ttu-id="69ae0-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="69ae0-103">Create subscription</span></span>

<span data-ttu-id="69ae0-104">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69ae0-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="69ae0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69ae0-105">Permissions</span></span>

 <span data-ttu-id="69ae0-106">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="69ae0-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="69ae0-107">Например, чтобы получать уведомления о сообщениях, приложению необходимо разрешение `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="69ae0-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="69ae0-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="69ae0-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="69ae0-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ae0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69ae0-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="69ae0-110">Supported resource</span></span> | <span data-ttu-id="69ae0-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69ae0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69ae0-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69ae0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69ae0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69ae0-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="69ae0-114">contact</span><span class="sxs-lookup"><span data-stu-id="69ae0-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="69ae0-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-115">Contacts.Read</span></span> | <span data-ttu-id="69ae0-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-116">Contacts.Read</span></span> | <span data-ttu-id="69ae0-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-117">Contacts.Read</span></span> |
|<span data-ttu-id="69ae0-118">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="69ae0-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="69ae0-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="69ae0-119">Not supported</span></span> | <span data-ttu-id="69ae0-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69ae0-120">Files.ReadWrite</span></span> | <span data-ttu-id="69ae0-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="69ae0-121">Not supported</span></span> |
|<span data-ttu-id="69ae0-122">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="69ae0-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="69ae0-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="69ae0-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="69ae0-124">Not supported</span></span> | <span data-ttu-id="69ae0-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="69ae0-126">event</span><span class="sxs-lookup"><span data-stu-id="69ae0-126">event</span></span>](../resources/event.md) | <span data-ttu-id="69ae0-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-127">Calendars.Read</span></span> | <span data-ttu-id="69ae0-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-128">Calendars.Read</span></span> | <span data-ttu-id="69ae0-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-129">Calendars.Read</span></span> |
|[<span data-ttu-id="69ae0-130">group</span><span class="sxs-lookup"><span data-stu-id="69ae0-130">group</span></span>](../resources/group.md) | <span data-ttu-id="69ae0-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-131">Group.Read.All</span></span> | <span data-ttu-id="69ae0-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="69ae0-132">Not supported</span></span> | <span data-ttu-id="69ae0-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-133">Group.Read.All</span></span> |
|[<span data-ttu-id="69ae0-134">group conversation</span><span class="sxs-lookup"><span data-stu-id="69ae0-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="69ae0-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-135">Group.Read.All</span></span> | <span data-ttu-id="69ae0-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="69ae0-136">Not supported</span></span> | <span data-ttu-id="69ae0-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="69ae0-137">Not supported</span></span> |
|[<span data-ttu-id="69ae0-138">message</span><span class="sxs-lookup"><span data-stu-id="69ae0-138">message</span></span>](../resources/message.md) | <span data-ttu-id="69ae0-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-139">Mail.Read</span></span> | <span data-ttu-id="69ae0-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-140">Mail.Read</span></span> | <span data-ttu-id="69ae0-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="69ae0-141">Mail.Read</span></span> |
|[<span data-ttu-id="69ae0-142">security alert</span><span class="sxs-lookup"><span data-stu-id="69ae0-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="69ae0-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="69ae0-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="69ae0-144">Not supported</span></span> | <span data-ttu-id="69ae0-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="69ae0-146">user</span><span class="sxs-lookup"><span data-stu-id="69ae0-146">user</span></span>](../resources/user.md) | <span data-ttu-id="69ae0-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-147">User.Read.All</span></span> | <span data-ttu-id="69ae0-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-148">User.Read.All</span></span> | <span data-ttu-id="69ae0-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="69ae0-149">User.Read.All</span></span> |

> <span data-ttu-id="69ae0-150">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="69ae0-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="69ae0-151">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="69ae0-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="69ae0-152">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="69ae0-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="69ae0-153">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="69ae0-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="69ae0-154">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="69ae0-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="69ae0-155">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="69ae0-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="69ae0-156">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="69ae0-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="69ae0-157">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="69ae0-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="69ae0-158">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="69ae0-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="69ae0-159">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="69ae0-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="69ae0-160">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="69ae0-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="69ae0-161">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69ae0-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="69ae0-162">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69ae0-162">Request headers</span></span>

| <span data-ttu-id="69ae0-163">Имя</span><span class="sxs-lookup"><span data-stu-id="69ae0-163">Name</span></span>       | <span data-ttu-id="69ae0-164">Тип</span><span class="sxs-lookup"><span data-stu-id="69ae0-164">Type</span></span> | <span data-ttu-id="69ae0-165">Описание</span><span class="sxs-lookup"><span data-stu-id="69ae0-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69ae0-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="69ae0-166">Authorization</span></span>  | <span data-ttu-id="69ae0-167">string</span><span class="sxs-lookup"><span data-stu-id="69ae0-167">string</span></span>  | <span data-ttu-id="69ae0-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69ae0-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="69ae0-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="69ae0-170">Response</span></span>

<span data-ttu-id="69ae0-171">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="69ae0-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69ae0-172">Пример</span><span class="sxs-lookup"><span data-stu-id="69ae0-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69ae0-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="69ae0-173">Request</span></span>

<span data-ttu-id="69ae0-174">Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="69ae0-174">Here is an example of the request to send a notification when the user receives a new mail.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="69ae0-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="69ae0-175">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="69ae0-176">C#</span><span class="sxs-lookup"><span data-stu-id="69ae0-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69ae0-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69ae0-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69ae0-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69ae0-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="69ae0-179">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69ae0-179">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="69ae0-180">Поле `clientState` является необязательным.</span><span class="sxs-lookup"><span data-stu-id="69ae0-180">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="69ae0-181">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="69ae0-181">Resources examples</span></span>

<span data-ttu-id="69ae0-182">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="69ae0-182">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="69ae0-183">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="69ae0-183">Resource type</span></span> | <span data-ttu-id="69ae0-184">Примеры</span><span class="sxs-lookup"><span data-stu-id="69ae0-184">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="69ae0-185">Mail</span><span class="sxs-lookup"><span data-stu-id="69ae0-185">Mail</span></span>|<span data-ttu-id="69ae0-186">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="69ae0-186">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="69ae0-187">me/messages</span><span class="sxs-lookup"><span data-stu-id="69ae0-187">me/messages</span></span>|
|<span data-ttu-id="69ae0-188">Contacts</span><span class="sxs-lookup"><span data-stu-id="69ae0-188">Contacts</span></span>|<span data-ttu-id="69ae0-189">me/contacts</span><span class="sxs-lookup"><span data-stu-id="69ae0-189">me/contacts</span></span>|
|<span data-ttu-id="69ae0-190">Calendars</span><span class="sxs-lookup"><span data-stu-id="69ae0-190">Calendars</span></span>|<span data-ttu-id="69ae0-191">me/events</span><span class="sxs-lookup"><span data-stu-id="69ae0-191">me/events</span></span>|
|<span data-ttu-id="69ae0-192">Users</span><span class="sxs-lookup"><span data-stu-id="69ae0-192">Users</span></span>|<span data-ttu-id="69ae0-193">users</span><span class="sxs-lookup"><span data-stu-id="69ae0-193">users</span></span>|
|<span data-ttu-id="69ae0-194">Groups</span><span class="sxs-lookup"><span data-stu-id="69ae0-194">Groups</span></span>|<span data-ttu-id="69ae0-195">groups</span><span class="sxs-lookup"><span data-stu-id="69ae0-195">groups</span></span>|
|<span data-ttu-id="69ae0-196">Conversations</span><span class="sxs-lookup"><span data-stu-id="69ae0-196">Conversations</span></span>|<span data-ttu-id="69ae0-197">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="69ae0-197">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="69ae0-198">Drives</span><span class="sxs-lookup"><span data-stu-id="69ae0-198">Drives</span></span>|<span data-ttu-id="69ae0-199">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="69ae0-199">me/drive/root</span></span>|
|<span data-ttu-id="69ae0-200">Security alert</span><span class="sxs-lookup"><span data-stu-id="69ae0-200">Security alert</span></span>|<span data-ttu-id="69ae0-201">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="69ae0-201">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="69ae0-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="69ae0-202">Response</span></span>

<span data-ttu-id="69ae0-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69ae0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="69ae0-206">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="69ae0-206">Notification endpoint validation</span></span>

<span data-ttu-id="69ae0-207">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="69ae0-207">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="69ae0-208">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="69ae0-208">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
