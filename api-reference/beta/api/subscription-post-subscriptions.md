---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: e5276d8cf4e0a096e1ce98c9247d0c46e9f515c9
ms.sourcegitcommit: 568909e47fb075264584e440fd0cad978abfab11
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/27/2020
ms.locfileid: "42287991"
---
# <a name="create-subscription"></a><span data-ttu-id="50252-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="50252-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50252-104">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="50252-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="50252-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50252-105">Permissions</span></span>

<span data-ttu-id="50252-106">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="50252-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="50252-107">Например, чтобы получать уведомления о сообщениях, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="50252-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="50252-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="50252-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="50252-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50252-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50252-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="50252-110">Supported resource</span></span> | <span data-ttu-id="50252-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50252-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50252-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50252-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50252-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50252-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="50252-114">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="50252-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="50252-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-115">Not supported</span></span> | <span data-ttu-id="50252-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-116">Not supported</span></span> | <span data-ttu-id="50252-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="50252-118">[chatMessage](../resources/chatmessage.md) (/теамс/аллмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="50252-118">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="50252-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-119">Not supported</span></span> | <span data-ttu-id="50252-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-120">Not supported</span></span> | <span data-ttu-id="50252-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-121">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="50252-122">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="50252-122">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="50252-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-123">Not supported</span></span> | <span data-ttu-id="50252-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-124">Not supported</span></span> | <span data-ttu-id="50252-125">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-125">Chat.Read.All</span></span>  |
|<span data-ttu-id="50252-126">[chatMessage](../resources/chatmessage.md) (/ЧАТС/аллмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="50252-126">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="50252-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-127">Not supported</span></span> | <span data-ttu-id="50252-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-128">Not supported</span></span> | <span data-ttu-id="50252-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-129">Chat.Read.All</span></span>  |
|[<span data-ttu-id="50252-130">contact</span><span class="sxs-lookup"><span data-stu-id="50252-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="50252-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="50252-131">Contacts.Read</span></span> | <span data-ttu-id="50252-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="50252-132">Contacts.Read</span></span> | <span data-ttu-id="50252-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="50252-133">Contacts.Read</span></span> |
|<span data-ttu-id="50252-134">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="50252-134">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="50252-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-135">Not supported</span></span> | <span data-ttu-id="50252-136">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50252-136">Files.ReadWrite</span></span> | <span data-ttu-id="50252-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-137">Not supported</span></span> |
|<span data-ttu-id="50252-138">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="50252-138">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="50252-139">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50252-139">Files.ReadWrite.All</span></span> | <span data-ttu-id="50252-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-140">Not supported</span></span> | <span data-ttu-id="50252-141">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50252-141">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="50252-142">event</span><span class="sxs-lookup"><span data-stu-id="50252-142">event</span></span>](../resources/event.md) | <span data-ttu-id="50252-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="50252-143">Calendars.Read</span></span> | <span data-ttu-id="50252-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="50252-144">Calendars.Read</span></span> | <span data-ttu-id="50252-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="50252-145">Calendars.Read</span></span> |
|[<span data-ttu-id="50252-146">group</span><span class="sxs-lookup"><span data-stu-id="50252-146">group</span></span>](../resources/group.md) | <span data-ttu-id="50252-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-147">Group.Read.All</span></span> | <span data-ttu-id="50252-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-148">Not supported</span></span> | <span data-ttu-id="50252-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-149">Group.Read.All</span></span> |
|[<span data-ttu-id="50252-150">group conversation</span><span class="sxs-lookup"><span data-stu-id="50252-150">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="50252-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-151">Group.Read.All</span></span> | <span data-ttu-id="50252-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-152">Not supported</span></span> | <span data-ttu-id="50252-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-153">Not supported</span></span> |
|[<span data-ttu-id="50252-154">message</span><span class="sxs-lookup"><span data-stu-id="50252-154">message</span></span>](../resources/message.md) | <span data-ttu-id="50252-155">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="50252-155">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="50252-156">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="50252-156">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="50252-157">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="50252-157">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="50252-158">security alert</span><span class="sxs-lookup"><span data-stu-id="50252-158">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="50252-159">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50252-159">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="50252-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="50252-160">Not supported</span></span> | <span data-ttu-id="50252-161">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50252-161">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="50252-162">user</span><span class="sxs-lookup"><span data-stu-id="50252-162">user</span></span>](../resources/user.md) | <span data-ttu-id="50252-163">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-163">User.Read.All</span></span> | <span data-ttu-id="50252-164">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-164">User.Read.All</span></span> | <span data-ttu-id="50252-165">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="50252-165">User.Read.All</span></span> |

### <a name="chatmessage-microsoft-teams"></a><span data-ttu-id="50252-166">chatMessage (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="50252-166">chatMessage (Microsoft Teams)</span></span>

<span data-ttu-id="50252-167">для подписок на **chatMessage** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="50252-167">**chatMessage** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="50252-168">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="50252-168">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="50252-169">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="50252-169">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="50252-170">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="50252-170">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="50252-171">**Примечание:** `/teams/allMessages` и `/chats/allMessages` в настоящее время находятся в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="50252-171">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="50252-172">Во время предварительной версии вы можете использовать этот API без сборов в соответствии с [условиями использования API Майкрософт](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="50252-172">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="50252-173">Однако пользователям приложений, использующих API, может потребоваться подписка на конкретные решения Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="50252-173">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="50252-174">После общедоступной доступности Корпорация Майкрософт может потребовать от вас или ваших клиентов взимать дополнительные сборы на основе объема данных, доступ к которым осуществляется через API.</span><span class="sxs-lookup"><span data-stu-id="50252-174">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem-onedrive"></a><span data-ttu-id="50252-175">driveItem (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="50252-175">driveItem (OneDrive)</span></span>

<span data-ttu-id="50252-176">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="50252-176">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="50252-177">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="50252-177">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="50252-178">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="50252-178">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="50252-179">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="50252-179">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="50252-180">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="50252-180">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="50252-181">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="50252-181">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message-outlook"></a><span data-ttu-id="50252-182">Contact, Event и Message (Outlook)</span><span class="sxs-lookup"><span data-stu-id="50252-182">contact, event, and message (Outlook)</span></span>

<span data-ttu-id="50252-183">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="50252-183">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="50252-184">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="50252-184">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="50252-185">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="50252-185">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="50252-186">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="50252-186">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="50252-187">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="50252-187">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="50252-188">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="50252-188">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="50252-189">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="50252-189">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="50252-190">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50252-190">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="50252-191">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50252-191">Request headers</span></span>

| <span data-ttu-id="50252-192">Имя</span><span class="sxs-lookup"><span data-stu-id="50252-192">Name</span></span>       | <span data-ttu-id="50252-193">Тип</span><span class="sxs-lookup"><span data-stu-id="50252-193">Type</span></span> | <span data-ttu-id="50252-194">Описание</span><span class="sxs-lookup"><span data-stu-id="50252-194">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="50252-195">Authorization</span><span class="sxs-lookup"><span data-stu-id="50252-195">Authorization</span></span>  | <span data-ttu-id="50252-196">string</span><span class="sxs-lookup"><span data-stu-id="50252-196">string</span></span>  | <span data-ttu-id="50252-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50252-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="50252-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="50252-199">Response</span></span>

<span data-ttu-id="50252-200">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50252-200">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50252-201">Пример</span><span class="sxs-lookup"><span data-stu-id="50252-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="50252-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="50252-202">Request</span></span>

<span data-ttu-id="50252-203">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50252-203">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="50252-204">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="50252-204">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="50252-205">Этот запрос создает подписку на уведомления о новых сообщениях, получаемых пользователем, который вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="50252-205">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="50252-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="50252-206">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="50252-207">C#</span><span class="sxs-lookup"><span data-stu-id="50252-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50252-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50252-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50252-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50252-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="50252-210">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="50252-210">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="50252-211">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="50252-211">Resource type</span></span> | <span data-ttu-id="50252-212">Примеры</span><span class="sxs-lookup"><span data-stu-id="50252-212">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="50252-213">Mail</span><span class="sxs-lookup"><span data-stu-id="50252-213">Mail</span></span>|<span data-ttu-id="50252-214">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="50252-214">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="50252-215">me/messages</span><span class="sxs-lookup"><span data-stu-id="50252-215">me/messages</span></span>|
|<span data-ttu-id="50252-216">Contacts</span><span class="sxs-lookup"><span data-stu-id="50252-216">Contacts</span></span>|<span data-ttu-id="50252-217">me/contacts</span><span class="sxs-lookup"><span data-stu-id="50252-217">me/contacts</span></span>|
|<span data-ttu-id="50252-218">Calendars</span><span class="sxs-lookup"><span data-stu-id="50252-218">Calendars</span></span>|<span data-ttu-id="50252-219">me/events</span><span class="sxs-lookup"><span data-stu-id="50252-219">me/events</span></span>|
|<span data-ttu-id="50252-220">Users</span><span class="sxs-lookup"><span data-stu-id="50252-220">Users</span></span>|<span data-ttu-id="50252-221">users</span><span class="sxs-lookup"><span data-stu-id="50252-221">users</span></span>|
|<span data-ttu-id="50252-222">Groups</span><span class="sxs-lookup"><span data-stu-id="50252-222">Groups</span></span>|<span data-ttu-id="50252-223">groups</span><span class="sxs-lookup"><span data-stu-id="50252-223">groups</span></span>|
|<span data-ttu-id="50252-224">Conversations</span><span class="sxs-lookup"><span data-stu-id="50252-224">Conversations</span></span>|<span data-ttu-id="50252-225">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="50252-225">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="50252-226">Drives</span><span class="sxs-lookup"><span data-stu-id="50252-226">Drives</span></span>|<span data-ttu-id="50252-227">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="50252-227">me/drive/root</span></span>|
|<span data-ttu-id="50252-228">Security alert</span><span class="sxs-lookup"><span data-stu-id="50252-228">Security alert</span></span>|<span data-ttu-id="50252-229">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="50252-229">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="50252-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="50252-230">Response</span></span>

<span data-ttu-id="50252-231">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="50252-231">The following example shows the response.</span></span> 

><span data-ttu-id="50252-p111">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50252-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="50252-234">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="50252-234">Notification endpoint validation</span></span>

<span data-ttu-id="50252-235">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="50252-235">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="50252-236">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="50252-236">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
