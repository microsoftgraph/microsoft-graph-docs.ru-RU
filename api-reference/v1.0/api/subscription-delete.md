---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b4b05d659453ef0867d60f3d43d137f4b697874
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034077"
---
# <a name="delete-subscription"></a><span data-ttu-id="ef159-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="ef159-103">Delete subscription</span></span>

<span data-ttu-id="ef159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef159-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef159-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="ef159-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef159-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef159-106">Permissions</span></span>

<span data-ttu-id="ef159-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ef159-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="ef159-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef159-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef159-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="ef159-109">Supported resource</span></span> | <span data-ttu-id="ef159-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef159-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef159-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef159-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef159-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="ef159-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="ef159-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="ef159-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="ef159-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-114">Not supported</span></span> | <span data-ttu-id="ef159-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-115">Not supported</span></span> | <span data-ttu-id="ef159-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="ef159-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="ef159-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="ef159-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-118">Not supported</span></span> | <span data-ttu-id="ef159-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-119">Not supported</span></span> |  <span data-ttu-id="ef159-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="ef159-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="ef159-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="ef159-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-122">Not supported</span></span> | <span data-ttu-id="ef159-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-123">Not supported</span></span> | <span data-ttu-id="ef159-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="ef159-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="ef159-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="ef159-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-126">Not supported</span></span> | <span data-ttu-id="ef159-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-127">Not supported</span></span> | <span data-ttu-id="ef159-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="ef159-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="ef159-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="ef159-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-130">Not supported</span></span> | <span data-ttu-id="ef159-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-131">Not supported</span></span> | <span data-ttu-id="ef159-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="ef159-133">contact</span><span class="sxs-lookup"><span data-stu-id="ef159-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="ef159-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-134">Contacts.Read</span></span> | <span data-ttu-id="ef159-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-135">Contacts.Read</span></span> | <span data-ttu-id="ef159-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-136">Contacts.Read</span></span> |
|<span data-ttu-id="ef159-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="ef159-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="ef159-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-138">Not supported</span></span> | <span data-ttu-id="ef159-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef159-139">Files.ReadWrite</span></span> | <span data-ttu-id="ef159-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-140">Not supported</span></span> |
|<span data-ttu-id="ef159-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="ef159-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="ef159-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef159-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="ef159-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-143">Not supported</span></span> | <span data-ttu-id="ef159-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef159-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="ef159-145">event</span><span class="sxs-lookup"><span data-stu-id="ef159-145">event</span></span>](../resources/event.md) | <span data-ttu-id="ef159-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-146">Calendars.Read</span></span> | <span data-ttu-id="ef159-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-147">Calendars.Read</span></span> | <span data-ttu-id="ef159-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-148">Calendars.Read</span></span> |
|[<span data-ttu-id="ef159-149">group</span><span class="sxs-lookup"><span data-stu-id="ef159-149">group</span></span>](../resources/group.md) | <span data-ttu-id="ef159-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-150">Group.Read.All</span></span> | <span data-ttu-id="ef159-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-151">Not supported</span></span> | <span data-ttu-id="ef159-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-152">Group.Read.All</span></span> |
|[<span data-ttu-id="ef159-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="ef159-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="ef159-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-154">Group.Read.All</span></span> | <span data-ttu-id="ef159-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-155">Not supported</span></span> | <span data-ttu-id="ef159-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-156">Not supported</span></span> |
|[<span data-ttu-id="ef159-157">list</span><span class="sxs-lookup"><span data-stu-id="ef159-157">list</span></span>](../resources/list.md) | <span data-ttu-id="ef159-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef159-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="ef159-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-159">Not supported</span></span> | <span data-ttu-id="ef159-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef159-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="ef159-161">message</span><span class="sxs-lookup"><span data-stu-id="ef159-161">message</span></span>](../resources/message.md) | <span data-ttu-id="ef159-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ef159-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ef159-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ef159-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="ef159-165">security alert</span><span class="sxs-lookup"><span data-stu-id="ef159-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="ef159-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef159-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="ef159-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef159-167">Not supported</span></span> | <span data-ttu-id="ef159-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef159-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="ef159-169">user</span><span class="sxs-lookup"><span data-stu-id="ef159-169">user</span></span>](../resources/user.md) | <span data-ttu-id="ef159-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-170">User.Read.All</span></span> | <span data-ttu-id="ef159-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-171">User.Read.All</span></span> | <span data-ttu-id="ef159-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef159-172">User.Read.All</span></span> |

> <span data-ttu-id="ef159-173">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ef159-173">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="ef159-174">driveItem</span><span class="sxs-lookup"><span data-stu-id="ef159-174">driveItem</span></span>

<span data-ttu-id="ef159-175">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ef159-175">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="ef159-176">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="ef159-176">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="ef159-177">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="ef159-177">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="ef159-178">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="ef159-178">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="ef159-179">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="ef159-179">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="ef159-180">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="ef159-180">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="ef159-181">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="ef159-181">contact, event, and message</span></span>

<span data-ttu-id="ef159-182">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="ef159-182">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="ef159-183">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="ef159-183">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="ef159-184">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="ef159-184">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="ef159-185">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef159-185">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="ef159-186">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="ef159-186">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="ef159-187">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ef159-187">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="ef159-188">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="ef159-188">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="ef159-189">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef159-189">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="ef159-190">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef159-190">Request headers</span></span>

| <span data-ttu-id="ef159-191">Имя</span><span class="sxs-lookup"><span data-stu-id="ef159-191">Name</span></span>       | <span data-ttu-id="ef159-192">Тип</span><span class="sxs-lookup"><span data-stu-id="ef159-192">Type</span></span> | <span data-ttu-id="ef159-193">Описание</span><span class="sxs-lookup"><span data-stu-id="ef159-193">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ef159-194">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef159-194">Authorization</span></span>  | <span data-ttu-id="ef159-195">string</span><span class="sxs-lookup"><span data-stu-id="ef159-195">string</span></span>  | <span data-ttu-id="ef159-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef159-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef159-198">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef159-198">Request body</span></span>

<span data-ttu-id="ef159-199">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef159-199">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef159-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef159-200">Response</span></span>

<span data-ttu-id="ef159-201">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef159-201">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="ef159-202">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="ef159-202">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="ef159-203">Пример</span><span class="sxs-lookup"><span data-stu-id="ef159-203">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ef159-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef159-204">Request</span></span>

<span data-ttu-id="ef159-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef159-205">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef159-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef159-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="ef159-207">C#</span><span class="sxs-lookup"><span data-stu-id="ef159-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef159-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef159-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef159-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef159-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef159-210">Java</span><span class="sxs-lookup"><span data-stu-id="ef159-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ef159-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef159-211">Response</span></span>

<span data-ttu-id="ef159-212">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef159-212">Here is an example of the response.</span></span>
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

