---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
ms.prod: change-notifications
doc_type: apiPageType
ms.openlocfilehash: fdd46e0b68ae1d7b2afab17cd6ded1c81c1fb7d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963678"
---
# <a name="delete-subscription"></a><span data-ttu-id="27c98-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="27c98-103">Delete subscription</span></span>

<span data-ttu-id="27c98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27c98-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27c98-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="27c98-105">Delete a subscription.</span></span>

<span data-ttu-id="27c98-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="27c98-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="27c98-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27c98-107">Permissions</span></span>

<span data-ttu-id="27c98-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="27c98-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="27c98-109">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27c98-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27c98-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="27c98-110">Supported resource</span></span> | <span data-ttu-id="27c98-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27c98-111">Delegated (work or school account)</span></span> | <span data-ttu-id="27c98-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27c98-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27c98-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="27c98-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="27c98-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="27c98-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="27c98-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-115">Not supported</span></span> | <span data-ttu-id="27c98-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-116">Not supported</span></span> | <span data-ttu-id="27c98-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-117">CallRecords.Read.All</span></span> |
|<span data-ttu-id="27c98-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="27c98-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="27c98-119">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-119">ChannelMessage.Read.All</span></span> | <span data-ttu-id="27c98-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-120">Not supported</span></span> |  <span data-ttu-id="27c98-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="27c98-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="27c98-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="27c98-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-123">Not supported</span></span> | <span data-ttu-id="27c98-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-124">Not supported</span></span> | <span data-ttu-id="27c98-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="27c98-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="27c98-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="27c98-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-127">Not supported</span></span> | <span data-ttu-id="27c98-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-128">Not supported</span></span> | <span data-ttu-id="27c98-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="27c98-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="27c98-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="27c98-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-131">Not supported</span></span> | <span data-ttu-id="27c98-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-132">Not supported</span></span> | <span data-ttu-id="27c98-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="27c98-134">contact</span><span class="sxs-lookup"><span data-stu-id="27c98-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="27c98-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-135">Contacts.Read</span></span> | <span data-ttu-id="27c98-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-136">Contacts.Read</span></span> | <span data-ttu-id="27c98-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-137">Contacts.Read</span></span> |
|<span data-ttu-id="27c98-138">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="27c98-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="27c98-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-139">Not supported</span></span> | <span data-ttu-id="27c98-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27c98-140">Files.ReadWrite</span></span> | <span data-ttu-id="27c98-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-141">Not supported</span></span> |
|<span data-ttu-id="27c98-142">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="27c98-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="27c98-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c98-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="27c98-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-144">Not supported</span></span> | <span data-ttu-id="27c98-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c98-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="27c98-146">event</span><span class="sxs-lookup"><span data-stu-id="27c98-146">event</span></span>](../resources/event.md) | <span data-ttu-id="27c98-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-147">Calendars.Read</span></span> | <span data-ttu-id="27c98-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-148">Calendars.Read</span></span> | <span data-ttu-id="27c98-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-149">Calendars.Read</span></span> |
|[<span data-ttu-id="27c98-150">group</span><span class="sxs-lookup"><span data-stu-id="27c98-150">group</span></span>](../resources/group.md) | <span data-ttu-id="27c98-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-151">Group.Read.All</span></span> | <span data-ttu-id="27c98-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-152">Not supported</span></span> | <span data-ttu-id="27c98-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-153">Group.Read.All</span></span> |
|[<span data-ttu-id="27c98-154">group conversation</span><span class="sxs-lookup"><span data-stu-id="27c98-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="27c98-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-155">Group.Read.All</span></span> | <span data-ttu-id="27c98-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-156">Not supported</span></span> | <span data-ttu-id="27c98-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-157">Not supported</span></span> |
|[<span data-ttu-id="27c98-158">list</span><span class="sxs-lookup"><span data-stu-id="27c98-158">list</span></span>](../resources/list.md) | <span data-ttu-id="27c98-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c98-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="27c98-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-160">Not supported</span></span> | <span data-ttu-id="27c98-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c98-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="27c98-162">message</span><span class="sxs-lookup"><span data-stu-id="27c98-162">message</span></span>](../resources/message.md) | <span data-ttu-id="27c98-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="27c98-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="27c98-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="27c98-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="27c98-166">security alert</span><span class="sxs-lookup"><span data-stu-id="27c98-166">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="27c98-167">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c98-167">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="27c98-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="27c98-168">Not supported</span></span> | <span data-ttu-id="27c98-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c98-169">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="27c98-170">user</span><span class="sxs-lookup"><span data-stu-id="27c98-170">user</span></span>](../resources/user.md) | <span data-ttu-id="27c98-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-171">User.Read.All</span></span> | <span data-ttu-id="27c98-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-172">User.Read.All</span></span> | <span data-ttu-id="27c98-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="27c98-173">User.Read.All</span></span> |

> <span data-ttu-id="27c98-174">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="27c98-174">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="27c98-175">driveItem</span><span class="sxs-lookup"><span data-stu-id="27c98-175">driveItem</span></span>

<span data-ttu-id="27c98-176">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="27c98-176">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="27c98-177">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="27c98-177">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="27c98-178">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="27c98-178">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="27c98-179">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="27c98-179">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="27c98-180">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="27c98-180">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="27c98-181">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="27c98-181">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="27c98-182">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="27c98-182">contact, event, and message</span></span>

<span data-ttu-id="27c98-183">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="27c98-183">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="27c98-184">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="27c98-184">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="27c98-185">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="27c98-185">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="27c98-186">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="27c98-186">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="27c98-187">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="27c98-187">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="27c98-188">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="27c98-188">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="27c98-189">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="27c98-189">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="27c98-190">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27c98-190">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="27c98-191">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27c98-191">Request headers</span></span>

| <span data-ttu-id="27c98-192">Имя</span><span class="sxs-lookup"><span data-stu-id="27c98-192">Name</span></span>       | <span data-ttu-id="27c98-193">Тип</span><span class="sxs-lookup"><span data-stu-id="27c98-193">Type</span></span> | <span data-ttu-id="27c98-194">Описание</span><span class="sxs-lookup"><span data-stu-id="27c98-194">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="27c98-195">Authorization</span><span class="sxs-lookup"><span data-stu-id="27c98-195">Authorization</span></span>  | <span data-ttu-id="27c98-196">string</span><span class="sxs-lookup"><span data-stu-id="27c98-196">string</span></span>  | <span data-ttu-id="27c98-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27c98-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27c98-199">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27c98-199">Request body</span></span>

<span data-ttu-id="27c98-200">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27c98-200">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27c98-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="27c98-201">Response</span></span>

<span data-ttu-id="27c98-202">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="27c98-202">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="27c98-203">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="27c98-203">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="27c98-204">Пример</span><span class="sxs-lookup"><span data-stu-id="27c98-204">Example</span></span>

##### <a name="request"></a><span data-ttu-id="27c98-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="27c98-205">Request</span></span>

<span data-ttu-id="27c98-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27c98-206">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27c98-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="27c98-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="27c98-208">C#</span><span class="sxs-lookup"><span data-stu-id="27c98-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27c98-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27c98-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27c98-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27c98-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27c98-211">Java</span><span class="sxs-lookup"><span data-stu-id="27c98-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="27c98-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="27c98-212">Response</span></span>

<span data-ttu-id="27c98-213">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27c98-213">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

