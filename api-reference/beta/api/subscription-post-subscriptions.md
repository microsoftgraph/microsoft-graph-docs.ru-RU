---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: fff6dd2d707ba75db352837e77089f97e58cb325
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774389"
---
# <a name="create-subscription"></a><span data-ttu-id="0c113-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="0c113-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c113-104">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0c113-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c113-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c113-105">Permissions</span></span>

<span data-ttu-id="0c113-106">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="0c113-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="0c113-107">Например, чтобы получать уведомления о сообщениях, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="0c113-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="0c113-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0c113-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="0c113-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c113-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c113-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="0c113-110">Supported resource</span></span> | <span data-ttu-id="0c113-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c113-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0c113-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c113-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c113-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c113-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="0c113-114">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="0c113-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="0c113-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-115">Not supported</span></span> | <span data-ttu-id="0c113-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-116">Not supported</span></span> | <span data-ttu-id="0c113-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c113-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="0c113-118">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="0c113-118">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="0c113-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-119">Not supported</span></span> | <span data-ttu-id="0c113-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-120">Not supported</span></span> | <span data-ttu-id="0c113-121">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c113-121">Chat.Read.All</span></span>  |
|[<span data-ttu-id="0c113-122">contact</span><span class="sxs-lookup"><span data-stu-id="0c113-122">contact</span></span>](../resources/contact.md) | <span data-ttu-id="0c113-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-123">Contacts.Read</span></span> | <span data-ttu-id="0c113-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-124">Contacts.Read</span></span> | <span data-ttu-id="0c113-125">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-125">Contacts.Read</span></span> |
|<span data-ttu-id="0c113-126">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="0c113-126">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="0c113-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-127">Not supported</span></span> | <span data-ttu-id="0c113-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c113-128">Files.ReadWrite</span></span> | <span data-ttu-id="0c113-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-129">Not supported</span></span> |
|<span data-ttu-id="0c113-130">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="0c113-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="0c113-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c113-131">Files.ReadWrite.All</span></span> | <span data-ttu-id="0c113-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-132">Not supported</span></span> | <span data-ttu-id="0c113-133">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c113-133">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="0c113-134">event</span><span class="sxs-lookup"><span data-stu-id="0c113-134">event</span></span>](../resources/event.md) | <span data-ttu-id="0c113-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-135">Calendars.Read</span></span> | <span data-ttu-id="0c113-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-136">Calendars.Read</span></span> | <span data-ttu-id="0c113-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-137">Calendars.Read</span></span> |
|[<span data-ttu-id="0c113-138">group</span><span class="sxs-lookup"><span data-stu-id="0c113-138">group</span></span>](../resources/group.md) | <span data-ttu-id="0c113-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c113-139">Group.Read.All</span></span> | <span data-ttu-id="0c113-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-140">Not supported</span></span> | <span data-ttu-id="0c113-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c113-141">Group.Read.All</span></span> |
|[<span data-ttu-id="0c113-142">group conversation</span><span class="sxs-lookup"><span data-stu-id="0c113-142">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="0c113-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c113-143">Group.Read.All</span></span> | <span data-ttu-id="0c113-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-144">Not supported</span></span> | <span data-ttu-id="0c113-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-145">Not supported</span></span> |
|[<span data-ttu-id="0c113-146">message</span><span class="sxs-lookup"><span data-stu-id="0c113-146">message</span></span>](../resources/message.md) | <span data-ttu-id="0c113-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="0c113-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="0c113-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0c113-149">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="0c113-150">security alert</span><span class="sxs-lookup"><span data-stu-id="0c113-150">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="0c113-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c113-151">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="0c113-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0c113-152">Not supported</span></span> | <span data-ttu-id="0c113-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c113-153">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="0c113-154">user</span><span class="sxs-lookup"><span data-stu-id="0c113-154">user</span></span>](../resources/user.md) | <span data-ttu-id="0c113-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c113-155">User.Read.All</span></span> | <span data-ttu-id="0c113-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c113-156">User.Read.All</span></span> | <span data-ttu-id="0c113-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c113-157">User.Read.All</span></span> |

> <span data-ttu-id="0c113-158">**Note:** для подписок на chatMessage требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="0c113-158">**Note:** chatMessage subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="0c113-159">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="0c113-159">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

> <span data-ttu-id="0c113-160">**Примечание:** Дополнительные ограничения применяются для подписок на OneDrive и элементов Outlook.</span><span class="sxs-lookup"><span data-stu-id="0c113-160">**Note:** Additional limitations apply for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="0c113-161">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="0c113-161">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="0c113-162">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="0c113-162">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="0c113-163">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="0c113-163">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="0c113-164">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="0c113-164">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="0c113-165">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="0c113-165">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="0c113-166">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="0c113-166">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="0c113-167">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="0c113-167">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="0c113-168">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="0c113-168">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="0c113-169">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0c113-169">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="0c113-170">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="0c113-170">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="0c113-171">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c113-171">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="0c113-172">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c113-172">Request headers</span></span>

| <span data-ttu-id="0c113-173">Имя</span><span class="sxs-lookup"><span data-stu-id="0c113-173">Name</span></span>       | <span data-ttu-id="0c113-174">Тип</span><span class="sxs-lookup"><span data-stu-id="0c113-174">Type</span></span> | <span data-ttu-id="0c113-175">Описание</span><span class="sxs-lookup"><span data-stu-id="0c113-175">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0c113-176">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c113-176">Authorization</span></span>  | <span data-ttu-id="0c113-177">string</span><span class="sxs-lookup"><span data-stu-id="0c113-177">string</span></span>  | <span data-ttu-id="0c113-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c113-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0c113-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c113-180">Response</span></span>

<span data-ttu-id="0c113-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c113-181">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c113-182">Пример</span><span class="sxs-lookup"><span data-stu-id="0c113-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c113-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c113-183">Request</span></span>

<span data-ttu-id="0c113-184">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c113-184">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="0c113-185">Поля `clientState` и `latestSupportedTlsVersion` являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="0c113-185">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="0c113-186">Этот запрос создает подписку на уведомления о новых сообщениях, получаемых пользователем, который вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="0c113-186">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c113-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c113-187">HTTP</span></span>](#tab/http)
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
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c113-188">C#</span><span class="sxs-lookup"><span data-stu-id="0c113-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c113-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c113-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c113-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c113-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0c113-191">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="0c113-191">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="0c113-192">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="0c113-192">Resource type</span></span> | <span data-ttu-id="0c113-193">Примеры</span><span class="sxs-lookup"><span data-stu-id="0c113-193">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="0c113-194">Mail</span><span class="sxs-lookup"><span data-stu-id="0c113-194">Mail</span></span>|<span data-ttu-id="0c113-195">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="0c113-195">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="0c113-196">me/messages</span><span class="sxs-lookup"><span data-stu-id="0c113-196">me/messages</span></span>|
|<span data-ttu-id="0c113-197">Contacts</span><span class="sxs-lookup"><span data-stu-id="0c113-197">Contacts</span></span>|<span data-ttu-id="0c113-198">me/contacts</span><span class="sxs-lookup"><span data-stu-id="0c113-198">me/contacts</span></span>|
|<span data-ttu-id="0c113-199">Calendars</span><span class="sxs-lookup"><span data-stu-id="0c113-199">Calendars</span></span>|<span data-ttu-id="0c113-200">me/events</span><span class="sxs-lookup"><span data-stu-id="0c113-200">me/events</span></span>|
|<span data-ttu-id="0c113-201">Users</span><span class="sxs-lookup"><span data-stu-id="0c113-201">Users</span></span>|<span data-ttu-id="0c113-202">users</span><span class="sxs-lookup"><span data-stu-id="0c113-202">users</span></span>|
|<span data-ttu-id="0c113-203">Groups</span><span class="sxs-lookup"><span data-stu-id="0c113-203">Groups</span></span>|<span data-ttu-id="0c113-204">groups</span><span class="sxs-lookup"><span data-stu-id="0c113-204">groups</span></span>|
|<span data-ttu-id="0c113-205">Conversations</span><span class="sxs-lookup"><span data-stu-id="0c113-205">Conversations</span></span>|<span data-ttu-id="0c113-206">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="0c113-206">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="0c113-207">Drives</span><span class="sxs-lookup"><span data-stu-id="0c113-207">Drives</span></span>|<span data-ttu-id="0c113-208">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="0c113-208">me/drive/root</span></span>|
|<span data-ttu-id="0c113-209">Security alert</span><span class="sxs-lookup"><span data-stu-id="0c113-209">Security alert</span></span>|<span data-ttu-id="0c113-210">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="0c113-210">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="0c113-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c113-211">Response</span></span>

<span data-ttu-id="0c113-212">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c113-212">The following example shows the response.</span></span> 

><span data-ttu-id="0c113-p109">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c113-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="0c113-215">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="0c113-215">Notification endpoint validation</span></span>

<span data-ttu-id="0c113-216">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="0c113-216">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="0c113-217">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="0c113-217">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
