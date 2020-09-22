---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 08166c2570c6c73fbb412a4713b5669b36e57736
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193320"
---
# <a name="delete-subscription"></a><span data-ttu-id="138bd-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="138bd-103">Delete subscription</span></span>

<span data-ttu-id="138bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="138bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="138bd-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="138bd-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="138bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="138bd-106">Permissions</span></span>

<span data-ttu-id="138bd-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="138bd-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="138bd-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="138bd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="138bd-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="138bd-109">Supported resource</span></span> | <span data-ttu-id="138bd-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="138bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="138bd-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="138bd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="138bd-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="138bd-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="138bd-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="138bd-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="138bd-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-114">Not supported</span></span> | <span data-ttu-id="138bd-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-115">Not supported</span></span> | <span data-ttu-id="138bd-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="138bd-117">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="138bd-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="138bd-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="138bd-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-119">Not supported</span></span> | <span data-ttu-id="138bd-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="138bd-121">[chatMessage](../resources/chatmessage.md) (/теамс/жеталлмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="138bd-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="138bd-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-122">Not supported</span></span> | <span data-ttu-id="138bd-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-123">Not supported</span></span> | <span data-ttu-id="138bd-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="138bd-125">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="138bd-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="138bd-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="138bd-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="138bd-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-127">Not supported</span></span> | <span data-ttu-id="138bd-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="138bd-129">[chatMessage](../resources/chatmessage.md) (/ЧАТС/жеталлмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="138bd-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="138bd-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-130">Not supported</span></span> | <span data-ttu-id="138bd-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-131">Not supported</span></span> | <span data-ttu-id="138bd-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="138bd-133">contact</span><span class="sxs-lookup"><span data-stu-id="138bd-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="138bd-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-134">Contacts.Read</span></span> | <span data-ttu-id="138bd-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-135">Contacts.Read</span></span> | <span data-ttu-id="138bd-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-136">Contacts.Read</span></span> |
|<span data-ttu-id="138bd-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="138bd-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="138bd-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-138">Not supported</span></span> | <span data-ttu-id="138bd-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="138bd-139">Files.ReadWrite</span></span> | <span data-ttu-id="138bd-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-140">Not supported</span></span> |
|<span data-ttu-id="138bd-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="138bd-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="138bd-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="138bd-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-143">Not supported</span></span> | <span data-ttu-id="138bd-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="138bd-145">event</span><span class="sxs-lookup"><span data-stu-id="138bd-145">event</span></span>](../resources/event.md) | <span data-ttu-id="138bd-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-146">Calendars.Read</span></span> | <span data-ttu-id="138bd-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-147">Calendars.Read</span></span> | <span data-ttu-id="138bd-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-148">Calendars.Read</span></span> |
|[<span data-ttu-id="138bd-149">group</span><span class="sxs-lookup"><span data-stu-id="138bd-149">group</span></span>](../resources/group.md) | <span data-ttu-id="138bd-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-150">Group.Read.All</span></span> | <span data-ttu-id="138bd-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-151">Not supported</span></span> | <span data-ttu-id="138bd-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-152">Group.Read.All</span></span> |
|[<span data-ttu-id="138bd-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="138bd-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="138bd-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-154">Group.Read.All</span></span> | <span data-ttu-id="138bd-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-155">Not supported</span></span> | <span data-ttu-id="138bd-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-156">Not supported</span></span> |
|[<span data-ttu-id="138bd-157">list</span><span class="sxs-lookup"><span data-stu-id="138bd-157">list</span></span>](../resources/list.md) | <span data-ttu-id="138bd-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="138bd-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-159">Not supported</span></span> | <span data-ttu-id="138bd-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="138bd-161">message</span><span class="sxs-lookup"><span data-stu-id="138bd-161">message</span></span>](../resources/message.md) | <span data-ttu-id="138bd-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="138bd-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="138bd-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="138bd-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="138bd-165">presence</span><span class="sxs-lookup"><span data-stu-id="138bd-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="138bd-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-166">Presence.Read.All</span></span> | <span data-ttu-id="138bd-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-167">Not supported</span></span> | <span data-ttu-id="138bd-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-168">Not supported</span></span> |
|[<span data-ttu-id="138bd-169">security alert</span><span class="sxs-lookup"><span data-stu-id="138bd-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="138bd-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="138bd-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="138bd-171">Not supported</span></span> | <span data-ttu-id="138bd-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="138bd-173">user</span><span class="sxs-lookup"><span data-stu-id="138bd-173">user</span></span>](../resources/user.md) | <span data-ttu-id="138bd-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-174">User.Read.All</span></span> | <span data-ttu-id="138bd-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-175">User.Read.All</span></span> | <span data-ttu-id="138bd-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="138bd-176">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="138bd-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="138bd-177">chatMessage</span></span>

<span data-ttu-id="138bd-178">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов (**инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="138bd-178">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="138bd-179">подписки **chatMessage** с разрешениями приложений включают данные ресурсов и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="138bd-179">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="138bd-180">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="138bd-180">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="138bd-181">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="138bd-181">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="138bd-182">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="138bd-182">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="138bd-183">**Примечание:** `/teams/getAllMessages` и `/chats/getAllMessages` доступны пользователям, у которых есть  
 [необходимые лицензии](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="138bd-183">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="138bd-184">driveItem</span><span class="sxs-lookup"><span data-stu-id="138bd-184">driveItem</span></span>

<span data-ttu-id="138bd-185">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="138bd-185">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="138bd-186">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="138bd-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="138bd-187">В личном хранилище OneDrive можно подписаться на корневую папку или любую подпапку на этом диске.</span><span class="sxs-lookup"><span data-stu-id="138bd-187">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="138bd-188">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="138bd-188">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="138bd-189">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="138bd-189">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="138bd-190">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="138bd-190">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="138bd-191">контакты, события и сообщения</span><span class="sxs-lookup"><span data-stu-id="138bd-191">contact, event, and message</span></span>

<span data-ttu-id="138bd-192">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="138bd-192">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="138bd-193">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="138bd-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="138bd-194">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="138bd-194">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="138bd-195">Например, нельзя использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="138bd-195">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="138bd-196">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="138bd-196">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="138bd-197">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="138bd-197">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="138bd-198">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="138bd-198">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="138bd-199">presence</span><span class="sxs-lookup"><span data-stu-id="138bd-199">presence</span></span>

<span data-ttu-id="138bd-200">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="138bd-200">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="138bd-201">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="138bd-201">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="138bd-202">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="138bd-202">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="138bd-203">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="138bd-203">Request headers</span></span>

| <span data-ttu-id="138bd-204">Имя</span><span class="sxs-lookup"><span data-stu-id="138bd-204">Name</span></span>       | <span data-ttu-id="138bd-205">Тип</span><span class="sxs-lookup"><span data-stu-id="138bd-205">Type</span></span> | <span data-ttu-id="138bd-206">Описание</span><span class="sxs-lookup"><span data-stu-id="138bd-206">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="138bd-207">Authorization</span><span class="sxs-lookup"><span data-stu-id="138bd-207">Authorization</span></span>  | <span data-ttu-id="138bd-208">string</span><span class="sxs-lookup"><span data-stu-id="138bd-208">string</span></span>  | <span data-ttu-id="138bd-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="138bd-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="138bd-211">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="138bd-211">Request body</span></span>

<span data-ttu-id="138bd-212">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="138bd-212">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="138bd-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="138bd-213">Response</span></span>

<span data-ttu-id="138bd-214">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="138bd-214">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="138bd-215">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="138bd-215">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="138bd-216">Пример</span><span class="sxs-lookup"><span data-stu-id="138bd-216">Example</span></span>

##### <a name="request"></a><span data-ttu-id="138bd-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="138bd-217">Request</span></span>

<span data-ttu-id="138bd-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="138bd-218">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="138bd-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="138bd-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="138bd-220">C#</span><span class="sxs-lookup"><span data-stu-id="138bd-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="138bd-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="138bd-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="138bd-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="138bd-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="138bd-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="138bd-223">Response</span></span>

<span data-ttu-id="138bd-224">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="138bd-224">Here is an example of the response.</span></span>
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


