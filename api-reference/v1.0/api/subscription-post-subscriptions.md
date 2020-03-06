---
title: Создание подписки
description: Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 98825de41285bb3bfe210654ee3991b100dc5407
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509733"
---
# <a name="create-subscription"></a><span data-ttu-id="05b61-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="05b61-103">Create subscription</span></span>

<span data-ttu-id="05b61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05b61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05b61-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="05b61-105">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="05b61-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05b61-106">Permissions</span></span>

 <span data-ttu-id="05b61-107">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="05b61-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="05b61-108">Например, чтобы получать уведомления о сообщениях, приложению необходимо разрешение `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="05b61-108">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="05b61-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="05b61-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="05b61-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05b61-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05b61-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="05b61-111">Supported resource</span></span> | <span data-ttu-id="05b61-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05b61-112">Delegated (work or school account)</span></span> | <span data-ttu-id="05b61-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05b61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05b61-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05b61-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="05b61-115">contact</span><span class="sxs-lookup"><span data-stu-id="05b61-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="05b61-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-116">Contacts.Read</span></span> | <span data-ttu-id="05b61-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-117">Contacts.Read</span></span> | <span data-ttu-id="05b61-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-118">Contacts.Read</span></span> |
|<span data-ttu-id="05b61-119">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="05b61-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="05b61-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05b61-120">Not supported</span></span> | <span data-ttu-id="05b61-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05b61-121">Files.ReadWrite</span></span> | <span data-ttu-id="05b61-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05b61-122">Not supported</span></span> |
|<span data-ttu-id="05b61-123">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="05b61-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="05b61-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b61-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="05b61-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05b61-125">Not supported</span></span> | <span data-ttu-id="05b61-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b61-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="05b61-127">event</span><span class="sxs-lookup"><span data-stu-id="05b61-127">event</span></span>](../resources/event.md) | <span data-ttu-id="05b61-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-128">Calendars.Read</span></span> | <span data-ttu-id="05b61-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-129">Calendars.Read</span></span> | <span data-ttu-id="05b61-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-130">Calendars.Read</span></span> |
|[<span data-ttu-id="05b61-131">group</span><span class="sxs-lookup"><span data-stu-id="05b61-131">group</span></span>](../resources/group.md) | <span data-ttu-id="05b61-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="05b61-132">Group.Read.All</span></span> | <span data-ttu-id="05b61-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05b61-133">Not supported</span></span> | <span data-ttu-id="05b61-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="05b61-134">Group.Read.All</span></span> |
|[<span data-ttu-id="05b61-135">group conversation</span><span class="sxs-lookup"><span data-stu-id="05b61-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="05b61-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="05b61-136">Group.Read.All</span></span> | <span data-ttu-id="05b61-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05b61-137">Not supported</span></span> | <span data-ttu-id="05b61-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05b61-138">Not supported</span></span> |
|[<span data-ttu-id="05b61-139">message</span><span class="sxs-lookup"><span data-stu-id="05b61-139">message</span></span>](../resources/message.md) | <span data-ttu-id="05b61-140">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-140">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="05b61-141">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-141">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="05b61-142">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="05b61-142">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="05b61-143">security alert</span><span class="sxs-lookup"><span data-stu-id="05b61-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="05b61-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b61-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="05b61-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="05b61-145">Not supported</span></span> | <span data-ttu-id="05b61-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b61-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="05b61-147">user</span><span class="sxs-lookup"><span data-stu-id="05b61-147">user</span></span>](../resources/user.md) | <span data-ttu-id="05b61-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="05b61-148">User.Read.All</span></span> | <span data-ttu-id="05b61-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="05b61-149">User.Read.All</span></span> | <span data-ttu-id="05b61-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="05b61-150">User.Read.All</span></span> |

> <span data-ttu-id="05b61-151">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="05b61-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="05b61-152">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="05b61-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="05b61-153">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="05b61-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="05b61-154">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="05b61-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="05b61-155">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="05b61-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="05b61-156">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="05b61-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="05b61-157">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="05b61-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="05b61-158">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="05b61-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="05b61-159">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="05b61-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="05b61-160">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="05b61-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="05b61-161">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="05b61-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="05b61-162">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05b61-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="05b61-163">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05b61-163">Request headers</span></span>

| <span data-ttu-id="05b61-164">Имя</span><span class="sxs-lookup"><span data-stu-id="05b61-164">Name</span></span>       | <span data-ttu-id="05b61-165">Тип</span><span class="sxs-lookup"><span data-stu-id="05b61-165">Type</span></span> | <span data-ttu-id="05b61-166">Описание</span><span class="sxs-lookup"><span data-stu-id="05b61-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="05b61-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="05b61-167">Authorization</span></span>  | <span data-ttu-id="05b61-168">string</span><span class="sxs-lookup"><span data-stu-id="05b61-168">string</span></span>  | <span data-ttu-id="05b61-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05b61-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="05b61-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b61-171">Response</span></span>

<span data-ttu-id="05b61-172">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05b61-172">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05b61-173">Пример</span><span class="sxs-lookup"><span data-stu-id="05b61-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="05b61-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="05b61-174">Request</span></span>

<span data-ttu-id="05b61-175">Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="05b61-175">Here is an example of the request to send a notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="05b61-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="05b61-176">HTTP</span></span>](#tab/http)
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
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="05b61-177">C#</span><span class="sxs-lookup"><span data-stu-id="05b61-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05b61-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05b61-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05b61-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05b61-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05b61-180">Java</span><span class="sxs-lookup"><span data-stu-id="05b61-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="05b61-181">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05b61-181">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="05b61-182">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="05b61-182">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="05b61-183">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="05b61-183">Resources examples</span></span>

<span data-ttu-id="05b61-184">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="05b61-184">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="05b61-185">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="05b61-185">Resource type</span></span> | <span data-ttu-id="05b61-186">Примеры</span><span class="sxs-lookup"><span data-stu-id="05b61-186">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="05b61-187">Mail</span><span class="sxs-lookup"><span data-stu-id="05b61-187">Mail</span></span>|<span data-ttu-id="05b61-188">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="05b61-188">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="05b61-189">me/messages</span><span class="sxs-lookup"><span data-stu-id="05b61-189">me/messages</span></span>|
|<span data-ttu-id="05b61-190">Contacts</span><span class="sxs-lookup"><span data-stu-id="05b61-190">Contacts</span></span>|<span data-ttu-id="05b61-191">me/contacts</span><span class="sxs-lookup"><span data-stu-id="05b61-191">me/contacts</span></span>|
|<span data-ttu-id="05b61-192">Calendars</span><span class="sxs-lookup"><span data-stu-id="05b61-192">Calendars</span></span>|<span data-ttu-id="05b61-193">me/events</span><span class="sxs-lookup"><span data-stu-id="05b61-193">me/events</span></span>|
|<span data-ttu-id="05b61-194">Users</span><span class="sxs-lookup"><span data-stu-id="05b61-194">Users</span></span>|<span data-ttu-id="05b61-195">users</span><span class="sxs-lookup"><span data-stu-id="05b61-195">users</span></span>|
|<span data-ttu-id="05b61-196">Groups</span><span class="sxs-lookup"><span data-stu-id="05b61-196">Groups</span></span>|<span data-ttu-id="05b61-197">groups</span><span class="sxs-lookup"><span data-stu-id="05b61-197">groups</span></span>|
|<span data-ttu-id="05b61-198">Conversations</span><span class="sxs-lookup"><span data-stu-id="05b61-198">Conversations</span></span>|<span data-ttu-id="05b61-199">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="05b61-199">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="05b61-200">Drives</span><span class="sxs-lookup"><span data-stu-id="05b61-200">Drives</span></span>|<span data-ttu-id="05b61-201">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="05b61-201">me/drive/root</span></span>|
|<span data-ttu-id="05b61-202">Security alert</span><span class="sxs-lookup"><span data-stu-id="05b61-202">Security alert</span></span>|<span data-ttu-id="05b61-203">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="05b61-203">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="05b61-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b61-204">Response</span></span>

<span data-ttu-id="05b61-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05b61-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="05b61-208">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="05b61-208">Notification endpoint validation</span></span>

<span data-ttu-id="05b61-209">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="05b61-209">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="05b61-210">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="05b61-210">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
