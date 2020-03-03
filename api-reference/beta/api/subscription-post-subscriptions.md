---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6bb11e36b2a5f11f94cea7294e77e6d23aa8dd54
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394479"
---
# <a name="create-subscription"></a><span data-ttu-id="256ac-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="256ac-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="256ac-104">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении нужного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="256ac-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="256ac-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="256ac-105">Permissions</span></span>

<span data-ttu-id="256ac-106">Для создания подписки необходимо разрешение на чтение ресурса.</span><span class="sxs-lookup"><span data-stu-id="256ac-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="256ac-107">Например, чтобы получать уведомления о сообщениях, вашему приложению требуется разрешение mail. Read.</span><span class="sxs-lookup"><span data-stu-id="256ac-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="256ac-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="256ac-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="256ac-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="256ac-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="256ac-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="256ac-110">Supported resource</span></span> | <span data-ttu-id="256ac-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="256ac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="256ac-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="256ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="256ac-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="256ac-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="256ac-114">[каллрекорд](../resources/callrecords-callrecord.md) (/коммуникатионс/каллрекордс)</span><span class="sxs-lookup"><span data-stu-id="256ac-114">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="256ac-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-115">Not supported</span></span> | <span data-ttu-id="256ac-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-116">Not supported</span></span> | <span data-ttu-id="256ac-117">Каллрекордс. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="256ac-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="256ac-118">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="256ac-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="256ac-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-119">Not supported</span></span> | <span data-ttu-id="256ac-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-120">Not supported</span></span> | <span data-ttu-id="256ac-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-121">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="256ac-122">[chatMessage](../resources/chatmessage.md) (/теамс/аллмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="256ac-122">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="256ac-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-123">Not supported</span></span> | <span data-ttu-id="256ac-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-124">Not supported</span></span> | <span data-ttu-id="256ac-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="256ac-126">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="256ac-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="256ac-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-127">Not supported</span></span> | <span data-ttu-id="256ac-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-128">Not supported</span></span> | <span data-ttu-id="256ac-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="256ac-130">[chatMessage](../resources/chatmessage.md) (/ЧАТС/аллмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="256ac-130">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="256ac-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-131">Not supported</span></span> | <span data-ttu-id="256ac-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-132">Not supported</span></span> | <span data-ttu-id="256ac-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="256ac-134">contact</span><span class="sxs-lookup"><span data-stu-id="256ac-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="256ac-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-135">Contacts.Read</span></span> | <span data-ttu-id="256ac-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-136">Contacts.Read</span></span> | <span data-ttu-id="256ac-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-137">Contacts.Read</span></span> |
|<span data-ttu-id="256ac-138">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="256ac-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="256ac-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-139">Not supported</span></span> | <span data-ttu-id="256ac-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="256ac-140">Files.ReadWrite</span></span> | <span data-ttu-id="256ac-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-141">Not supported</span></span> |
|<span data-ttu-id="256ac-142">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="256ac-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="256ac-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256ac-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="256ac-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-144">Not supported</span></span> | <span data-ttu-id="256ac-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256ac-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="256ac-146">event</span><span class="sxs-lookup"><span data-stu-id="256ac-146">event</span></span>](../resources/event.md) | <span data-ttu-id="256ac-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-147">Calendars.Read</span></span> | <span data-ttu-id="256ac-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-148">Calendars.Read</span></span> | <span data-ttu-id="256ac-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-149">Calendars.Read</span></span> |
|[<span data-ttu-id="256ac-150">group</span><span class="sxs-lookup"><span data-stu-id="256ac-150">group</span></span>](../resources/group.md) | <span data-ttu-id="256ac-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-151">Group.Read.All</span></span> | <span data-ttu-id="256ac-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-152">Not supported</span></span> | <span data-ttu-id="256ac-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-153">Group.Read.All</span></span> |
|[<span data-ttu-id="256ac-154">group conversation</span><span class="sxs-lookup"><span data-stu-id="256ac-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="256ac-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-155">Group.Read.All</span></span> | <span data-ttu-id="256ac-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-156">Not supported</span></span> | <span data-ttu-id="256ac-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-157">Not supported</span></span> |
|[<span data-ttu-id="256ac-158">list</span><span class="sxs-lookup"><span data-stu-id="256ac-158">list</span></span>](../resources/list.md) | <span data-ttu-id="256ac-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256ac-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="256ac-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-160">Not supported</span></span> | <span data-ttu-id="256ac-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256ac-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="256ac-162">message</span><span class="sxs-lookup"><span data-stu-id="256ac-162">message</span></span>](../resources/message.md) | <span data-ttu-id="256ac-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="256ac-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="256ac-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="256ac-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="256ac-166">security alert</span><span class="sxs-lookup"><span data-stu-id="256ac-166">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="256ac-167">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256ac-167">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="256ac-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="256ac-168">Not supported</span></span> | <span data-ttu-id="256ac-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="256ac-169">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="256ac-170">user</span><span class="sxs-lookup"><span data-stu-id="256ac-170">user</span></span>](../resources/user.md) | <span data-ttu-id="256ac-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-171">User.Read.All</span></span> | <span data-ttu-id="256ac-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-172">User.Read.All</span></span> | <span data-ttu-id="256ac-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="256ac-173">User.Read.All</span></span> |

### <a name="chatmessage-microsoft-teams"></a><span data-ttu-id="256ac-174">chatMessage (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="256ac-174">chatMessage (Microsoft Teams)</span></span>

<span data-ttu-id="256ac-175">для подписок на **chatMessage** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="256ac-175">**chatMessage** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="256ac-176">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="256ac-176">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="256ac-177">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="256ac-177">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="256ac-178">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="256ac-178">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="256ac-179">**Примечание:** `/teams/allMessages` и `/chats/allMessages` в настоящее время находятся в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="256ac-179">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="256ac-180">Во время предварительной версии вы можете использовать этот API без сборов в соответствии с [условиями использования API Майкрософт](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="256ac-180">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="256ac-181">Однако пользователям приложений, использующих API, может потребоваться подписка на конкретные решения Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="256ac-181">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="256ac-182">После общедоступной доступности Корпорация Майкрософт может потребовать от вас или ваших клиентов взимать дополнительные сборы на основе объема данных, доступ к которым осуществляется через API.</span><span class="sxs-lookup"><span data-stu-id="256ac-182">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem-onedrive"></a><span data-ttu-id="256ac-183">driveItem (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="256ac-183">driveItem (OneDrive)</span></span>

<span data-ttu-id="256ac-184">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="256ac-184">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="256ac-185">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="256ac-185">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="256ac-186">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="256ac-186">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="256ac-187">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="256ac-187">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="256ac-188">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="256ac-188">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="256ac-189">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="256ac-189">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message-outlook"></a><span data-ttu-id="256ac-190">Contact, Event и Message (Outlook)</span><span class="sxs-lookup"><span data-stu-id="256ac-190">contact, event, and message (Outlook)</span></span>

<span data-ttu-id="256ac-191">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="256ac-191">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="256ac-192">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="256ac-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="256ac-193">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="256ac-193">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="256ac-194">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="256ac-194">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="256ac-195">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="256ac-195">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="256ac-196">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="256ac-196">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="256ac-197">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="256ac-197">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="256ac-198">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="256ac-198">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="256ac-199">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="256ac-199">Request headers</span></span>

| <span data-ttu-id="256ac-200">Имя</span><span class="sxs-lookup"><span data-stu-id="256ac-200">Name</span></span>       | <span data-ttu-id="256ac-201">Тип</span><span class="sxs-lookup"><span data-stu-id="256ac-201">Type</span></span> | <span data-ttu-id="256ac-202">Описание</span><span class="sxs-lookup"><span data-stu-id="256ac-202">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="256ac-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="256ac-203">Authorization</span></span>  | <span data-ttu-id="256ac-204">string</span><span class="sxs-lookup"><span data-stu-id="256ac-204">string</span></span>  | <span data-ttu-id="256ac-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="256ac-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="256ac-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="256ac-207">Response</span></span>

<span data-ttu-id="256ac-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="256ac-208">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="256ac-209">Пример</span><span class="sxs-lookup"><span data-stu-id="256ac-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="256ac-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="256ac-210">Request</span></span>

<span data-ttu-id="256ac-211">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="256ac-211">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="256ac-212">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="256ac-212">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="256ac-213">Этот запрос создает подписку на уведомления о новых сообщениях, получаемых пользователем, который вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="256ac-213">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="256ac-214">HTTP</span><span class="sxs-lookup"><span data-stu-id="256ac-214">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="256ac-215">C#</span><span class="sxs-lookup"><span data-stu-id="256ac-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="256ac-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="256ac-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="256ac-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="256ac-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="256ac-218">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="256ac-218">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="256ac-219">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="256ac-219">Resource type</span></span> | <span data-ttu-id="256ac-220">Примеры</span><span class="sxs-lookup"><span data-stu-id="256ac-220">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="256ac-221">Mail</span><span class="sxs-lookup"><span data-stu-id="256ac-221">Mail</span></span>|<span data-ttu-id="256ac-222">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="256ac-222">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="256ac-223">me/messages</span><span class="sxs-lookup"><span data-stu-id="256ac-223">me/messages</span></span>|
|<span data-ttu-id="256ac-224">Contacts</span><span class="sxs-lookup"><span data-stu-id="256ac-224">Contacts</span></span>|<span data-ttu-id="256ac-225">me/contacts</span><span class="sxs-lookup"><span data-stu-id="256ac-225">me/contacts</span></span>|
|<span data-ttu-id="256ac-226">Calendars</span><span class="sxs-lookup"><span data-stu-id="256ac-226">Calendars</span></span>|<span data-ttu-id="256ac-227">me/events</span><span class="sxs-lookup"><span data-stu-id="256ac-227">me/events</span></span>|
|<span data-ttu-id="256ac-228">Users</span><span class="sxs-lookup"><span data-stu-id="256ac-228">Users</span></span>|<span data-ttu-id="256ac-229">users</span><span class="sxs-lookup"><span data-stu-id="256ac-229">users</span></span>|
|<span data-ttu-id="256ac-230">Groups</span><span class="sxs-lookup"><span data-stu-id="256ac-230">Groups</span></span>|<span data-ttu-id="256ac-231">groups</span><span class="sxs-lookup"><span data-stu-id="256ac-231">groups</span></span>|
|<span data-ttu-id="256ac-232">Conversations</span><span class="sxs-lookup"><span data-stu-id="256ac-232">Conversations</span></span>|<span data-ttu-id="256ac-233">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="256ac-233">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="256ac-234">Drives</span><span class="sxs-lookup"><span data-stu-id="256ac-234">Drives</span></span>|<span data-ttu-id="256ac-235">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="256ac-235">me/drive/root</span></span>|
|<span data-ttu-id="256ac-236">Список</span><span class="sxs-lookup"><span data-stu-id="256ac-236">List</span></span>|<span data-ttu-id="256ac-237">Site/{site-ID}/Lists/{List-ID}</span><span class="sxs-lookup"><span data-stu-id="256ac-237">site/{site-id}/lists/{list-id}</span></span>|
|<span data-ttu-id="256ac-238">Security alert</span><span class="sxs-lookup"><span data-stu-id="256ac-238">Security alert</span></span>|<span data-ttu-id="256ac-239">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="256ac-239">security/alerts?$filter=status eq ‘New’</span></span>|
|<span data-ttu-id="256ac-240">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="256ac-240">Call records</span></span>|<span data-ttu-id="256ac-241">связь/Каллрекордс</span><span class="sxs-lookup"><span data-stu-id="256ac-241">communications/callRecords</span></span>|

### <a name="response"></a><span data-ttu-id="256ac-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="256ac-242">Response</span></span>

<span data-ttu-id="256ac-243">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="256ac-243">The following example shows the response.</span></span> 

><span data-ttu-id="256ac-p111">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="256ac-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="256ac-246">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="256ac-246">Notification endpoint validation</span></span>

<span data-ttu-id="256ac-247">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="256ac-247">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="256ac-248">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="256ac-248">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
