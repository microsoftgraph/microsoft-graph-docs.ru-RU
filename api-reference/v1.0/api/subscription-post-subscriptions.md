---
title: Создание подписки
description: Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменении данных в Microsoft Graph.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fb6f04b020fd925d1131f2d8f88afe44b185c5c7
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761432"
---
# <a name="create-subscription"></a><span data-ttu-id="c08c8-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="c08c8-103">Create subscription</span></span>

<span data-ttu-id="c08c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c08c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c08c8-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c08c8-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="c08c8-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="c08c8-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="c08c8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c08c8-107">Permissions</span></span>

<span data-ttu-id="c08c8-108">Создание подписки требует наличия области чтения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="c08c8-108">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="c08c8-109">Например, чтобы получать уведомления об изменениях в сообщениях, приложению необходимо разрешение `Mail.Read`.</span><span class="sxs-lookup"><span data-stu-id="c08c8-109">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
<span data-ttu-id="c08c8-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c08c8-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c08c8-111">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c08c8-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c08c8-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="c08c8-112">Supported resource</span></span> | <span data-ttu-id="c08c8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c08c8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c08c8-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c08c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c08c8-115">Application</span><span class="sxs-lookup"><span data-stu-id="c08c8-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="c08c8-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="c08c8-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="c08c8-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-117">Not supported</span></span> | <span data-ttu-id="c08c8-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-118">Not supported</span></span> | <span data-ttu-id="c08c8-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="c08c8-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="c08c8-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="c08c8-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-121">ChannelMessage.Read.All</span></span> | <span data-ttu-id="c08c8-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-122">Not supported</span></span> |  <span data-ttu-id="c08c8-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c08c8-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="c08c8-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="c08c8-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-125">Not supported</span></span> | <span data-ttu-id="c08c8-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-126">Not supported</span></span> | <span data-ttu-id="c08c8-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c08c8-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="c08c8-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="c08c8-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-129">Not supported</span></span> | <span data-ttu-id="c08c8-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-130">Not supported</span></span> | <span data-ttu-id="c08c8-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="c08c8-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="c08c8-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="c08c8-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-133">Not supported</span></span> | <span data-ttu-id="c08c8-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-134">Not supported</span></span> | <span data-ttu-id="c08c8-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="c08c8-136">contact</span><span class="sxs-lookup"><span data-stu-id="c08c8-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c08c8-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-137">Contacts.Read</span></span> | <span data-ttu-id="c08c8-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-138">Contacts.Read</span></span> | <span data-ttu-id="c08c8-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-139">Contacts.Read</span></span> |
|<span data-ttu-id="c08c8-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="c08c8-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="c08c8-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-141">Not supported</span></span> | <span data-ttu-id="c08c8-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c08c8-142">Files.ReadWrite</span></span> | <span data-ttu-id="c08c8-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-143">Not supported</span></span> |
|<span data-ttu-id="c08c8-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="c08c8-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="c08c8-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="c08c8-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-146">Not supported</span></span> | <span data-ttu-id="c08c8-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="c08c8-148">event</span><span class="sxs-lookup"><span data-stu-id="c08c8-148">event</span></span>](../resources/event.md) | <span data-ttu-id="c08c8-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-149">Calendars.Read</span></span> | <span data-ttu-id="c08c8-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-150">Calendars.Read</span></span> | <span data-ttu-id="c08c8-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-151">Calendars.Read</span></span> |
|[<span data-ttu-id="c08c8-152">group</span><span class="sxs-lookup"><span data-stu-id="c08c8-152">group</span></span>](../resources/group.md) | <span data-ttu-id="c08c8-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-153">Group.Read.All</span></span> | <span data-ttu-id="c08c8-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-154">Not supported</span></span> | <span data-ttu-id="c08c8-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-155">Group.Read.All</span></span> |
|[<span data-ttu-id="c08c8-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="c08c8-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="c08c8-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-157">Group.Read.All</span></span> | <span data-ttu-id="c08c8-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-158">Not supported</span></span> | <span data-ttu-id="c08c8-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-159">Not supported</span></span> |
|[<span data-ttu-id="c08c8-160">list</span><span class="sxs-lookup"><span data-stu-id="c08c8-160">list</span></span>](../resources/list.md) | <span data-ttu-id="c08c8-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="c08c8-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-162">Not supported</span></span> | <span data-ttu-id="c08c8-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="c08c8-164">message</span><span class="sxs-lookup"><span data-stu-id="c08c8-164">message</span></span>](../resources/message.md) | <span data-ttu-id="c08c8-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c08c8-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c08c8-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c08c8-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="c08c8-168">security alert</span><span class="sxs-lookup"><span data-stu-id="c08c8-168">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="c08c8-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-169">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="c08c8-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c08c8-170">Not supported</span></span> | <span data-ttu-id="c08c8-171">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-171">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="c08c8-172">user</span><span class="sxs-lookup"><span data-stu-id="c08c8-172">user</span></span>](../resources/user.md) | <span data-ttu-id="c08c8-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-173">User.Read.All</span></span> | <span data-ttu-id="c08c8-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-174">User.Read.All</span></span> | <span data-ttu-id="c08c8-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08c8-175">User.Read.All</span></span> |

> <span data-ttu-id="c08c8-176">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="c08c8-176">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="c08c8-177">driveItem</span><span class="sxs-lookup"><span data-stu-id="c08c8-177">driveItem</span></span>

<span data-ttu-id="c08c8-178">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c08c8-178">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="c08c8-179">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="c08c8-179">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="c08c8-180">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="c08c8-180">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="c08c8-181">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="c08c8-181">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="c08c8-182">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="c08c8-182">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="c08c8-183">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="c08c8-183">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="c08c8-184">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="c08c8-184">contact, event, and message</span></span>

<span data-ttu-id="c08c8-185">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="c08c8-185">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="c08c8-186">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="c08c8-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="c08c8-187">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="c08c8-187">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="c08c8-188">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c08c8-188">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="c08c8-189">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="c08c8-189">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="c08c8-190">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c08c8-190">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="c08c8-191">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="c08c8-191">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="c08c8-192">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c08c8-192">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="c08c8-193">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c08c8-193">Request headers</span></span>

| <span data-ttu-id="c08c8-194">Имя</span><span class="sxs-lookup"><span data-stu-id="c08c8-194">Name</span></span>       | <span data-ttu-id="c08c8-195">Тип</span><span class="sxs-lookup"><span data-stu-id="c08c8-195">Type</span></span> | <span data-ttu-id="c08c8-196">Описание</span><span class="sxs-lookup"><span data-stu-id="c08c8-196">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c08c8-197">Authorization</span><span class="sxs-lookup"><span data-stu-id="c08c8-197">Authorization</span></span>  | <span data-ttu-id="c08c8-198">string</span><span class="sxs-lookup"><span data-stu-id="c08c8-198">string</span></span>  | <span data-ttu-id="c08c8-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c08c8-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c08c8-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="c08c8-201">Response</span></span>

<span data-ttu-id="c08c8-202">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c08c8-202">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="c08c8-203">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="c08c8-203">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="c08c8-204">Пример</span><span class="sxs-lookup"><span data-stu-id="c08c8-204">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c08c8-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="c08c8-205">Request</span></span>

<span data-ttu-id="c08c8-206">Ниже представлен пример запроса на отправку уведомления об изменениях при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="c08c8-206">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="c08c8-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="c08c8-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="c08c8-208">C#</span><span class="sxs-lookup"><span data-stu-id="c08c8-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c08c8-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c08c8-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c08c8-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c08c8-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c08c8-211">Java</span><span class="sxs-lookup"><span data-stu-id="c08c8-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c08c8-212">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c08c8-212">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="c08c8-213">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="c08c8-213">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="c08c8-214">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="c08c8-214">Resources examples</span></span>

<span data-ttu-id="c08c8-215">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="c08c8-215">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="c08c8-216">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="c08c8-216">Resource type</span></span> | <span data-ttu-id="c08c8-217">Примеры</span><span class="sxs-lookup"><span data-stu-id="c08c8-217">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="c08c8-218">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="c08c8-218">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="c08c8-219">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="c08c8-219">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c08c8-220">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="c08c8-220">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="c08c8-221">Контакты</span><span class="sxs-lookup"><span data-stu-id="c08c8-221">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="c08c8-222">Беседы</span><span class="sxs-lookup"><span data-stu-id="c08c8-222">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="c08c8-223">Диски</span><span class="sxs-lookup"><span data-stu-id="c08c8-223">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="c08c8-224">События</span><span class="sxs-lookup"><span data-stu-id="c08c8-224">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="c08c8-225">Группы</span><span class="sxs-lookup"><span data-stu-id="c08c8-225">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="c08c8-226">Список</span><span class="sxs-lookup"><span data-stu-id="c08c8-226">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="c08c8-227">Почта</span><span class="sxs-lookup"><span data-stu-id="c08c8-227">Mail</span></span>](../resources/message.md)|<span data-ttu-id="c08c8-228">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="c08c8-228">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="c08c8-229">Пользователи</span><span class="sxs-lookup"><span data-stu-id="c08c8-229">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="c08c8-230">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="c08c8-230">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> <span data-ttu-id="c08c8-231">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="c08c8-231">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="c08c8-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="c08c8-232">Response</span></span>

<span data-ttu-id="c08c8-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c08c8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="c08c8-236">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="c08c8-236">Notification endpoint validation</span></span>

<span data-ttu-id="c08c8-237">Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="c08c8-237">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="c08c8-238">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="c08c8-238">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

