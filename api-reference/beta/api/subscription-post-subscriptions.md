---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 4a5ffc3ec86c0ce40e4b5fca25b7f0ddcf5dca9f
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844178"
---
# <a name="create-subscription"></a><span data-ttu-id="2ae21-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="2ae21-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ae21-104">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2ae21-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ae21-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ae21-105">Permissions</span></span>

<span data-ttu-id="2ae21-106">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ae21-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="2ae21-107">Например, чтобы получать уведомления о сообщениях, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="2ae21-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="2ae21-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2ae21-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2ae21-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ae21-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ae21-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="2ae21-110">Supported resource</span></span> | <span data-ttu-id="2ae21-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ae21-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ae21-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ae21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ae21-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ae21-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="2ae21-114">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="2ae21-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="2ae21-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-115">Not supported</span></span> | <span data-ttu-id="2ae21-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-116">Not supported</span></span> | <span data-ttu-id="2ae21-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2ae21-118">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="2ae21-118">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="2ae21-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-119">Not supported</span></span> | <span data-ttu-id="2ae21-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-120">Not supported</span></span> | <span data-ttu-id="2ae21-121">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-121">Chat.Read.All</span></span>  |
|[<span data-ttu-id="2ae21-122">contact</span><span class="sxs-lookup"><span data-stu-id="2ae21-122">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2ae21-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-123">Contacts.Read</span></span> | <span data-ttu-id="2ae21-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-124">Contacts.Read</span></span> | <span data-ttu-id="2ae21-125">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-125">Contacts.Read</span></span> |
|<span data-ttu-id="2ae21-126">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="2ae21-126">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2ae21-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-127">Not supported</span></span> | <span data-ttu-id="2ae21-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ae21-128">Files.ReadWrite</span></span> | <span data-ttu-id="2ae21-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-129">Not supported</span></span> |
|<span data-ttu-id="2ae21-130">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="2ae21-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2ae21-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-131">Files.ReadWrite.All</span></span> | <span data-ttu-id="2ae21-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-132">Not supported</span></span> | <span data-ttu-id="2ae21-133">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-133">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2ae21-134">event</span><span class="sxs-lookup"><span data-stu-id="2ae21-134">event</span></span>](../resources/event.md) | <span data-ttu-id="2ae21-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-135">Calendars.Read</span></span> | <span data-ttu-id="2ae21-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-136">Calendars.Read</span></span> | <span data-ttu-id="2ae21-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-137">Calendars.Read</span></span> |
|[<span data-ttu-id="2ae21-138">group</span><span class="sxs-lookup"><span data-stu-id="2ae21-138">group</span></span>](../resources/group.md) | <span data-ttu-id="2ae21-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-139">Group.Read.All</span></span> | <span data-ttu-id="2ae21-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-140">Not supported</span></span> | <span data-ttu-id="2ae21-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-141">Group.Read.All</span></span> |
|[<span data-ttu-id="2ae21-142">group conversation</span><span class="sxs-lookup"><span data-stu-id="2ae21-142">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2ae21-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-143">Group.Read.All</span></span> | <span data-ttu-id="2ae21-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-144">Not supported</span></span> | <span data-ttu-id="2ae21-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-145">Not supported</span></span> |
|[<span data-ttu-id="2ae21-146">message</span><span class="sxs-lookup"><span data-stu-id="2ae21-146">message</span></span>](../resources/message.md) | <span data-ttu-id="2ae21-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2ae21-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2ae21-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2ae21-149">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="2ae21-150">security alert</span><span class="sxs-lookup"><span data-stu-id="2ae21-150">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="2ae21-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-151">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2ae21-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2ae21-152">Not supported</span></span> | <span data-ttu-id="2ae21-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-153">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="2ae21-154">user</span><span class="sxs-lookup"><span data-stu-id="2ae21-154">user</span></span>](../resources/user.md) | <span data-ttu-id="2ae21-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-155">User.Read.All</span></span> | <span data-ttu-id="2ae21-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-156">User.Read.All</span></span> | <span data-ttu-id="2ae21-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ae21-157">User.Read.All</span></span> |

> <span data-ttu-id="2ae21-158">**Примечание:** Дополнительные ограничения применяются для подписок на OneDrive и элементов Outlook.</span><span class="sxs-lookup"><span data-stu-id="2ae21-158">**Note:** Additional limitations apply for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="2ae21-159">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="2ae21-159">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="2ae21-160">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="2ae21-160">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2ae21-161">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="2ae21-161">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2ae21-162">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="2ae21-162">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="2ae21-163">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="2ae21-163">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="2ae21-164">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="2ae21-164">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2ae21-165">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ae21-165">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="2ae21-166">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="2ae21-166">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2ae21-167">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2ae21-167">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2ae21-168">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="2ae21-168">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="2ae21-169">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ae21-169">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="2ae21-170">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ae21-170">Request headers</span></span>

| <span data-ttu-id="2ae21-171">Имя</span><span class="sxs-lookup"><span data-stu-id="2ae21-171">Name</span></span>       | <span data-ttu-id="2ae21-172">Тип</span><span class="sxs-lookup"><span data-stu-id="2ae21-172">Type</span></span> | <span data-ttu-id="2ae21-173">Описание</span><span class="sxs-lookup"><span data-stu-id="2ae21-173">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2ae21-174">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ae21-174">Authorization</span></span>  | <span data-ttu-id="2ae21-175">string</span><span class="sxs-lookup"><span data-stu-id="2ae21-175">string</span></span>  | <span data-ttu-id="2ae21-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ae21-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2ae21-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ae21-178">Response</span></span>

<span data-ttu-id="2ae21-179">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ae21-179">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ae21-180">Пример</span><span class="sxs-lookup"><span data-stu-id="2ae21-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ae21-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ae21-181">Request</span></span>

<span data-ttu-id="2ae21-182">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ae21-182">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="2ae21-183">Поле `clientState` является необязательным.</span><span class="sxs-lookup"><span data-stu-id="2ae21-183">The `clientState` field is optional.</span></span>

<span data-ttu-id="2ae21-184">Этот запрос создает подписку на уведомления о новых сообщениях, получаемых пользователем, который вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="2ae21-184">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ae21-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ae21-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ae21-186">C#</span><span class="sxs-lookup"><span data-stu-id="2ae21-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ae21-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ae21-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ae21-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ae21-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2ae21-189">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="2ae21-189">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="2ae21-190">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="2ae21-190">Resource type</span></span> | <span data-ttu-id="2ae21-191">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ae21-191">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="2ae21-192">Mail</span><span class="sxs-lookup"><span data-stu-id="2ae21-192">Mail</span></span>|<span data-ttu-id="2ae21-193">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="2ae21-193">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="2ae21-194">me/messages</span><span class="sxs-lookup"><span data-stu-id="2ae21-194">me/messages</span></span>|
|<span data-ttu-id="2ae21-195">Contacts</span><span class="sxs-lookup"><span data-stu-id="2ae21-195">Contacts</span></span>|<span data-ttu-id="2ae21-196">me/contacts</span><span class="sxs-lookup"><span data-stu-id="2ae21-196">me/contacts</span></span>|
|<span data-ttu-id="2ae21-197">Calendars</span><span class="sxs-lookup"><span data-stu-id="2ae21-197">Calendars</span></span>|<span data-ttu-id="2ae21-198">me/events</span><span class="sxs-lookup"><span data-stu-id="2ae21-198">me/events</span></span>|
|<span data-ttu-id="2ae21-199">Users</span><span class="sxs-lookup"><span data-stu-id="2ae21-199">Users</span></span>|<span data-ttu-id="2ae21-200">users</span><span class="sxs-lookup"><span data-stu-id="2ae21-200">users</span></span>|
|<span data-ttu-id="2ae21-201">Groups</span><span class="sxs-lookup"><span data-stu-id="2ae21-201">Groups</span></span>|<span data-ttu-id="2ae21-202">groups</span><span class="sxs-lookup"><span data-stu-id="2ae21-202">groups</span></span>|
|<span data-ttu-id="2ae21-203">Conversations</span><span class="sxs-lookup"><span data-stu-id="2ae21-203">Conversations</span></span>|<span data-ttu-id="2ae21-204">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="2ae21-204">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="2ae21-205">Drives</span><span class="sxs-lookup"><span data-stu-id="2ae21-205">Drives</span></span>|<span data-ttu-id="2ae21-206">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="2ae21-206">me/drive/root</span></span>|
|<span data-ttu-id="2ae21-207">Security alert</span><span class="sxs-lookup"><span data-stu-id="2ae21-207">Security alert</span></span>|<span data-ttu-id="2ae21-208">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="2ae21-208">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="2ae21-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ae21-209">Response</span></span>

<span data-ttu-id="2ae21-210">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ae21-210">The following example shows the response.</span></span> 

><span data-ttu-id="2ae21-p108">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ae21-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="2ae21-213">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="2ae21-213">Notification endpoint validation</span></span>

<span data-ttu-id="2ae21-214">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="2ae21-214">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="2ae21-215">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="2ae21-215">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
