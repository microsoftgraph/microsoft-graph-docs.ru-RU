---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 9bc36204ac432714f7431cb203672f543d92e662
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038055"
---
# <a name="get-subscription"></a><span data-ttu-id="9fc13-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="9fc13-103">Get subscription</span></span>

<span data-ttu-id="9fc13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fc13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9fc13-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="9fc13-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fc13-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fc13-106">Permissions</span></span>

<span data-ttu-id="9fc13-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9fc13-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="9fc13-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fc13-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9fc13-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="9fc13-109">Supported resource</span></span> | <span data-ttu-id="9fc13-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fc13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9fc13-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fc13-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fc13-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="9fc13-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="9fc13-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="9fc13-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="9fc13-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-114">Not supported</span></span> | <span data-ttu-id="9fc13-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-115">Not supported</span></span> | <span data-ttu-id="9fc13-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-116">CallRecords.Read.All</span></span> |
|[<span data-ttu-id="9fc13-117">contact</span><span class="sxs-lookup"><span data-stu-id="9fc13-117">contact</span></span>](../resources/contact.md) | <span data-ttu-id="9fc13-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-118">Contacts.Read</span></span> | <span data-ttu-id="9fc13-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-119">Contacts.Read</span></span> | <span data-ttu-id="9fc13-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-120">Contacts.Read</span></span> |
|<span data-ttu-id="9fc13-121">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="9fc13-121">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="9fc13-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-122">Not supported</span></span> | <span data-ttu-id="9fc13-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fc13-123">Files.ReadWrite</span></span> | <span data-ttu-id="9fc13-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-124">Not supported</span></span> |
|<span data-ttu-id="9fc13-125">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="9fc13-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="9fc13-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-126">Files.ReadWrite.All</span></span> | <span data-ttu-id="9fc13-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-127">Not supported</span></span> | <span data-ttu-id="9fc13-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-128">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="9fc13-129">event</span><span class="sxs-lookup"><span data-stu-id="9fc13-129">event</span></span>](../resources/event.md) | <span data-ttu-id="9fc13-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-130">Calendars.Read</span></span> | <span data-ttu-id="9fc13-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-131">Calendars.Read</span></span> | <span data-ttu-id="9fc13-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-132">Calendars.Read</span></span> |
|[<span data-ttu-id="9fc13-133">group</span><span class="sxs-lookup"><span data-stu-id="9fc13-133">group</span></span>](../resources/group.md) | <span data-ttu-id="9fc13-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-134">Group.Read.All</span></span> | <span data-ttu-id="9fc13-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-135">Not supported</span></span> | <span data-ttu-id="9fc13-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-136">Group.Read.All</span></span> |
|[<span data-ttu-id="9fc13-137">group conversation</span><span class="sxs-lookup"><span data-stu-id="9fc13-137">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="9fc13-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-138">Group.Read.All</span></span> | <span data-ttu-id="9fc13-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-139">Not supported</span></span> | <span data-ttu-id="9fc13-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-140">Not supported</span></span> |
|[<span data-ttu-id="9fc13-141">list</span><span class="sxs-lookup"><span data-stu-id="9fc13-141">list</span></span>](../resources/list.md) | <span data-ttu-id="9fc13-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-142">Sites.ReadWrite.All</span></span> | <span data-ttu-id="9fc13-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-143">Not supported</span></span> | <span data-ttu-id="9fc13-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-144">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="9fc13-145">message</span><span class="sxs-lookup"><span data-stu-id="9fc13-145">message</span></span>](../resources/message.md) | <span data-ttu-id="9fc13-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="9fc13-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="9fc13-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9fc13-148">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="9fc13-149">security alert</span><span class="sxs-lookup"><span data-stu-id="9fc13-149">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="9fc13-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-150">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="9fc13-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fc13-151">Not supported</span></span> | <span data-ttu-id="9fc13-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-152">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="9fc13-153">user</span><span class="sxs-lookup"><span data-stu-id="9fc13-153">user</span></span>](../resources/user.md) | <span data-ttu-id="9fc13-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-154">User.Read.All</span></span> | <span data-ttu-id="9fc13-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-155">User.Read.All</span></span> | <span data-ttu-id="9fc13-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc13-156">User.Read.All</span></span> |

> <span data-ttu-id="9fc13-157">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="9fc13-157">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="9fc13-158">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="9fc13-158">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="9fc13-159">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="9fc13-159">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="9fc13-160">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="9fc13-160">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="9fc13-161">Уведомления об изменениях отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="9fc13-161">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="9fc13-162">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="9fc13-162">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="9fc13-163">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="9fc13-163">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="9fc13-164">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fc13-164">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="9fc13-165">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="9fc13-165">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="9fc13-166">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="9fc13-166">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="9fc13-167">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="9fc13-167">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="9fc13-168">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fc13-168">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9fc13-169">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9fc13-169">Optional query parameters</span></span>

<span data-ttu-id="9fc13-170">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9fc13-170">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fc13-171">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fc13-171">Request headers</span></span>

| <span data-ttu-id="9fc13-172">Имя</span><span class="sxs-lookup"><span data-stu-id="9fc13-172">Name</span></span>       | <span data-ttu-id="9fc13-173">Тип</span><span class="sxs-lookup"><span data-stu-id="9fc13-173">Type</span></span> | <span data-ttu-id="9fc13-174">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc13-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9fc13-175">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fc13-175">Authorization</span></span>  | <span data-ttu-id="9fc13-176">string</span><span class="sxs-lookup"><span data-stu-id="9fc13-176">string</span></span>  | <span data-ttu-id="9fc13-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fc13-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fc13-179">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fc13-179">Request body</span></span>

<span data-ttu-id="9fc13-180">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fc13-180">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fc13-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fc13-181">Response</span></span>

<span data-ttu-id="9fc13-182">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fc13-182">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fc13-183">Пример</span><span class="sxs-lookup"><span data-stu-id="9fc13-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9fc13-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fc13-184">Request</span></span>

<span data-ttu-id="9fc13-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc13-185">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9fc13-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fc13-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="9fc13-187">C#</span><span class="sxs-lookup"><span data-stu-id="9fc13-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fc13-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fc13-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fc13-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fc13-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9fc13-190">Java</span><span class="sxs-lookup"><span data-stu-id="9fc13-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9fc13-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fc13-191">Response</span></span>

<span data-ttu-id="9fc13-192">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fc13-192">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2"
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

