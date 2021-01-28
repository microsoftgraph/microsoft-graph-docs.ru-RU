---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b38975627a0a3c23b9e19acbb235c4bc26036918
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034266"
---
# <a name="delete-subscription"></a><span data-ttu-id="73030-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="73030-103">Delete subscription</span></span>

<span data-ttu-id="73030-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73030-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73030-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="73030-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="73030-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73030-106">Permissions</span></span>

<span data-ttu-id="73030-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="73030-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="73030-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73030-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73030-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="73030-109">Supported resource</span></span> | <span data-ttu-id="73030-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73030-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73030-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73030-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73030-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="73030-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="73030-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="73030-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="73030-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-114">Not supported</span></span> | <span data-ttu-id="73030-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-115">Not supported</span></span> | <span data-ttu-id="73030-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="73030-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="73030-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="73030-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="73030-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-119">Not supported</span></span> | <span data-ttu-id="73030-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="73030-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="73030-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="73030-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-122">Not supported</span></span> | <span data-ttu-id="73030-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-123">Not supported</span></span> | <span data-ttu-id="73030-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="73030-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="73030-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="73030-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73030-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="73030-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-127">Not supported</span></span> | <span data-ttu-id="73030-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="73030-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="73030-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="73030-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-130">Not supported</span></span> | <span data-ttu-id="73030-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-131">Not supported</span></span> | <span data-ttu-id="73030-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="73030-133">contact</span><span class="sxs-lookup"><span data-stu-id="73030-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="73030-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73030-134">Contacts.Read</span></span> | <span data-ttu-id="73030-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73030-135">Contacts.Read</span></span> | <span data-ttu-id="73030-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73030-136">Contacts.Read</span></span> |
|<span data-ttu-id="73030-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="73030-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="73030-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-138">Not supported</span></span> | <span data-ttu-id="73030-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73030-139">Files.ReadWrite</span></span> | <span data-ttu-id="73030-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-140">Not supported</span></span> |
|<span data-ttu-id="73030-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="73030-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="73030-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="73030-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-143">Not supported</span></span> | <span data-ttu-id="73030-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="73030-145">event</span><span class="sxs-lookup"><span data-stu-id="73030-145">event</span></span>](../resources/event.md) | <span data-ttu-id="73030-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73030-146">Calendars.Read</span></span> | <span data-ttu-id="73030-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73030-147">Calendars.Read</span></span> | <span data-ttu-id="73030-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73030-148">Calendars.Read</span></span> |
|[<span data-ttu-id="73030-149">group</span><span class="sxs-lookup"><span data-stu-id="73030-149">group</span></span>](../resources/group.md) | <span data-ttu-id="73030-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-150">Group.Read.All</span></span> | <span data-ttu-id="73030-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-151">Not supported</span></span> | <span data-ttu-id="73030-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-152">Group.Read.All</span></span> |
|[<span data-ttu-id="73030-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="73030-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="73030-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-154">Group.Read.All</span></span> | <span data-ttu-id="73030-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-155">Not supported</span></span> | <span data-ttu-id="73030-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-156">Not supported</span></span> |
|[<span data-ttu-id="73030-157">list</span><span class="sxs-lookup"><span data-stu-id="73030-157">list</span></span>](../resources/list.md) | <span data-ttu-id="73030-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="73030-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-159">Not supported</span></span> | <span data-ttu-id="73030-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="73030-161">message</span><span class="sxs-lookup"><span data-stu-id="73030-161">message</span></span>](../resources/message.md) | <span data-ttu-id="73030-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73030-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="73030-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73030-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="73030-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73030-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="73030-165">presence</span><span class="sxs-lookup"><span data-stu-id="73030-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="73030-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-166">Presence.Read.All</span></span> | <span data-ttu-id="73030-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-167">Not supported</span></span> | <span data-ttu-id="73030-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-168">Not supported</span></span> |
|[<span data-ttu-id="73030-169">printer</span><span class="sxs-lookup"><span data-stu-id="73030-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="73030-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-170">Not supported</span></span> | <span data-ttu-id="73030-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-171">Not supported</span></span> | <span data-ttu-id="73030-172">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="73030-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="73030-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="73030-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-174">Not supported</span></span> | <span data-ttu-id="73030-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-175">Not supported</span></span> | <span data-ttu-id="73030-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="73030-177">security alert</span><span class="sxs-lookup"><span data-stu-id="73030-177">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="73030-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="73030-179">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-179">Not supported</span></span> | <span data-ttu-id="73030-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73030-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="73030-181">todoTask</span><span class="sxs-lookup"><span data-stu-id="73030-181">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="73030-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73030-182">Tasks.ReadWrite</span></span> | <span data-ttu-id="73030-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73030-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="73030-184">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73030-184">Not supported</span></span> |
|[<span data-ttu-id="73030-185">user</span><span class="sxs-lookup"><span data-stu-id="73030-185">user</span></span>](../resources/user.md) | <span data-ttu-id="73030-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-186">User.Read.All</span></span> | <span data-ttu-id="73030-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-187">User.Read.All</span></span> | <span data-ttu-id="73030-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="73030-188">User.Read.All</span></span> |

> <span data-ttu-id="73030-189">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="73030-189">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="73030-190">driveItem</span><span class="sxs-lookup"><span data-stu-id="73030-190">driveItem</span></span>

<span data-ttu-id="73030-191">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="73030-191">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="73030-192">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="73030-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="73030-193">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="73030-193">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="73030-194">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="73030-194">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="73030-195">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="73030-195">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="73030-196">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="73030-196">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="73030-197">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="73030-197">contact, event, and message</span></span>

<span data-ttu-id="73030-198">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="73030-198">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="73030-199">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="73030-199">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="73030-200">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="73030-200">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="73030-201">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="73030-201">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="73030-202">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="73030-202">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="73030-203">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="73030-203">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="73030-204">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="73030-204">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="73030-205">presence</span><span class="sxs-lookup"><span data-stu-id="73030-205">presence</span></span>

<span data-ttu-id="73030-206">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="73030-206">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="73030-207">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="73030-207">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="73030-208">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73030-208">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="73030-209">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73030-209">Request headers</span></span>

| <span data-ttu-id="73030-210">Имя</span><span class="sxs-lookup"><span data-stu-id="73030-210">Name</span></span>       | <span data-ttu-id="73030-211">Тип</span><span class="sxs-lookup"><span data-stu-id="73030-211">Type</span></span> | <span data-ttu-id="73030-212">Описание</span><span class="sxs-lookup"><span data-stu-id="73030-212">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73030-213">Authorization</span><span class="sxs-lookup"><span data-stu-id="73030-213">Authorization</span></span>  | <span data-ttu-id="73030-214">string</span><span class="sxs-lookup"><span data-stu-id="73030-214">string</span></span>  | <span data-ttu-id="73030-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73030-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73030-217">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73030-217">Request body</span></span>

<span data-ttu-id="73030-218">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73030-218">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73030-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="73030-219">Response</span></span>

<span data-ttu-id="73030-220">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="73030-220">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="73030-221">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="73030-221">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="73030-222">Пример</span><span class="sxs-lookup"><span data-stu-id="73030-222">Example</span></span>

##### <a name="request"></a><span data-ttu-id="73030-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="73030-223">Request</span></span>

<span data-ttu-id="73030-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73030-224">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73030-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="73030-225">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="73030-226">C#</span><span class="sxs-lookup"><span data-stu-id="73030-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73030-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73030-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73030-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73030-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73030-229">Java</span><span class="sxs-lookup"><span data-stu-id="73030-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="73030-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="73030-230">Response</span></span>

<span data-ttu-id="73030-231">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73030-231">Here is an example of the response.</span></span>
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


