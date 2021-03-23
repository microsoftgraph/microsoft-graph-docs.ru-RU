---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 00c4f95eb53ec565084e309b49173887b0428f39
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51031130"
---
# <a name="delete-subscription"></a><span data-ttu-id="225cc-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="225cc-103">Delete subscription</span></span>

<span data-ttu-id="225cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="225cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="225cc-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="225cc-105">Delete a subscription.</span></span>

<span data-ttu-id="225cc-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="225cc-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="225cc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="225cc-107">Permissions</span></span>

<span data-ttu-id="225cc-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="225cc-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="225cc-109">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="225cc-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="225cc-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="225cc-110">Supported resource</span></span> | <span data-ttu-id="225cc-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="225cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="225cc-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="225cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="225cc-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="225cc-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="225cc-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="225cc-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="225cc-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-115">Not supported</span></span> | <span data-ttu-id="225cc-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-116">Not supported</span></span> | <span data-ttu-id="225cc-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-117">CallRecords.Read.All</span></span> |
|<span data-ttu-id="225cc-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="225cc-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="225cc-119">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-119">ChannelMessage.Read.All</span></span> | <span data-ttu-id="225cc-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-120">Not supported</span></span> |  <span data-ttu-id="225cc-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="225cc-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="225cc-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="225cc-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-123">Not supported</span></span> | <span data-ttu-id="225cc-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-124">Not supported</span></span> | <span data-ttu-id="225cc-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="225cc-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="225cc-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="225cc-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-127">Not supported</span></span> | <span data-ttu-id="225cc-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-128">Not supported</span></span> | <span data-ttu-id="225cc-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="225cc-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="225cc-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="225cc-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-131">Not supported</span></span> | <span data-ttu-id="225cc-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-132">Not supported</span></span> | <span data-ttu-id="225cc-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="225cc-134">contact</span><span class="sxs-lookup"><span data-stu-id="225cc-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="225cc-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-135">Contacts.Read</span></span> | <span data-ttu-id="225cc-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-136">Contacts.Read</span></span> | <span data-ttu-id="225cc-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-137">Contacts.Read</span></span> |
|<span data-ttu-id="225cc-138">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="225cc-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="225cc-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-139">Not supported</span></span> | <span data-ttu-id="225cc-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="225cc-140">Files.ReadWrite</span></span> | <span data-ttu-id="225cc-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-141">Not supported</span></span> |
|<span data-ttu-id="225cc-142">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="225cc-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="225cc-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225cc-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="225cc-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-144">Not supported</span></span> | <span data-ttu-id="225cc-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225cc-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="225cc-146">event</span><span class="sxs-lookup"><span data-stu-id="225cc-146">event</span></span>](../resources/event.md) | <span data-ttu-id="225cc-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-147">Calendars.Read</span></span> | <span data-ttu-id="225cc-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-148">Calendars.Read</span></span> | <span data-ttu-id="225cc-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-149">Calendars.Read</span></span> |
|[<span data-ttu-id="225cc-150">group</span><span class="sxs-lookup"><span data-stu-id="225cc-150">group</span></span>](../resources/group.md) | <span data-ttu-id="225cc-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-151">Group.Read.All</span></span> | <span data-ttu-id="225cc-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-152">Not supported</span></span> | <span data-ttu-id="225cc-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-153">Group.Read.All</span></span> |
|[<span data-ttu-id="225cc-154">group conversation</span><span class="sxs-lookup"><span data-stu-id="225cc-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="225cc-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-155">Group.Read.All</span></span> | <span data-ttu-id="225cc-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-156">Not supported</span></span> | <span data-ttu-id="225cc-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-157">Not supported</span></span> |
|[<span data-ttu-id="225cc-158">list</span><span class="sxs-lookup"><span data-stu-id="225cc-158">list</span></span>](../resources/list.md) | <span data-ttu-id="225cc-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225cc-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="225cc-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-160">Not supported</span></span> | <span data-ttu-id="225cc-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225cc-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="225cc-162">message</span><span class="sxs-lookup"><span data-stu-id="225cc-162">message</span></span>](../resources/message.md) | <span data-ttu-id="225cc-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="225cc-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="225cc-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="225cc-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="225cc-166">printer</span><span class="sxs-lookup"><span data-stu-id="225cc-166">printer</span></span>](../resources/printer.md) | <span data-ttu-id="225cc-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-167">Not supported</span></span> | <span data-ttu-id="225cc-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-168">Not supported</span></span> | <span data-ttu-id="225cc-169">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225cc-169">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="225cc-170">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="225cc-170">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="225cc-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-171">Not supported</span></span> | <span data-ttu-id="225cc-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-172">Not supported</span></span> | <span data-ttu-id="225cc-173">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225cc-173">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="225cc-174">security alert</span><span class="sxs-lookup"><span data-stu-id="225cc-174">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="225cc-175">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225cc-175">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="225cc-176">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="225cc-176">Not supported</span></span> | <span data-ttu-id="225cc-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225cc-177">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="225cc-178">user</span><span class="sxs-lookup"><span data-stu-id="225cc-178">user</span></span>](../resources/user.md) | <span data-ttu-id="225cc-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-179">User.Read.All</span></span> | <span data-ttu-id="225cc-180">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-180">User.Read.All</span></span> | <span data-ttu-id="225cc-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="225cc-181">User.Read.All</span></span> |


> <span data-ttu-id="225cc-182">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="225cc-182">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="225cc-183">driveItem</span><span class="sxs-lookup"><span data-stu-id="225cc-183">driveItem</span></span>

<span data-ttu-id="225cc-184">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="225cc-184">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="225cc-185">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="225cc-185">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="225cc-186">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="225cc-186">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="225cc-187">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="225cc-187">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="225cc-188">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="225cc-188">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="225cc-189">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="225cc-189">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="225cc-190">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="225cc-190">contact, event, and message</span></span>

<span data-ttu-id="225cc-191">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="225cc-191">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="225cc-192">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="225cc-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="225cc-193">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="225cc-193">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="225cc-194">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="225cc-194">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="225cc-195">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="225cc-195">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="225cc-196">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="225cc-196">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="225cc-197">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="225cc-197">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="225cc-198">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="225cc-198">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="225cc-199">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="225cc-199">Request headers</span></span>

| <span data-ttu-id="225cc-200">Имя</span><span class="sxs-lookup"><span data-stu-id="225cc-200">Name</span></span>       | <span data-ttu-id="225cc-201">Тип</span><span class="sxs-lookup"><span data-stu-id="225cc-201">Type</span></span> | <span data-ttu-id="225cc-202">Описание</span><span class="sxs-lookup"><span data-stu-id="225cc-202">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="225cc-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="225cc-203">Authorization</span></span>  | <span data-ttu-id="225cc-204">string</span><span class="sxs-lookup"><span data-stu-id="225cc-204">string</span></span>  | <span data-ttu-id="225cc-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="225cc-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="225cc-207">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="225cc-207">Request body</span></span>

<span data-ttu-id="225cc-208">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="225cc-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="225cc-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="225cc-209">Response</span></span>

<span data-ttu-id="225cc-210">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="225cc-210">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="225cc-211">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="225cc-211">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="225cc-212">Пример</span><span class="sxs-lookup"><span data-stu-id="225cc-212">Example</span></span>

##### <a name="request"></a><span data-ttu-id="225cc-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="225cc-213">Request</span></span>

<span data-ttu-id="225cc-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="225cc-214">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="225cc-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="225cc-215">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="225cc-216">C#</span><span class="sxs-lookup"><span data-stu-id="225cc-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="225cc-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="225cc-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="225cc-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="225cc-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="225cc-219">Java</span><span class="sxs-lookup"><span data-stu-id="225cc-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="225cc-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="225cc-220">Response</span></span>

<span data-ttu-id="225cc-221">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="225cc-221">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
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

