---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: d07ca13bf0c455bf4df9fd69a7006fad663f38bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044349"
---
# <a name="delete-subscription"></a><span data-ttu-id="6939e-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="6939e-103">Delete subscription</span></span>

<span data-ttu-id="6939e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6939e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6939e-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="6939e-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6939e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6939e-106">Permissions</span></span>

<span data-ttu-id="6939e-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6939e-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6939e-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6939e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6939e-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="6939e-109">Supported resource</span></span> | <span data-ttu-id="6939e-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6939e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6939e-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6939e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6939e-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="6939e-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6939e-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="6939e-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="6939e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-114">Not supported</span></span> | <span data-ttu-id="6939e-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-115">Not supported</span></span> | <span data-ttu-id="6939e-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="6939e-117">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="6939e-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6939e-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6939e-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="6939e-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-119">Not supported</span></span> | <span data-ttu-id="6939e-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6939e-121">[chatMessage](../resources/chatmessage.md) (/теамс/аллмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="6939e-121">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6939e-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-122">Not supported</span></span> | <span data-ttu-id="6939e-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-123">Not supported</span></span> | <span data-ttu-id="6939e-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6939e-125">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="6939e-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6939e-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6939e-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="6939e-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-127">Not supported</span></span> | <span data-ttu-id="6939e-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="6939e-129">[chatMessage](../resources/chatmessage.md) (/ЧАТС/аллмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="6939e-129">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6939e-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-130">Not supported</span></span> | <span data-ttu-id="6939e-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-131">Not supported</span></span> | <span data-ttu-id="6939e-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6939e-133">contact</span><span class="sxs-lookup"><span data-stu-id="6939e-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6939e-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-134">Contacts.Read</span></span> | <span data-ttu-id="6939e-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-135">Contacts.Read</span></span> | <span data-ttu-id="6939e-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-136">Contacts.Read</span></span> |
|<span data-ttu-id="6939e-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="6939e-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6939e-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-138">Not supported</span></span> | <span data-ttu-id="6939e-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6939e-139">Files.ReadWrite</span></span> | <span data-ttu-id="6939e-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-140">Not supported</span></span> |
|<span data-ttu-id="6939e-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6939e-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6939e-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6939e-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="6939e-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-143">Not supported</span></span> | <span data-ttu-id="6939e-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6939e-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6939e-145">event</span><span class="sxs-lookup"><span data-stu-id="6939e-145">event</span></span>](../resources/event.md) | <span data-ttu-id="6939e-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-146">Calendars.Read</span></span> | <span data-ttu-id="6939e-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-147">Calendars.Read</span></span> | <span data-ttu-id="6939e-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-148">Calendars.Read</span></span> |
|[<span data-ttu-id="6939e-149">group</span><span class="sxs-lookup"><span data-stu-id="6939e-149">group</span></span>](../resources/group.md) | <span data-ttu-id="6939e-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-150">Group.Read.All</span></span> | <span data-ttu-id="6939e-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-151">Not supported</span></span> | <span data-ttu-id="6939e-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-152">Group.Read.All</span></span> |
|[<span data-ttu-id="6939e-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="6939e-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6939e-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-154">Group.Read.All</span></span> | <span data-ttu-id="6939e-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-155">Not supported</span></span> | <span data-ttu-id="6939e-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-156">Not supported</span></span> |
|[<span data-ttu-id="6939e-157">list</span><span class="sxs-lookup"><span data-stu-id="6939e-157">list</span></span>](../resources/list.md) | <span data-ttu-id="6939e-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6939e-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6939e-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-159">Not supported</span></span> | <span data-ttu-id="6939e-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6939e-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6939e-161">message</span><span class="sxs-lookup"><span data-stu-id="6939e-161">message</span></span>](../resources/message.md) | <span data-ttu-id="6939e-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6939e-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6939e-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6939e-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6939e-165">presence</span><span class="sxs-lookup"><span data-stu-id="6939e-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="6939e-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-166">Presence.Read.All</span></span> | <span data-ttu-id="6939e-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-167">Not supported</span></span> | <span data-ttu-id="6939e-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-168">Not supported</span></span> |
|[<span data-ttu-id="6939e-169">security alert</span><span class="sxs-lookup"><span data-stu-id="6939e-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6939e-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6939e-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6939e-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6939e-171">Not supported</span></span> | <span data-ttu-id="6939e-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6939e-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6939e-173">user</span><span class="sxs-lookup"><span data-stu-id="6939e-173">user</span></span>](../resources/user.md) | <span data-ttu-id="6939e-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-174">User.Read.All</span></span> | <span data-ttu-id="6939e-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-175">User.Read.All</span></span> | <span data-ttu-id="6939e-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6939e-176">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="6939e-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6939e-177">chatMessage</span></span>

<span data-ttu-id="6939e-178">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов (**инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="6939e-178">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="6939e-179">подписки **chatMessage** с разрешениями приложений включают данные ресурсов и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="6939e-179">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="6939e-180">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="6939e-180">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="6939e-181">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="6939e-181">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="6939e-182">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="6939e-182">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="6939e-183">**Примечание:** `/teams/allMessages` и `/chats/allMessages` в настоящее время находятся в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="6939e-183">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="6939e-184">Во время предварительной версии вы можете использовать этот API без сборов в соответствии с [условиями использования API Майкрософт](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="6939e-184">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="6939e-185">Однако пользователям приложений, использующих API, может потребоваться подписка на конкретные решения Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6939e-185">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="6939e-186">После общедоступной доступности Корпорация Майкрософт может потребовать от вас или ваших клиентов взимать дополнительные сборы на основе объема данных, доступ к которым осуществляется через API.</span><span class="sxs-lookup"><span data-stu-id="6939e-186">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="6939e-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="6939e-187">driveItem</span></span>

<span data-ttu-id="6939e-188">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6939e-188">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="6939e-189">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="6939e-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6939e-190">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="6939e-190">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6939e-191">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="6939e-191">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6939e-192">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="6939e-192">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6939e-193">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="6939e-193">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6939e-194">контакты, события и сообщения</span><span class="sxs-lookup"><span data-stu-id="6939e-194">contact, event, and message</span></span>

<span data-ttu-id="6939e-195">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="6939e-195">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6939e-196">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="6939e-196">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6939e-197">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="6939e-197">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6939e-198">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6939e-198">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6939e-199">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="6939e-199">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6939e-200">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6939e-200">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6939e-201">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="6939e-201">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="6939e-202">presence</span><span class="sxs-lookup"><span data-stu-id="6939e-202">presence</span></span>

<span data-ttu-id="6939e-203">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="6939e-203">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="6939e-204">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="6939e-204">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="6939e-205">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6939e-205">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6939e-206">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6939e-206">Request headers</span></span>

| <span data-ttu-id="6939e-207">Имя</span><span class="sxs-lookup"><span data-stu-id="6939e-207">Name</span></span>       | <span data-ttu-id="6939e-208">Тип</span><span class="sxs-lookup"><span data-stu-id="6939e-208">Type</span></span> | <span data-ttu-id="6939e-209">Описание</span><span class="sxs-lookup"><span data-stu-id="6939e-209">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6939e-210">Authorization</span><span class="sxs-lookup"><span data-stu-id="6939e-210">Authorization</span></span>  | <span data-ttu-id="6939e-211">string</span><span class="sxs-lookup"><span data-stu-id="6939e-211">string</span></span>  | <span data-ttu-id="6939e-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6939e-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6939e-214">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6939e-214">Request body</span></span>

<span data-ttu-id="6939e-215">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6939e-215">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6939e-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="6939e-216">Response</span></span>

<span data-ttu-id="6939e-217">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6939e-217">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="6939e-218">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="6939e-218">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="6939e-219">Пример</span><span class="sxs-lookup"><span data-stu-id="6939e-219">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6939e-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="6939e-220">Request</span></span>

<span data-ttu-id="6939e-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6939e-221">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6939e-222">HTTP</span><span class="sxs-lookup"><span data-stu-id="6939e-222">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="6939e-223">C#</span><span class="sxs-lookup"><span data-stu-id="6939e-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6939e-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6939e-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6939e-225">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6939e-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6939e-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="6939e-226">Response</span></span>

<span data-ttu-id="6939e-227">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6939e-227">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


