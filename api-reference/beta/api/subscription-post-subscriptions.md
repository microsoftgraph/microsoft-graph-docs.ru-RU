---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: e199e2c9fa0240eda593843d88490e7f22b0f506
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744082"
---
# <a name="create-subscription"></a><span data-ttu-id="8b9ca-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="8b9ca-103">Create subscription</span></span>

<span data-ttu-id="8b9ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b9ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b9ca-105">Подписывает приложение прослушивателя на получение уведомлений об изменениях, когда запрошенный тип изменений выполняется для указанного ресурса в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b9ca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b9ca-106">Permissions</span></span>

<span data-ttu-id="8b9ca-107">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="8b9ca-108">Например, чтобы получать уведомления об изменениях для сообщений, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="8b9ca-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8b9ca-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b9ca-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b9ca-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="8b9ca-111">Supported resource</span></span> | <span data-ttu-id="8b9ca-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b9ca-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b9ca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b9ca-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="8b9ca-115">[каллрекорд](../resources/callrecords-callrecord.md) (/коммуникатионс/каллрекордс)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="8b9ca-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-116">Not supported</span></span> | <span data-ttu-id="8b9ca-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-117">Not supported</span></span> | <span data-ttu-id="8b9ca-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="8b9ca-119">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="8b9ca-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-120">Not supported</span></span> | <span data-ttu-id="8b9ca-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-121">Not supported</span></span> | <span data-ttu-id="8b9ca-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8b9ca-123">[chatMessage](../resources/chatmessage.md) (/теамс/аллмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-123">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="8b9ca-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-124">Not supported</span></span> | <span data-ttu-id="8b9ca-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-125">Not supported</span></span> | <span data-ttu-id="8b9ca-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8b9ca-127">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="8b9ca-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-128">Not supported</span></span> | <span data-ttu-id="8b9ca-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-129">Not supported</span></span> | <span data-ttu-id="8b9ca-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="8b9ca-131">[chatMessage](../resources/chatmessage.md) (/ЧАТС/аллмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-131">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="8b9ca-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-132">Not supported</span></span> | <span data-ttu-id="8b9ca-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-133">Not supported</span></span> | <span data-ttu-id="8b9ca-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="8b9ca-135">contact</span><span class="sxs-lookup"><span data-stu-id="8b9ca-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="8b9ca-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-136">Contacts.Read</span></span> | <span data-ttu-id="8b9ca-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-137">Contacts.Read</span></span> | <span data-ttu-id="8b9ca-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-138">Contacts.Read</span></span> |
|<span data-ttu-id="8b9ca-139">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="8b9ca-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-140">Not supported</span></span> | <span data-ttu-id="8b9ca-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b9ca-141">Files.ReadWrite</span></span> | <span data-ttu-id="8b9ca-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-142">Not supported</span></span> |
|<span data-ttu-id="8b9ca-143">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="8b9ca-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="8b9ca-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-145">Not supported</span></span> | <span data-ttu-id="8b9ca-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b9ca-147">event</span><span class="sxs-lookup"><span data-stu-id="8b9ca-147">event</span></span>](../resources/event.md) | <span data-ttu-id="8b9ca-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-148">Calendars.Read</span></span> | <span data-ttu-id="8b9ca-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-149">Calendars.Read</span></span> | <span data-ttu-id="8b9ca-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-150">Calendars.Read</span></span> |
|[<span data-ttu-id="8b9ca-151">group</span><span class="sxs-lookup"><span data-stu-id="8b9ca-151">group</span></span>](../resources/group.md) | <span data-ttu-id="8b9ca-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-152">Group.Read.All</span></span> | <span data-ttu-id="8b9ca-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-153">Not supported</span></span> | <span data-ttu-id="8b9ca-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-154">Group.Read.All</span></span> |
|[<span data-ttu-id="8b9ca-155">group conversation</span><span class="sxs-lookup"><span data-stu-id="8b9ca-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="8b9ca-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-156">Group.Read.All</span></span> | <span data-ttu-id="8b9ca-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-157">Not supported</span></span> | <span data-ttu-id="8b9ca-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-158">Not supported</span></span> |
|[<span data-ttu-id="8b9ca-159">list</span><span class="sxs-lookup"><span data-stu-id="8b9ca-159">list</span></span>](../resources/list.md) | <span data-ttu-id="8b9ca-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="8b9ca-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-161">Not supported</span></span> | <span data-ttu-id="8b9ca-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b9ca-163">message</span><span class="sxs-lookup"><span data-stu-id="8b9ca-163">message</span></span>](../resources/message.md) | <span data-ttu-id="8b9ca-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8b9ca-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8b9ca-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b9ca-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="8b9ca-167">security alert</span><span class="sxs-lookup"><span data-stu-id="8b9ca-167">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="8b9ca-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-168">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="8b9ca-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b9ca-169">Not supported</span></span> | <span data-ttu-id="8b9ca-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-170">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b9ca-171">user</span><span class="sxs-lookup"><span data-stu-id="8b9ca-171">user</span></span>](../resources/user.md) | <span data-ttu-id="8b9ca-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-172">User.Read.All</span></span> | <span data-ttu-id="8b9ca-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-173">User.Read.All</span></span> | <span data-ttu-id="8b9ca-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9ca-174">User.Read.All</span></span> |

### <a name="chatmessage-microsoft-teams"></a><span data-ttu-id="8b9ca-175">chatMessage (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-175">chatMessage (Microsoft Teams)</span></span>

<span data-ttu-id="8b9ca-176">для подписок на **chatMessage** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="8b9ca-176">**chatMessage** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="8b9ca-177">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-177">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="8b9ca-178">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-178">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="8b9ca-179">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="8b9ca-179">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="8b9ca-180">**Примечание:** `/teams/allMessages` и `/chats/allMessages` в настоящее время находятся в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-180">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="8b9ca-181">Во время предварительной версии вы можете использовать этот API без сборов в соответствии с [условиями использования API Майкрософт](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="8b9ca-181">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="8b9ca-182">Однако пользователям приложений, использующих API, может потребоваться подписка на конкретные решения Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-182">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="8b9ca-183">После общедоступной доступности Корпорация Майкрософт может потребовать от вас или ваших клиентов взимать дополнительные сборы на основе объема данных, доступ к которым осуществляется через API.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-183">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem-onedrive"></a><span data-ttu-id="8b9ca-184">driveItem (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-184">driveItem (OneDrive)</span></span>

<span data-ttu-id="8b9ca-185">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-185">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="8b9ca-186">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="8b9ca-187">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-187">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="8b9ca-188">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-188">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="8b9ca-189">Уведомления об изменениях отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других экземпляров **driveItem** в иерархии.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-189">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="8b9ca-190">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-190">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message-outlook"></a><span data-ttu-id="8b9ca-191">Contact, Event и Message (Outlook)</span><span class="sxs-lookup"><span data-stu-id="8b9ca-191">contact, event, and message (Outlook)</span></span>

<span data-ttu-id="8b9ca-192">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-192">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="8b9ca-193">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="8b9ca-194">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-194">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="8b9ca-195">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-195">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="8b9ca-196">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="8b9ca-196">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="8b9ca-197">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-197">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="8b9ca-198">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-198">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="8b9ca-199">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b9ca-199">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="8b9ca-200">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b9ca-200">Request headers</span></span>

| <span data-ttu-id="8b9ca-201">Имя</span><span class="sxs-lookup"><span data-stu-id="8b9ca-201">Name</span></span>       | <span data-ttu-id="8b9ca-202">Тип</span><span class="sxs-lookup"><span data-stu-id="8b9ca-202">Type</span></span> | <span data-ttu-id="8b9ca-203">Описание</span><span class="sxs-lookup"><span data-stu-id="8b9ca-203">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8b9ca-204">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b9ca-204">Authorization</span></span>  | <span data-ttu-id="8b9ca-205">string</span><span class="sxs-lookup"><span data-stu-id="8b9ca-205">string</span></span>  | <span data-ttu-id="8b9ca-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8b9ca-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b9ca-208">Response</span></span>

<span data-ttu-id="8b9ca-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-209">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="8b9ca-210">Сведения о том, как возвращаются ошибки, приведены в разделе [ошибочные ответы][error-response].</span><span class="sxs-lookup"><span data-stu-id="8b9ca-210">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="8b9ca-211">Пример</span><span class="sxs-lookup"><span data-stu-id="8b9ca-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b9ca-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b9ca-212">Request</span></span>

<span data-ttu-id="8b9ca-213">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-213">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="8b9ca-214">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-214">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="8b9ca-215">Этот запрос создает подписку на уведомления об изменениях новой почты, полученной в текущий момент, когда пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-215">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b9ca-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b9ca-216">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b9ca-217">C#</span><span class="sxs-lookup"><span data-stu-id="8b9ca-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b9ca-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b9ca-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b9ca-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b9ca-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="8b9ca-220">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-220">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="8b9ca-221">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="8b9ca-221">Resource type</span></span> | <span data-ttu-id="8b9ca-222">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b9ca-222">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="8b9ca-223">Mail</span><span class="sxs-lookup"><span data-stu-id="8b9ca-223">Mail</span></span>|<span data-ttu-id="8b9ca-224">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="8b9ca-224">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="8b9ca-225">me/messages</span><span class="sxs-lookup"><span data-stu-id="8b9ca-225">me/messages</span></span>|
|<span data-ttu-id="8b9ca-226">Contacts</span><span class="sxs-lookup"><span data-stu-id="8b9ca-226">Contacts</span></span>|<span data-ttu-id="8b9ca-227">me/contacts</span><span class="sxs-lookup"><span data-stu-id="8b9ca-227">me/contacts</span></span>|
|<span data-ttu-id="8b9ca-228">Calendars</span><span class="sxs-lookup"><span data-stu-id="8b9ca-228">Calendars</span></span>|<span data-ttu-id="8b9ca-229">me/events</span><span class="sxs-lookup"><span data-stu-id="8b9ca-229">me/events</span></span>|
|<span data-ttu-id="8b9ca-230">Users</span><span class="sxs-lookup"><span data-stu-id="8b9ca-230">Users</span></span>|<span data-ttu-id="8b9ca-231">users</span><span class="sxs-lookup"><span data-stu-id="8b9ca-231">users</span></span>|
|<span data-ttu-id="8b9ca-232">Groups</span><span class="sxs-lookup"><span data-stu-id="8b9ca-232">Groups</span></span>|<span data-ttu-id="8b9ca-233">groups</span><span class="sxs-lookup"><span data-stu-id="8b9ca-233">groups</span></span>|
|<span data-ttu-id="8b9ca-234">Conversations</span><span class="sxs-lookup"><span data-stu-id="8b9ca-234">Conversations</span></span>|<span data-ttu-id="8b9ca-235">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="8b9ca-235">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="8b9ca-236">Drives</span><span class="sxs-lookup"><span data-stu-id="8b9ca-236">Drives</span></span>|<span data-ttu-id="8b9ca-237">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="8b9ca-237">me/drive/root</span></span>|
|<span data-ttu-id="8b9ca-238">Список</span><span class="sxs-lookup"><span data-stu-id="8b9ca-238">List</span></span>|<span data-ttu-id="8b9ca-239">sites/{site-id}/lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="8b9ca-239">sites/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="8b9ca-240">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="8b9ca-240">Security alert</span></span>|<span data-ttu-id="8b9ca-241">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="8b9ca-241">security/alerts?$filter=status eq ‘New’</span></span>|
|<span data-ttu-id="8b9ca-242">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="8b9ca-242">Call records</span></span>|<span data-ttu-id="8b9ca-243">связь/Каллрекордс</span><span class="sxs-lookup"><span data-stu-id="8b9ca-243">communications/callRecords</span></span>|
|[<span data-ttu-id="8b9ca-244">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="8b9ca-244">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8b9ca-245">Chats/{ID}/messages, Chats/Аллмессажес, Teams/{ID}/channels/{ID}/messages, Teams/Аллмессажес</span><span class="sxs-lookup"><span data-stu-id="8b9ca-245">chats/{id}/messages, chats/allMessages, teams/{id}/channels/{id}/messages, teams/allMessages</span></span> |

### <a name="response"></a><span data-ttu-id="8b9ca-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b9ca-246">Response</span></span>

<span data-ttu-id="8b9ca-247">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-247">The following example shows the response.</span></span> 

><span data-ttu-id="8b9ca-p111">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b9ca-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="8b9ca-250">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="8b9ca-250">Notification endpoint validation</span></span>

<span data-ttu-id="8b9ca-251">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="8b9ca-251">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="8b9ca-252">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="8b9ca-252">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

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
