---
title: Создание подписки
description: Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 05914a1014e9d635da8d38927e207a5c17823c93
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543431"
---
# <a name="create-subscription"></a><span data-ttu-id="682f8-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="682f8-103">Create subscription</span></span>

<span data-ttu-id="682f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="682f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="682f8-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="682f8-105">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="682f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="682f8-106">Permissions</span></span>

 <span data-ttu-id="682f8-107">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="682f8-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="682f8-108">Например, чтобы получать уведомления о сообщениях, приложению необходимо разрешение `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="682f8-108">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="682f8-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="682f8-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="682f8-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="682f8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="682f8-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="682f8-111">Supported resource</span></span> | <span data-ttu-id="682f8-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="682f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="682f8-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="682f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="682f8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="682f8-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="682f8-115">contact</span><span class="sxs-lookup"><span data-stu-id="682f8-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="682f8-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-116">Contacts.Read</span></span> | <span data-ttu-id="682f8-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-117">Contacts.Read</span></span> | <span data-ttu-id="682f8-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-118">Contacts.Read</span></span> |
|<span data-ttu-id="682f8-119">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="682f8-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="682f8-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="682f8-120">Not supported</span></span> | <span data-ttu-id="682f8-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="682f8-121">Files.ReadWrite</span></span> | <span data-ttu-id="682f8-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="682f8-122">Not supported</span></span> |
|<span data-ttu-id="682f8-123">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="682f8-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="682f8-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682f8-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="682f8-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="682f8-125">Not supported</span></span> | <span data-ttu-id="682f8-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682f8-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="682f8-127">event</span><span class="sxs-lookup"><span data-stu-id="682f8-127">event</span></span>](../resources/event.md) | <span data-ttu-id="682f8-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-128">Calendars.Read</span></span> | <span data-ttu-id="682f8-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-129">Calendars.Read</span></span> | <span data-ttu-id="682f8-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-130">Calendars.Read</span></span> |
|[<span data-ttu-id="682f8-131">group</span><span class="sxs-lookup"><span data-stu-id="682f8-131">group</span></span>](../resources/group.md) | <span data-ttu-id="682f8-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="682f8-132">Group.Read.All</span></span> | <span data-ttu-id="682f8-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="682f8-133">Not supported</span></span> | <span data-ttu-id="682f8-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="682f8-134">Group.Read.All</span></span> |
|[<span data-ttu-id="682f8-135">group conversation</span><span class="sxs-lookup"><span data-stu-id="682f8-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="682f8-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="682f8-136">Group.Read.All</span></span> | <span data-ttu-id="682f8-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="682f8-137">Not supported</span></span> | <span data-ttu-id="682f8-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="682f8-138">Not supported</span></span> |
|[<span data-ttu-id="682f8-139">list</span><span class="sxs-lookup"><span data-stu-id="682f8-139">list</span></span>](../resources/list.md) | <span data-ttu-id="682f8-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682f8-140">Sites.ReadWrite.All</span></span> | <span data-ttu-id="682f8-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="682f8-141">Not supported</span></span> | <span data-ttu-id="682f8-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682f8-142">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="682f8-143">message</span><span class="sxs-lookup"><span data-stu-id="682f8-143">message</span></span>](../resources/message.md) | <span data-ttu-id="682f8-144">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-144">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="682f8-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="682f8-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="682f8-146">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="682f8-147">security alert</span><span class="sxs-lookup"><span data-stu-id="682f8-147">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="682f8-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682f8-148">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="682f8-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="682f8-149">Not supported</span></span> | <span data-ttu-id="682f8-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682f8-150">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="682f8-151">user</span><span class="sxs-lookup"><span data-stu-id="682f8-151">user</span></span>](../resources/user.md) | <span data-ttu-id="682f8-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="682f8-152">User.Read.All</span></span> | <span data-ttu-id="682f8-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="682f8-153">User.Read.All</span></span> | <span data-ttu-id="682f8-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="682f8-154">User.Read.All</span></span> |

> <span data-ttu-id="682f8-155">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="682f8-155">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="682f8-156">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="682f8-156">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="682f8-157">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="682f8-157">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="682f8-158">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="682f8-158">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="682f8-159">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="682f8-159">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="682f8-160">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="682f8-160">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="682f8-161">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="682f8-161">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="682f8-162">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="682f8-162">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="682f8-163">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="682f8-163">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="682f8-164">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="682f8-164">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="682f8-165">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="682f8-165">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="682f8-166">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="682f8-166">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="682f8-167">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="682f8-167">Request headers</span></span>

| <span data-ttu-id="682f8-168">Имя</span><span class="sxs-lookup"><span data-stu-id="682f8-168">Name</span></span>       | <span data-ttu-id="682f8-169">Тип</span><span class="sxs-lookup"><span data-stu-id="682f8-169">Type</span></span> | <span data-ttu-id="682f8-170">Описание</span><span class="sxs-lookup"><span data-stu-id="682f8-170">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="682f8-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="682f8-171">Authorization</span></span>  | <span data-ttu-id="682f8-172">string</span><span class="sxs-lookup"><span data-stu-id="682f8-172">string</span></span>  | <span data-ttu-id="682f8-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="682f8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="682f8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="682f8-175">Response</span></span>

<span data-ttu-id="682f8-176">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="682f8-176">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="682f8-177">Пример</span><span class="sxs-lookup"><span data-stu-id="682f8-177">Example</span></span>

##### <a name="request"></a><span data-ttu-id="682f8-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="682f8-178">Request</span></span>

<span data-ttu-id="682f8-179">Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="682f8-179">Here is an example of the request to send a notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="682f8-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="682f8-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="682f8-181">C#</span><span class="sxs-lookup"><span data-stu-id="682f8-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="682f8-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="682f8-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="682f8-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="682f8-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="682f8-184">Java</span><span class="sxs-lookup"><span data-stu-id="682f8-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="682f8-185">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="682f8-185">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="682f8-186">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="682f8-186">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="682f8-187">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="682f8-187">Resources examples</span></span>

<span data-ttu-id="682f8-188">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="682f8-188">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="682f8-189">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="682f8-189">Resource type</span></span> | <span data-ttu-id="682f8-190">Примеры</span><span class="sxs-lookup"><span data-stu-id="682f8-190">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="682f8-191">Mail</span><span class="sxs-lookup"><span data-stu-id="682f8-191">Mail</span></span>|<span data-ttu-id="682f8-192">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="682f8-192">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="682f8-193">me/messages</span><span class="sxs-lookup"><span data-stu-id="682f8-193">me/messages</span></span>|
|<span data-ttu-id="682f8-194">Contacts</span><span class="sxs-lookup"><span data-stu-id="682f8-194">Contacts</span></span>|<span data-ttu-id="682f8-195">me/contacts</span><span class="sxs-lookup"><span data-stu-id="682f8-195">me/contacts</span></span>|
|<span data-ttu-id="682f8-196">Calendars</span><span class="sxs-lookup"><span data-stu-id="682f8-196">Calendars</span></span>|<span data-ttu-id="682f8-197">me/events</span><span class="sxs-lookup"><span data-stu-id="682f8-197">me/events</span></span>|
|<span data-ttu-id="682f8-198">Users</span><span class="sxs-lookup"><span data-stu-id="682f8-198">Users</span></span>|<span data-ttu-id="682f8-199">users</span><span class="sxs-lookup"><span data-stu-id="682f8-199">users</span></span>|
|<span data-ttu-id="682f8-200">Groups</span><span class="sxs-lookup"><span data-stu-id="682f8-200">Groups</span></span>|<span data-ttu-id="682f8-201">groups</span><span class="sxs-lookup"><span data-stu-id="682f8-201">groups</span></span>|
|<span data-ttu-id="682f8-202">Conversations</span><span class="sxs-lookup"><span data-stu-id="682f8-202">Conversations</span></span>|<span data-ttu-id="682f8-203">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="682f8-203">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="682f8-204">Drives</span><span class="sxs-lookup"><span data-stu-id="682f8-204">Drives</span></span>|<span data-ttu-id="682f8-205">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="682f8-205">me/drive/root</span></span>|
|<span data-ttu-id="682f8-206">Список</span><span class="sxs-lookup"><span data-stu-id="682f8-206">List</span></span>|<span data-ttu-id="682f8-207">sites/{site-id}/lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="682f8-207">sites/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="682f8-208">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="682f8-208">Security alert</span></span>|<span data-ttu-id="682f8-209">security/alerts?$filter=status eq 'New'</span><span class="sxs-lookup"><span data-stu-id="682f8-209">security/alerts?$filter=status eq 'New'</span></span>|

##### <a name="response"></a><span data-ttu-id="682f8-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="682f8-210">Response</span></span>

<span data-ttu-id="682f8-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="682f8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="682f8-214">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="682f8-214">Notification endpoint validation</span></span>

<span data-ttu-id="682f8-215">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="682f8-215">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="682f8-216">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="682f8-216">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
