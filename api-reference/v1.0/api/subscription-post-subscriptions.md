---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в Microsoft Graph.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 28053ccd79b8cbab521f3cbd702dd46835d14ecb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491835"
---
# <a name="create-subscription"></a><span data-ttu-id="bf95a-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="bf95a-103">Create subscription</span></span>

<span data-ttu-id="bf95a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf95a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf95a-105">Подписывает приложение прослушивателя на получение уведомлений об изменениях, когда запрошенный тип изменений выполняется для указанного ресурса в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bf95a-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf95a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf95a-106">Permissions</span></span>

 <span data-ttu-id="bf95a-107">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="bf95a-107">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="bf95a-108">Например, чтобы получать уведомления об изменениях для сообщений, ваше приложение должно иметь `Mail.Read` разрешение.</span><span class="sxs-lookup"><span data-stu-id="bf95a-108">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="bf95a-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bf95a-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="bf95a-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf95a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf95a-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="bf95a-111">Supported resource</span></span> | <span data-ttu-id="bf95a-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf95a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf95a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf95a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf95a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf95a-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="bf95a-115">[каллрекорд](../resources/callrecords-callrecord.md) (/коммуникатионс/каллрекордс)</span><span class="sxs-lookup"><span data-stu-id="bf95a-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="bf95a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-116">Not supported</span></span> | <span data-ttu-id="bf95a-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-117">Not supported</span></span> | <span data-ttu-id="bf95a-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-118">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="bf95a-119">contact</span><span class="sxs-lookup"><span data-stu-id="bf95a-119">contact</span></span>](../resources/contact.md) | <span data-ttu-id="bf95a-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-120">Contacts.Read</span></span> | <span data-ttu-id="bf95a-121">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-121">Contacts.Read</span></span> | <span data-ttu-id="bf95a-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-122">Contacts.Read</span></span> |
|<span data-ttu-id="bf95a-123">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="bf95a-123">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="bf95a-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-124">Not supported</span></span> | <span data-ttu-id="bf95a-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf95a-125">Files.ReadWrite</span></span> | <span data-ttu-id="bf95a-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-126">Not supported</span></span> |
|<span data-ttu-id="bf95a-127">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="bf95a-127">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="bf95a-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-128">Files.ReadWrite.All</span></span> | <span data-ttu-id="bf95a-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-129">Not supported</span></span> | <span data-ttu-id="bf95a-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-130">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf95a-131">event</span><span class="sxs-lookup"><span data-stu-id="bf95a-131">event</span></span>](../resources/event.md) | <span data-ttu-id="bf95a-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-132">Calendars.Read</span></span> | <span data-ttu-id="bf95a-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-133">Calendars.Read</span></span> | <span data-ttu-id="bf95a-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-134">Calendars.Read</span></span> |
|[<span data-ttu-id="bf95a-135">group</span><span class="sxs-lookup"><span data-stu-id="bf95a-135">group</span></span>](../resources/group.md) | <span data-ttu-id="bf95a-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-136">Group.Read.All</span></span> | <span data-ttu-id="bf95a-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-137">Not supported</span></span> | <span data-ttu-id="bf95a-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-138">Group.Read.All</span></span> |
|[<span data-ttu-id="bf95a-139">group conversation</span><span class="sxs-lookup"><span data-stu-id="bf95a-139">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="bf95a-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-140">Group.Read.All</span></span> | <span data-ttu-id="bf95a-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-141">Not supported</span></span> | <span data-ttu-id="bf95a-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-142">Not supported</span></span> |
|[<span data-ttu-id="bf95a-143">list</span><span class="sxs-lookup"><span data-stu-id="bf95a-143">list</span></span>](../resources/list.md) | <span data-ttu-id="bf95a-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-144">Sites.ReadWrite.All</span></span> | <span data-ttu-id="bf95a-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-145">Not supported</span></span> | <span data-ttu-id="bf95a-146">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-146">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf95a-147">message</span><span class="sxs-lookup"><span data-stu-id="bf95a-147">message</span></span>](../resources/message.md) | <span data-ttu-id="bf95a-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bf95a-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-149">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="bf95a-150">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf95a-150">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="bf95a-151">security alert</span><span class="sxs-lookup"><span data-stu-id="bf95a-151">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="bf95a-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-152">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="bf95a-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bf95a-153">Not supported</span></span> | <span data-ttu-id="bf95a-154">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-154">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="bf95a-155">user</span><span class="sxs-lookup"><span data-stu-id="bf95a-155">user</span></span>](../resources/user.md) | <span data-ttu-id="bf95a-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-156">User.Read.All</span></span> | <span data-ttu-id="bf95a-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-157">User.Read.All</span></span> | <span data-ttu-id="bf95a-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf95a-158">User.Read.All</span></span> |

> <span data-ttu-id="bf95a-159">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="bf95a-159">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="bf95a-160">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="bf95a-160">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="bf95a-161">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="bf95a-161">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="bf95a-162">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="bf95a-162">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="bf95a-163">Уведомления об изменениях отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других экземпляров **driveItem** в иерархии.</span><span class="sxs-lookup"><span data-stu-id="bf95a-163">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="bf95a-164">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="bf95a-164">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="bf95a-165">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="bf95a-165">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="bf95a-166">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf95a-166">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="bf95a-167">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="bf95a-167">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="bf95a-168">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="bf95a-168">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="bf95a-169">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="bf95a-169">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="bf95a-170">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf95a-170">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="bf95a-171">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf95a-171">Request headers</span></span>

| <span data-ttu-id="bf95a-172">Имя</span><span class="sxs-lookup"><span data-stu-id="bf95a-172">Name</span></span>       | <span data-ttu-id="bf95a-173">Тип</span><span class="sxs-lookup"><span data-stu-id="bf95a-173">Type</span></span> | <span data-ttu-id="bf95a-174">Описание</span><span class="sxs-lookup"><span data-stu-id="bf95a-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bf95a-175">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf95a-175">Authorization</span></span>  | <span data-ttu-id="bf95a-176">string</span><span class="sxs-lookup"><span data-stu-id="bf95a-176">string</span></span>  | <span data-ttu-id="bf95a-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf95a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bf95a-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf95a-179">Response</span></span>

<span data-ttu-id="bf95a-180">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bf95a-180">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="bf95a-181">Сведения о том, как возвращаются ошибки, приведены в разделе [ошибочные ответы][error-response].</span><span class="sxs-lookup"><span data-stu-id="bf95a-181">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="bf95a-182">Пример</span><span class="sxs-lookup"><span data-stu-id="bf95a-182">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bf95a-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf95a-183">Request</span></span>

<span data-ttu-id="bf95a-184">Ниже приведен пример запроса на отправку уведомления об изменении при получении пользователем новой почты.</span><span class="sxs-lookup"><span data-stu-id="bf95a-184">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf95a-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf95a-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bf95a-186">C#</span><span class="sxs-lookup"><span data-stu-id="bf95a-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf95a-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf95a-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf95a-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf95a-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf95a-189">Java</span><span class="sxs-lookup"><span data-stu-id="bf95a-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="bf95a-190">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf95a-190">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="bf95a-191">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="bf95a-191">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="bf95a-192">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="bf95a-192">Resources examples</span></span>

<span data-ttu-id="bf95a-193">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="bf95a-193">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="bf95a-194">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="bf95a-194">Resource type</span></span> | <span data-ttu-id="bf95a-195">Примеры</span><span class="sxs-lookup"><span data-stu-id="bf95a-195">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="bf95a-196">Mail</span><span class="sxs-lookup"><span data-stu-id="bf95a-196">Mail</span></span>|<span data-ttu-id="bf95a-197">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="bf95a-197">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="bf95a-198">me/messages</span><span class="sxs-lookup"><span data-stu-id="bf95a-198">me/messages</span></span>|
|<span data-ttu-id="bf95a-199">Contacts</span><span class="sxs-lookup"><span data-stu-id="bf95a-199">Contacts</span></span>|<span data-ttu-id="bf95a-200">me/contacts</span><span class="sxs-lookup"><span data-stu-id="bf95a-200">me/contacts</span></span>|
|<span data-ttu-id="bf95a-201">Calendars</span><span class="sxs-lookup"><span data-stu-id="bf95a-201">Calendars</span></span>|<span data-ttu-id="bf95a-202">me/events</span><span class="sxs-lookup"><span data-stu-id="bf95a-202">me/events</span></span>|
|<span data-ttu-id="bf95a-203">Users</span><span class="sxs-lookup"><span data-stu-id="bf95a-203">Users</span></span>|<span data-ttu-id="bf95a-204">users</span><span class="sxs-lookup"><span data-stu-id="bf95a-204">users</span></span>|
|<span data-ttu-id="bf95a-205">Groups</span><span class="sxs-lookup"><span data-stu-id="bf95a-205">Groups</span></span>|<span data-ttu-id="bf95a-206">groups</span><span class="sxs-lookup"><span data-stu-id="bf95a-206">groups</span></span>|
|<span data-ttu-id="bf95a-207">Conversations</span><span class="sxs-lookup"><span data-stu-id="bf95a-207">Conversations</span></span>|<span data-ttu-id="bf95a-208">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="bf95a-208">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="bf95a-209">Drives</span><span class="sxs-lookup"><span data-stu-id="bf95a-209">Drives</span></span>|<span data-ttu-id="bf95a-210">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="bf95a-210">me/drive/root</span></span>|
|<span data-ttu-id="bf95a-211">Список</span><span class="sxs-lookup"><span data-stu-id="bf95a-211">List</span></span>|<span data-ttu-id="bf95a-212">sites/{site-id}/lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="bf95a-212">sites/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="bf95a-213">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="bf95a-213">Security alert</span></span>|<span data-ttu-id="bf95a-214">security/alerts?$filter=status eq 'New'</span><span class="sxs-lookup"><span data-stu-id="bf95a-214">security/alerts?$filter=status eq 'New'</span></span>|
|<span data-ttu-id="bf95a-215">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="bf95a-215">Call records</span></span>|<span data-ttu-id="bf95a-216">связь/Каллрекордс</span><span class="sxs-lookup"><span data-stu-id="bf95a-216">communications/callRecords</span></span>|

##### <a name="response"></a><span data-ttu-id="bf95a-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf95a-217">Response</span></span>

<span data-ttu-id="bf95a-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf95a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="bf95a-221">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="bf95a-221">Notification endpoint validation</span></span>

<span data-ttu-id="bf95a-222">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="bf95a-222">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="bf95a-223">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="bf95a-223">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
