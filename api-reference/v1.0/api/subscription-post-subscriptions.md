---
title: Создание подписки
description: Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 801a6d99d467207a1cd6791219eb1bf6fa3290d6
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216239"
---
# <a name="create-subscription"></a><span data-ttu-id="e3048-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="e3048-103">Create subscription</span></span>

<span data-ttu-id="e3048-104">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e3048-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3048-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3048-105">Permissions</span></span>

 <span data-ttu-id="e3048-106">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e3048-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="e3048-107">Например, чтобы получать уведомления о сообщениях, приложению необходимо разрешение `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="e3048-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="e3048-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e3048-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e3048-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3048-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3048-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="e3048-110">Supported resource</span></span> | <span data-ttu-id="e3048-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3048-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e3048-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3048-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3048-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3048-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="e3048-114">contact</span><span class="sxs-lookup"><span data-stu-id="e3048-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e3048-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-115">Contacts.Read</span></span> | <span data-ttu-id="e3048-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-116">Contacts.Read</span></span> | <span data-ttu-id="e3048-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-117">Contacts.Read</span></span> |
|<span data-ttu-id="e3048-118">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="e3048-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="e3048-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3048-119">Not supported</span></span> | <span data-ttu-id="e3048-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3048-120">Files.ReadWrite</span></span> | <span data-ttu-id="e3048-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3048-121">Not supported</span></span> |
|<span data-ttu-id="e3048-122">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="e3048-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="e3048-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3048-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="e3048-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3048-124">Not supported</span></span> | <span data-ttu-id="e3048-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3048-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="e3048-126">event</span><span class="sxs-lookup"><span data-stu-id="e3048-126">event</span></span>](../resources/event.md) | <span data-ttu-id="e3048-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-127">Calendars.Read</span></span> | <span data-ttu-id="e3048-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-128">Calendars.Read</span></span> | <span data-ttu-id="e3048-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-129">Calendars.Read</span></span> |
|[<span data-ttu-id="e3048-130">group</span><span class="sxs-lookup"><span data-stu-id="e3048-130">group</span></span>](../resources/group.md) | <span data-ttu-id="e3048-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3048-131">Group.Read.All</span></span> | <span data-ttu-id="e3048-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3048-132">Not supported</span></span> | <span data-ttu-id="e3048-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3048-133">Group.Read.All</span></span> |
|[<span data-ttu-id="e3048-134">group conversation</span><span class="sxs-lookup"><span data-stu-id="e3048-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="e3048-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3048-135">Group.Read.All</span></span> | <span data-ttu-id="e3048-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3048-136">Not supported</span></span> | <span data-ttu-id="e3048-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3048-137">Not supported</span></span> |
|[<span data-ttu-id="e3048-138">message</span><span class="sxs-lookup"><span data-stu-id="e3048-138">message</span></span>](../resources/message.md) | <span data-ttu-id="e3048-139">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-139">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e3048-140">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-140">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="e3048-141">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3048-141">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="e3048-142">security alert</span><span class="sxs-lookup"><span data-stu-id="e3048-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="e3048-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3048-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="e3048-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3048-144">Not supported</span></span> | <span data-ttu-id="e3048-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3048-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="e3048-146">user</span><span class="sxs-lookup"><span data-stu-id="e3048-146">user</span></span>](../resources/user.md) | <span data-ttu-id="e3048-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3048-147">User.Read.All</span></span> | <span data-ttu-id="e3048-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3048-148">User.Read.All</span></span> | <span data-ttu-id="e3048-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3048-149">User.Read.All</span></span> |

> <span data-ttu-id="e3048-150">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="e3048-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="e3048-151">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="e3048-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="e3048-152">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="e3048-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="e3048-153">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="e3048-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="e3048-154">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="e3048-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="e3048-155">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="e3048-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="e3048-156">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="e3048-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="e3048-157">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="e3048-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="e3048-158">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="e3048-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="e3048-159">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e3048-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="e3048-160">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="e3048-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="e3048-161">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3048-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="e3048-162">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3048-162">Request headers</span></span>

| <span data-ttu-id="e3048-163">Имя</span><span class="sxs-lookup"><span data-stu-id="e3048-163">Name</span></span>       | <span data-ttu-id="e3048-164">Тип</span><span class="sxs-lookup"><span data-stu-id="e3048-164">Type</span></span> | <span data-ttu-id="e3048-165">Описание</span><span class="sxs-lookup"><span data-stu-id="e3048-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e3048-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3048-166">Authorization</span></span>  | <span data-ttu-id="e3048-167">string</span><span class="sxs-lookup"><span data-stu-id="e3048-167">string</span></span>  | <span data-ttu-id="e3048-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3048-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e3048-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3048-170">Response</span></span>

<span data-ttu-id="e3048-171">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3048-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3048-172">Пример</span><span class="sxs-lookup"><span data-stu-id="e3048-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e3048-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3048-173">Request</span></span>

<span data-ttu-id="e3048-174">Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="e3048-174">Here is an example of the request to send a notification when the user receives a new mail.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e3048-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3048-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3048-176">C#</span><span class="sxs-lookup"><span data-stu-id="e3048-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3048-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3048-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3048-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3048-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e3048-179">Java</span><span class="sxs-lookup"><span data-stu-id="e3048-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e3048-180">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3048-180">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="e3048-181">Поле `clientState` является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e3048-181">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="e3048-182">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="e3048-182">Resources examples</span></span>

<span data-ttu-id="e3048-183">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="e3048-183">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="e3048-184">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="e3048-184">Resource type</span></span> | <span data-ttu-id="e3048-185">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3048-185">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="e3048-186">Mail</span><span class="sxs-lookup"><span data-stu-id="e3048-186">Mail</span></span>|<span data-ttu-id="e3048-187">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="e3048-187">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="e3048-188">me/messages</span><span class="sxs-lookup"><span data-stu-id="e3048-188">me/messages</span></span>|
|<span data-ttu-id="e3048-189">Contacts</span><span class="sxs-lookup"><span data-stu-id="e3048-189">Contacts</span></span>|<span data-ttu-id="e3048-190">me/contacts</span><span class="sxs-lookup"><span data-stu-id="e3048-190">me/contacts</span></span>|
|<span data-ttu-id="e3048-191">Calendars</span><span class="sxs-lookup"><span data-stu-id="e3048-191">Calendars</span></span>|<span data-ttu-id="e3048-192">me/events</span><span class="sxs-lookup"><span data-stu-id="e3048-192">me/events</span></span>|
|<span data-ttu-id="e3048-193">Users</span><span class="sxs-lookup"><span data-stu-id="e3048-193">Users</span></span>|<span data-ttu-id="e3048-194">users</span><span class="sxs-lookup"><span data-stu-id="e3048-194">users</span></span>|
|<span data-ttu-id="e3048-195">Groups</span><span class="sxs-lookup"><span data-stu-id="e3048-195">Groups</span></span>|<span data-ttu-id="e3048-196">groups</span><span class="sxs-lookup"><span data-stu-id="e3048-196">groups</span></span>|
|<span data-ttu-id="e3048-197">Conversations</span><span class="sxs-lookup"><span data-stu-id="e3048-197">Conversations</span></span>|<span data-ttu-id="e3048-198">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="e3048-198">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="e3048-199">Drives</span><span class="sxs-lookup"><span data-stu-id="e3048-199">Drives</span></span>|<span data-ttu-id="e3048-200">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="e3048-200">me/drive/root</span></span>|
|<span data-ttu-id="e3048-201">Security alert</span><span class="sxs-lookup"><span data-stu-id="e3048-201">Security alert</span></span>|<span data-ttu-id="e3048-202">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="e3048-202">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="e3048-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3048-203">Response</span></span>

<span data-ttu-id="e3048-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3048-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="e3048-207">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="e3048-207">Notification endpoint validation</span></span>

<span data-ttu-id="e3048-208">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="e3048-208">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="e3048-209">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="e3048-209">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
