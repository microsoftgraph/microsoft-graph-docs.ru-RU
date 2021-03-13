---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 93b614c8ba93b5643b5f630294e40fee1edf002c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761537"
---
# <a name="get-subscription"></a><span data-ttu-id="6525d-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="6525d-103">Get subscription</span></span>

<span data-ttu-id="6525d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6525d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6525d-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="6525d-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="6525d-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="6525d-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="6525d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6525d-107">Permissions</span></span>

<span data-ttu-id="6525d-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6525d-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6525d-109">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6525d-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6525d-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="6525d-110">Supported resource</span></span> | <span data-ttu-id="6525d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6525d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6525d-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6525d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6525d-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="6525d-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6525d-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="6525d-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="6525d-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-115">Not supported</span></span> | <span data-ttu-id="6525d-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-116">Not supported</span></span> | <span data-ttu-id="6525d-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-117">CallRecords.Read.All</span></span> |
|<span data-ttu-id="6525d-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6525d-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6525d-119">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-119">ChannelMessage.Read.All</span></span> | <span data-ttu-id="6525d-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-120">Not supported</span></span> |  <span data-ttu-id="6525d-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6525d-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="6525d-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6525d-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-123">Not supported</span></span> | <span data-ttu-id="6525d-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-124">Not supported</span></span> | <span data-ttu-id="6525d-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6525d-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6525d-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6525d-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-127">Not supported</span></span> | <span data-ttu-id="6525d-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-128">Not supported</span></span> | <span data-ttu-id="6525d-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="6525d-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="6525d-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6525d-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-131">Not supported</span></span> | <span data-ttu-id="6525d-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-132">Not supported</span></span> | <span data-ttu-id="6525d-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6525d-134">contact</span><span class="sxs-lookup"><span data-stu-id="6525d-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6525d-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-135">Contacts.Read</span></span> | <span data-ttu-id="6525d-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-136">Contacts.Read</span></span> | <span data-ttu-id="6525d-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-137">Contacts.Read</span></span> |
|<span data-ttu-id="6525d-138">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="6525d-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6525d-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-139">Not supported</span></span> | <span data-ttu-id="6525d-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6525d-140">Files.ReadWrite</span></span> | <span data-ttu-id="6525d-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-141">Not supported</span></span> |
|<span data-ttu-id="6525d-142">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6525d-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6525d-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6525d-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="6525d-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-144">Not supported</span></span> | <span data-ttu-id="6525d-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6525d-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6525d-146">event</span><span class="sxs-lookup"><span data-stu-id="6525d-146">event</span></span>](../resources/event.md) | <span data-ttu-id="6525d-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-147">Calendars.Read</span></span> | <span data-ttu-id="6525d-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-148">Calendars.Read</span></span> | <span data-ttu-id="6525d-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-149">Calendars.Read</span></span> |
|[<span data-ttu-id="6525d-150">group</span><span class="sxs-lookup"><span data-stu-id="6525d-150">group</span></span>](../resources/group.md) | <span data-ttu-id="6525d-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-151">Group.Read.All</span></span> | <span data-ttu-id="6525d-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-152">Not supported</span></span> | <span data-ttu-id="6525d-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-153">Group.Read.All</span></span> |
|[<span data-ttu-id="6525d-154">group conversation</span><span class="sxs-lookup"><span data-stu-id="6525d-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6525d-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-155">Group.Read.All</span></span> | <span data-ttu-id="6525d-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-156">Not supported</span></span> | <span data-ttu-id="6525d-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-157">Not supported</span></span> |
|[<span data-ttu-id="6525d-158">list</span><span class="sxs-lookup"><span data-stu-id="6525d-158">list</span></span>](../resources/list.md) | <span data-ttu-id="6525d-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6525d-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6525d-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-160">Not supported</span></span> | <span data-ttu-id="6525d-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6525d-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6525d-162">message</span><span class="sxs-lookup"><span data-stu-id="6525d-162">message</span></span>](../resources/message.md) | <span data-ttu-id="6525d-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6525d-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6525d-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6525d-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6525d-166">security alert</span><span class="sxs-lookup"><span data-stu-id="6525d-166">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6525d-167">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6525d-167">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6525d-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6525d-168">Not supported</span></span> | <span data-ttu-id="6525d-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6525d-169">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6525d-170">user</span><span class="sxs-lookup"><span data-stu-id="6525d-170">user</span></span>](../resources/user.md) | <span data-ttu-id="6525d-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-171">User.Read.All</span></span> | <span data-ttu-id="6525d-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-172">User.Read.All</span></span> | <span data-ttu-id="6525d-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6525d-173">User.Read.All</span></span> |

> <span data-ttu-id="6525d-174">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="6525d-174">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="6525d-175">driveItem</span><span class="sxs-lookup"><span data-stu-id="6525d-175">driveItem</span></span>

<span data-ttu-id="6525d-176">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6525d-176">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="6525d-177">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6525d-177">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6525d-178">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="6525d-178">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6525d-179">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="6525d-179">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6525d-180">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="6525d-180">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6525d-181">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="6525d-181">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6525d-182">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="6525d-182">contact, event, and message</span></span>

<span data-ttu-id="6525d-183">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="6525d-183">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6525d-184">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6525d-184">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6525d-185">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="6525d-185">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6525d-186">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6525d-186">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6525d-187">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="6525d-187">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6525d-188">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6525d-188">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6525d-189">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="6525d-189">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="6525d-190">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6525d-190">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6525d-191">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6525d-191">Optional query parameters</span></span>

<span data-ttu-id="6525d-192">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6525d-192">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6525d-193">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6525d-193">Request headers</span></span>

| <span data-ttu-id="6525d-194">Имя</span><span class="sxs-lookup"><span data-stu-id="6525d-194">Name</span></span>       | <span data-ttu-id="6525d-195">Тип</span><span class="sxs-lookup"><span data-stu-id="6525d-195">Type</span></span> | <span data-ttu-id="6525d-196">Описание</span><span class="sxs-lookup"><span data-stu-id="6525d-196">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6525d-197">Authorization</span><span class="sxs-lookup"><span data-stu-id="6525d-197">Authorization</span></span>  | <span data-ttu-id="6525d-198">string</span><span class="sxs-lookup"><span data-stu-id="6525d-198">string</span></span>  | <span data-ttu-id="6525d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6525d-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6525d-201">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6525d-201">Request body</span></span>

<span data-ttu-id="6525d-202">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6525d-202">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6525d-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="6525d-203">Response</span></span>

<span data-ttu-id="6525d-204">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6525d-204">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6525d-205">Пример</span><span class="sxs-lookup"><span data-stu-id="6525d-205">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6525d-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="6525d-206">Request</span></span>

<span data-ttu-id="6525d-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6525d-207">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6525d-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="6525d-208">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="6525d-209">C#</span><span class="sxs-lookup"><span data-stu-id="6525d-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6525d-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6525d-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6525d-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6525d-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6525d-212">Java</span><span class="sxs-lookup"><span data-stu-id="6525d-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6525d-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="6525d-213">Response</span></span>

<span data-ttu-id="6525d-214">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6525d-214">Here is an example of the response.</span></span>
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

