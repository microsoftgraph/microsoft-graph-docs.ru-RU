---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c318ba13b21767311d2cecc5b421cea21a81b2c0
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092603"
---
# <a name="get-subscription"></a><span data-ttu-id="daa71-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="daa71-103">Get subscription</span></span>

<span data-ttu-id="daa71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daa71-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="daa71-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="daa71-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="daa71-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="daa71-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="daa71-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="daa71-107">Permissions</span></span>

<span data-ttu-id="daa71-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="daa71-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="daa71-109">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daa71-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="daa71-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="daa71-110">Supported resource</span></span> | <span data-ttu-id="daa71-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daa71-111">Delegated (work or school account)</span></span> | <span data-ttu-id="daa71-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daa71-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daa71-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="daa71-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="daa71-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="daa71-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="daa71-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-115">Not supported</span></span> | <span data-ttu-id="daa71-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-116">Not supported</span></span> | <span data-ttu-id="daa71-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-117">CallRecords.Read.All</span></span> |
|<span data-ttu-id="daa71-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="daa71-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="daa71-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-119">Not supported</span></span> | <span data-ttu-id="daa71-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-120">Not supported</span></span> |  <span data-ttu-id="daa71-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="daa71-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="daa71-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="daa71-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-123">Not supported</span></span> | <span data-ttu-id="daa71-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-124">Not supported</span></span> | <span data-ttu-id="daa71-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="daa71-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="daa71-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="daa71-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-127">Not supported</span></span> | <span data-ttu-id="daa71-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-128">Not supported</span></span> | <span data-ttu-id="daa71-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="daa71-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="daa71-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="daa71-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-131">Not supported</span></span> | <span data-ttu-id="daa71-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-132">Not supported</span></span> | <span data-ttu-id="daa71-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="daa71-134">contact</span><span class="sxs-lookup"><span data-stu-id="daa71-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="daa71-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-135">Contacts.Read</span></span> | <span data-ttu-id="daa71-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-136">Contacts.Read</span></span> | <span data-ttu-id="daa71-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-137">Contacts.Read</span></span> |
|<span data-ttu-id="daa71-138">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="daa71-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="daa71-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-139">Not supported</span></span> | <span data-ttu-id="daa71-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="daa71-140">Files.ReadWrite</span></span> | <span data-ttu-id="daa71-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-141">Not supported</span></span> |
|<span data-ttu-id="daa71-142">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="daa71-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="daa71-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daa71-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="daa71-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-144">Not supported</span></span> | <span data-ttu-id="daa71-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daa71-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="daa71-146">event</span><span class="sxs-lookup"><span data-stu-id="daa71-146">event</span></span>](../resources/event.md) | <span data-ttu-id="daa71-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-147">Calendars.Read</span></span> | <span data-ttu-id="daa71-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-148">Calendars.Read</span></span> | <span data-ttu-id="daa71-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-149">Calendars.Read</span></span> |
|[<span data-ttu-id="daa71-150">group</span><span class="sxs-lookup"><span data-stu-id="daa71-150">group</span></span>](../resources/group.md) | <span data-ttu-id="daa71-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-151">Group.Read.All</span></span> | <span data-ttu-id="daa71-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-152">Not supported</span></span> | <span data-ttu-id="daa71-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-153">Group.Read.All</span></span> |
|[<span data-ttu-id="daa71-154">group conversation</span><span class="sxs-lookup"><span data-stu-id="daa71-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="daa71-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-155">Group.Read.All</span></span> | <span data-ttu-id="daa71-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-156">Not supported</span></span> | <span data-ttu-id="daa71-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-157">Not supported</span></span> |
|[<span data-ttu-id="daa71-158">list</span><span class="sxs-lookup"><span data-stu-id="daa71-158">list</span></span>](../resources/list.md) | <span data-ttu-id="daa71-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daa71-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="daa71-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-160">Not supported</span></span> | <span data-ttu-id="daa71-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daa71-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="daa71-162">message</span><span class="sxs-lookup"><span data-stu-id="daa71-162">message</span></span>](../resources/message.md) | <span data-ttu-id="daa71-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="daa71-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="daa71-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="daa71-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="daa71-166">security alert</span><span class="sxs-lookup"><span data-stu-id="daa71-166">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="daa71-167">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daa71-167">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="daa71-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daa71-168">Not supported</span></span> | <span data-ttu-id="daa71-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daa71-169">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="daa71-170">user</span><span class="sxs-lookup"><span data-stu-id="daa71-170">user</span></span>](../resources/user.md) | <span data-ttu-id="daa71-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-171">User.Read.All</span></span> | <span data-ttu-id="daa71-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-172">User.Read.All</span></span> | <span data-ttu-id="daa71-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa71-173">User.Read.All</span></span> |

> <span data-ttu-id="daa71-174">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="daa71-174">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="daa71-175">driveItem</span><span class="sxs-lookup"><span data-stu-id="daa71-175">driveItem</span></span>

<span data-ttu-id="daa71-176">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="daa71-176">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="daa71-177">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="daa71-177">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="daa71-178">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="daa71-178">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="daa71-179">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="daa71-179">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="daa71-180">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="daa71-180">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="daa71-181">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="daa71-181">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="daa71-182">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="daa71-182">contact, event, and message</span></span>

<span data-ttu-id="daa71-183">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="daa71-183">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="daa71-184">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="daa71-184">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="daa71-185">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="daa71-185">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="daa71-186">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="daa71-186">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="daa71-187">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="daa71-187">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="daa71-188">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="daa71-188">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="daa71-189">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="daa71-189">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="daa71-190">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daa71-190">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="daa71-191">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="daa71-191">Optional query parameters</span></span>

<span data-ttu-id="daa71-192">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="daa71-192">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="daa71-193">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="daa71-193">Request headers</span></span>

| <span data-ttu-id="daa71-194">Имя</span><span class="sxs-lookup"><span data-stu-id="daa71-194">Name</span></span>       | <span data-ttu-id="daa71-195">Тип</span><span class="sxs-lookup"><span data-stu-id="daa71-195">Type</span></span> | <span data-ttu-id="daa71-196">Описание</span><span class="sxs-lookup"><span data-stu-id="daa71-196">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="daa71-197">Authorization</span><span class="sxs-lookup"><span data-stu-id="daa71-197">Authorization</span></span>  | <span data-ttu-id="daa71-198">string</span><span class="sxs-lookup"><span data-stu-id="daa71-198">string</span></span>  | <span data-ttu-id="daa71-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="daa71-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="daa71-201">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="daa71-201">Request body</span></span>

<span data-ttu-id="daa71-202">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="daa71-202">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daa71-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="daa71-203">Response</span></span>

<span data-ttu-id="daa71-204">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="daa71-204">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daa71-205">Пример</span><span class="sxs-lookup"><span data-stu-id="daa71-205">Example</span></span>

##### <a name="request"></a><span data-ttu-id="daa71-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="daa71-206">Request</span></span>

<span data-ttu-id="daa71-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="daa71-207">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="daa71-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="daa71-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="daa71-209">C#</span><span class="sxs-lookup"><span data-stu-id="daa71-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="daa71-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="daa71-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="daa71-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="daa71-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="daa71-212">Java</span><span class="sxs-lookup"><span data-stu-id="daa71-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="daa71-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="daa71-213">Response</span></span>

<span data-ttu-id="daa71-214">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="daa71-214">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

