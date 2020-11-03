---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fbf44321322d51bc237715f7b4555a68655ee10
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848691"
---
# <a name="delete-subscription"></a><span data-ttu-id="10366-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="10366-103">Delete subscription</span></span>

<span data-ttu-id="10366-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10366-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10366-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="10366-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="10366-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10366-106">Permissions</span></span>

<span data-ttu-id="10366-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="10366-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="10366-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10366-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10366-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="10366-109">Supported resource</span></span> | <span data-ttu-id="10366-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10366-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10366-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10366-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10366-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="10366-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="10366-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="10366-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="10366-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-114">Not supported</span></span> | <span data-ttu-id="10366-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-115">Not supported</span></span> | <span data-ttu-id="10366-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="10366-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="10366-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="10366-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10366-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="10366-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-119">Not supported</span></span> | <span data-ttu-id="10366-120">Чаннелмессаже. Read. Group \*, Чаннелмессаже. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="10366-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="10366-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="10366-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="10366-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-122">Not supported</span></span> | <span data-ttu-id="10366-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-123">Not supported</span></span> | <span data-ttu-id="10366-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="10366-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="10366-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="10366-126">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10366-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="10366-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-127">Not supported</span></span> | <span data-ttu-id="10366-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="10366-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="10366-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="10366-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-130">Not supported</span></span> | <span data-ttu-id="10366-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-131">Not supported</span></span> | <span data-ttu-id="10366-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="10366-133">contact</span><span class="sxs-lookup"><span data-stu-id="10366-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="10366-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="10366-134">Contacts.Read</span></span> | <span data-ttu-id="10366-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="10366-135">Contacts.Read</span></span> | <span data-ttu-id="10366-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="10366-136">Contacts.Read</span></span> |
|<span data-ttu-id="10366-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="10366-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="10366-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-138">Not supported</span></span> | <span data-ttu-id="10366-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10366-139">Files.ReadWrite</span></span> | <span data-ttu-id="10366-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-140">Not supported</span></span> |
|<span data-ttu-id="10366-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="10366-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="10366-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10366-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="10366-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-143">Not supported</span></span> | <span data-ttu-id="10366-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10366-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="10366-145">event</span><span class="sxs-lookup"><span data-stu-id="10366-145">event</span></span>](../resources/event.md) | <span data-ttu-id="10366-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="10366-146">Calendars.Read</span></span> | <span data-ttu-id="10366-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="10366-147">Calendars.Read</span></span> | <span data-ttu-id="10366-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="10366-148">Calendars.Read</span></span> |
|[<span data-ttu-id="10366-149">group</span><span class="sxs-lookup"><span data-stu-id="10366-149">group</span></span>](../resources/group.md) | <span data-ttu-id="10366-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-150">Group.Read.All</span></span> | <span data-ttu-id="10366-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-151">Not supported</span></span> | <span data-ttu-id="10366-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-152">Group.Read.All</span></span> |
|[<span data-ttu-id="10366-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="10366-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="10366-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-154">Group.Read.All</span></span> | <span data-ttu-id="10366-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-155">Not supported</span></span> | <span data-ttu-id="10366-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-156">Not supported</span></span> |
|[<span data-ttu-id="10366-157">list</span><span class="sxs-lookup"><span data-stu-id="10366-157">list</span></span>](../resources/list.md) | <span data-ttu-id="10366-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10366-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="10366-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-159">Not supported</span></span> | <span data-ttu-id="10366-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10366-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="10366-161">message</span><span class="sxs-lookup"><span data-stu-id="10366-161">message</span></span>](../resources/message.md) | <span data-ttu-id="10366-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="10366-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="10366-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="10366-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="10366-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="10366-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="10366-165">presence</span><span class="sxs-lookup"><span data-stu-id="10366-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="10366-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-166">Presence.Read.All</span></span> | <span data-ttu-id="10366-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-167">Not supported</span></span> | <span data-ttu-id="10366-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-168">Not supported</span></span> |
|[<span data-ttu-id="10366-169">security alert</span><span class="sxs-lookup"><span data-stu-id="10366-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="10366-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10366-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="10366-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="10366-171">Not supported</span></span> | <span data-ttu-id="10366-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10366-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="10366-173">user</span><span class="sxs-lookup"><span data-stu-id="10366-173">user</span></span>](../resources/user.md) | <span data-ttu-id="10366-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-174">User.Read.All</span></span> | <span data-ttu-id="10366-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-175">User.Read.All</span></span> | <span data-ttu-id="10366-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="10366-176">User.Read.All</span></span> |

> <span data-ttu-id="10366-177">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="10366-177">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="10366-178">chatMessage</span><span class="sxs-lookup"><span data-stu-id="10366-178">chatMessage</span></span>

<span data-ttu-id="10366-179">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов ( **инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="10366-179">**chatMessage** subscriptions with delegated permissions do not support resource data ( **includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="10366-180">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="10366-180">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="10366-181">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="10366-181">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="10366-182">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="10366-182">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="10366-183">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="10366-183">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="10366-184">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="10366-184">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="10366-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="10366-185">driveItem</span></span>

<span data-ttu-id="10366-186">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="10366-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="10366-187">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="10366-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="10366-188">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="10366-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="10366-189">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="10366-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="10366-190">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="10366-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="10366-191">Нельзя подписаться на экземпляры **drive** или **driveItem** , не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="10366-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="10366-192">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="10366-192">contact, event, and message</span></span>

<span data-ttu-id="10366-193">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="10366-193">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="10366-194">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="10366-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="10366-195">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="10366-195">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="10366-196">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="10366-196">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="10366-197">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="10366-197">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="10366-198">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="10366-198">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="10366-199">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="10366-199">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="10366-200">presence</span><span class="sxs-lookup"><span data-stu-id="10366-200">presence</span></span>

<span data-ttu-id="10366-201">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="10366-201">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="10366-202">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="10366-202">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="10366-203">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10366-203">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="10366-204">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10366-204">Request headers</span></span>

| <span data-ttu-id="10366-205">Имя</span><span class="sxs-lookup"><span data-stu-id="10366-205">Name</span></span>       | <span data-ttu-id="10366-206">Тип</span><span class="sxs-lookup"><span data-stu-id="10366-206">Type</span></span> | <span data-ttu-id="10366-207">Описание</span><span class="sxs-lookup"><span data-stu-id="10366-207">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10366-208">Authorization</span><span class="sxs-lookup"><span data-stu-id="10366-208">Authorization</span></span>  | <span data-ttu-id="10366-209">string</span><span class="sxs-lookup"><span data-stu-id="10366-209">string</span></span>  | <span data-ttu-id="10366-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10366-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10366-212">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10366-212">Request body</span></span>

<span data-ttu-id="10366-213">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10366-213">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10366-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="10366-214">Response</span></span>

<span data-ttu-id="10366-215">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="10366-215">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="10366-216">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="10366-216">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="10366-217">Пример</span><span class="sxs-lookup"><span data-stu-id="10366-217">Example</span></span>

##### <a name="request"></a><span data-ttu-id="10366-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="10366-218">Request</span></span>

<span data-ttu-id="10366-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10366-219">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10366-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="10366-220">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="10366-221">C#</span><span class="sxs-lookup"><span data-stu-id="10366-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10366-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10366-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10366-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10366-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="10366-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="10366-224">Response</span></span>

<span data-ttu-id="10366-225">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10366-225">Here is an example of the response.</span></span>
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


