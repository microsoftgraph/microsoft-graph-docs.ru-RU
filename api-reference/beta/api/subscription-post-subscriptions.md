---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 487be3c7a50dcd5b09ece599f69b74248965eacf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870840"
---
# <a name="create-subscription"></a><span data-ttu-id="db98d-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="db98d-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db98d-104">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="db98d-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="db98d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db98d-105">Permissions</span></span>

<span data-ttu-id="db98d-106">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="db98d-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="db98d-107">Например, чтобы получать уведомления о сообщениях, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="db98d-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="db98d-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="db98d-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="db98d-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db98d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db98d-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="db98d-110">Supported resource</span></span> | <span data-ttu-id="db98d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db98d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db98d-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db98d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db98d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db98d-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="db98d-114">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="db98d-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="db98d-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-115">Not supported</span></span> | <span data-ttu-id="db98d-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-116">Not supported</span></span> | <span data-ttu-id="db98d-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="db98d-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="db98d-118">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="db98d-118">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="db98d-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-119">Not supported</span></span> | <span data-ttu-id="db98d-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-120">Not supported</span></span> | <span data-ttu-id="db98d-121">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="db98d-121">Chat.Read.All</span></span>  |
|[<span data-ttu-id="db98d-122">contact</span><span class="sxs-lookup"><span data-stu-id="db98d-122">contact</span></span>](../resources/contact.md) | <span data-ttu-id="db98d-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-123">Contacts.Read</span></span> | <span data-ttu-id="db98d-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-124">Contacts.Read</span></span> | <span data-ttu-id="db98d-125">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-125">Contacts.Read</span></span> |
|<span data-ttu-id="db98d-126">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="db98d-126">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="db98d-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-127">Not supported</span></span> | <span data-ttu-id="db98d-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db98d-128">Files.ReadWrite</span></span> | <span data-ttu-id="db98d-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-129">Not supported</span></span> |
|<span data-ttu-id="db98d-130">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="db98d-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="db98d-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db98d-131">Files.ReadWrite.All</span></span> | <span data-ttu-id="db98d-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-132">Not supported</span></span> | <span data-ttu-id="db98d-133">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db98d-133">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="db98d-134">event</span><span class="sxs-lookup"><span data-stu-id="db98d-134">event</span></span>](../resources/event.md) | <span data-ttu-id="db98d-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-135">Calendars.Read</span></span> | <span data-ttu-id="db98d-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-136">Calendars.Read</span></span> | <span data-ttu-id="db98d-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-137">Calendars.Read</span></span> |
|[<span data-ttu-id="db98d-138">group</span><span class="sxs-lookup"><span data-stu-id="db98d-138">group</span></span>](../resources/group.md) | <span data-ttu-id="db98d-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="db98d-139">Group.Read.All</span></span> | <span data-ttu-id="db98d-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-140">Not supported</span></span> | <span data-ttu-id="db98d-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="db98d-141">Group.Read.All</span></span> |
|[<span data-ttu-id="db98d-142">group conversation</span><span class="sxs-lookup"><span data-stu-id="db98d-142">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="db98d-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="db98d-143">Group.Read.All</span></span> | <span data-ttu-id="db98d-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-144">Not supported</span></span> | <span data-ttu-id="db98d-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-145">Not supported</span></span> |
|[<span data-ttu-id="db98d-146">message</span><span class="sxs-lookup"><span data-stu-id="db98d-146">message</span></span>](../resources/message.md) | <span data-ttu-id="db98d-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="db98d-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="db98d-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="db98d-149">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="db98d-150">security alert</span><span class="sxs-lookup"><span data-stu-id="db98d-150">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="db98d-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db98d-151">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="db98d-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="db98d-152">Not supported</span></span> | <span data-ttu-id="db98d-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db98d-153">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="db98d-154">user</span><span class="sxs-lookup"><span data-stu-id="db98d-154">user</span></span>](../resources/user.md) | <span data-ttu-id="db98d-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="db98d-155">User.Read.All</span></span> | <span data-ttu-id="db98d-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="db98d-156">User.Read.All</span></span> | <span data-ttu-id="db98d-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="db98d-157">User.Read.All</span></span> |

> <span data-ttu-id="db98d-158">**Примечание:** В январе 2020 подписки chatMessage потребуют [шифрования](/graph/webhooks-with-resource-data), и создание подписки завершится с ошибками, если [енкриптионцертификате](../resources/subscription.md) не задано.</span><span class="sxs-lookup"><span data-stu-id="db98d-158">**Note:** In January 2020, chatMessage subscriptions will require [encryption](/graph/webhooks-with-resource-data), and subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

> <span data-ttu-id="db98d-159">**Примечание:** Дополнительные ограничения применяются для подписок на OneDrive и элементов Outlook.</span><span class="sxs-lookup"><span data-stu-id="db98d-159">**Note:** Additional limitations apply for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="db98d-160">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="db98d-160">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="db98d-161">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="db98d-161">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="db98d-162">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="db98d-162">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="db98d-163">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="db98d-163">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="db98d-164">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="db98d-164">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="db98d-165">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="db98d-165">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="db98d-166">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="db98d-166">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="db98d-167">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="db98d-167">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="db98d-168">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="db98d-168">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="db98d-169">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="db98d-169">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="db98d-170">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db98d-170">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="db98d-171">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db98d-171">Request headers</span></span>

| <span data-ttu-id="db98d-172">Имя</span><span class="sxs-lookup"><span data-stu-id="db98d-172">Name</span></span>       | <span data-ttu-id="db98d-173">Тип</span><span class="sxs-lookup"><span data-stu-id="db98d-173">Type</span></span> | <span data-ttu-id="db98d-174">Описание</span><span class="sxs-lookup"><span data-stu-id="db98d-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db98d-175">Authorization</span><span class="sxs-lookup"><span data-stu-id="db98d-175">Authorization</span></span>  | <span data-ttu-id="db98d-176">string</span><span class="sxs-lookup"><span data-stu-id="db98d-176">string</span></span>  | <span data-ttu-id="db98d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db98d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="db98d-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="db98d-179">Response</span></span>

<span data-ttu-id="db98d-180">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db98d-180">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db98d-181">Пример</span><span class="sxs-lookup"><span data-stu-id="db98d-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="db98d-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="db98d-182">Request</span></span>

<span data-ttu-id="db98d-183">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db98d-183">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="db98d-184">Поле `clientState` является необязательным.</span><span class="sxs-lookup"><span data-stu-id="db98d-184">The `clientState` field is optional.</span></span>

<span data-ttu-id="db98d-185">Этот запрос создает подписку на уведомления о новых сообщениях, получаемых пользователем, который вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="db98d-185">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db98d-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="db98d-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db98d-187">C#</span><span class="sxs-lookup"><span data-stu-id="db98d-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db98d-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db98d-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db98d-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db98d-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="db98d-190">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="db98d-190">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="db98d-191">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="db98d-191">Resource type</span></span> | <span data-ttu-id="db98d-192">Примеры</span><span class="sxs-lookup"><span data-stu-id="db98d-192">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="db98d-193">Mail</span><span class="sxs-lookup"><span data-stu-id="db98d-193">Mail</span></span>|<span data-ttu-id="db98d-194">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="db98d-194">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="db98d-195">me/messages</span><span class="sxs-lookup"><span data-stu-id="db98d-195">me/messages</span></span>|
|<span data-ttu-id="db98d-196">Contacts</span><span class="sxs-lookup"><span data-stu-id="db98d-196">Contacts</span></span>|<span data-ttu-id="db98d-197">me/contacts</span><span class="sxs-lookup"><span data-stu-id="db98d-197">me/contacts</span></span>|
|<span data-ttu-id="db98d-198">Calendars</span><span class="sxs-lookup"><span data-stu-id="db98d-198">Calendars</span></span>|<span data-ttu-id="db98d-199">me/events</span><span class="sxs-lookup"><span data-stu-id="db98d-199">me/events</span></span>|
|<span data-ttu-id="db98d-200">Users</span><span class="sxs-lookup"><span data-stu-id="db98d-200">Users</span></span>|<span data-ttu-id="db98d-201">users</span><span class="sxs-lookup"><span data-stu-id="db98d-201">users</span></span>|
|<span data-ttu-id="db98d-202">Groups</span><span class="sxs-lookup"><span data-stu-id="db98d-202">Groups</span></span>|<span data-ttu-id="db98d-203">groups</span><span class="sxs-lookup"><span data-stu-id="db98d-203">groups</span></span>|
|<span data-ttu-id="db98d-204">Conversations</span><span class="sxs-lookup"><span data-stu-id="db98d-204">Conversations</span></span>|<span data-ttu-id="db98d-205">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="db98d-205">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="db98d-206">Drives</span><span class="sxs-lookup"><span data-stu-id="db98d-206">Drives</span></span>|<span data-ttu-id="db98d-207">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="db98d-207">me/drive/root</span></span>|
|<span data-ttu-id="db98d-208">Security alert</span><span class="sxs-lookup"><span data-stu-id="db98d-208">Security alert</span></span>|<span data-ttu-id="db98d-209">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="db98d-209">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="db98d-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="db98d-210">Response</span></span>

<span data-ttu-id="db98d-211">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db98d-211">The following example shows the response.</span></span> 

><span data-ttu-id="db98d-p108">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db98d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="db98d-214">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="db98d-214">Notification endpoint validation</span></span>

<span data-ttu-id="db98d-215">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="db98d-215">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="db98d-216">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="db98d-216">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
