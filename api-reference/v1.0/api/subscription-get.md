---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Priority
author: piotrci
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fdd850b5965e20b4de2602368c3ece3fe47b65b5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703807"
---
# <a name="get-subscription"></a><span data-ttu-id="9fd39-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="9fd39-103">Get subscription</span></span>

<span data-ttu-id="9fd39-104">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="9fd39-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fd39-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fd39-105">Permissions</span></span>

<span data-ttu-id="9fd39-106">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9fd39-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="9fd39-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fd39-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9fd39-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="9fd39-108">Supported resource</span></span> | <span data-ttu-id="9fd39-109">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fd39-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9fd39-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fd39-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fd39-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fd39-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="9fd39-112">contact</span><span class="sxs-lookup"><span data-stu-id="9fd39-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="9fd39-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-113">Contacts.Read</span></span> | <span data-ttu-id="9fd39-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-114">Contacts.Read</span></span> | <span data-ttu-id="9fd39-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-115">Contacts.Read</span></span> |
|<span data-ttu-id="9fd39-116">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="9fd39-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="9fd39-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fd39-117">Not supported</span></span> | <span data-ttu-id="9fd39-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fd39-118">Files.ReadWrite</span></span> | <span data-ttu-id="9fd39-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fd39-119">Not supported</span></span> |
|<span data-ttu-id="9fd39-120">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="9fd39-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="9fd39-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="9fd39-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fd39-122">Not supported</span></span> | <span data-ttu-id="9fd39-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="9fd39-124">event</span><span class="sxs-lookup"><span data-stu-id="9fd39-124">event</span></span>](../resources/event.md) | <span data-ttu-id="9fd39-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-125">Calendars.Read</span></span> | <span data-ttu-id="9fd39-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-126">Calendars.Read</span></span> | <span data-ttu-id="9fd39-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-127">Calendars.Read</span></span> |
|[<span data-ttu-id="9fd39-128">group</span><span class="sxs-lookup"><span data-stu-id="9fd39-128">group</span></span>](../resources/group.md) | <span data-ttu-id="9fd39-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-129">Group.Read.All</span></span> | <span data-ttu-id="9fd39-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fd39-130">Not supported</span></span> | <span data-ttu-id="9fd39-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-131">Group.Read.All</span></span> |
|[<span data-ttu-id="9fd39-132">group conversation</span><span class="sxs-lookup"><span data-stu-id="9fd39-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="9fd39-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-133">Group.Read.All</span></span> | <span data-ttu-id="9fd39-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fd39-134">Not supported</span></span> | <span data-ttu-id="9fd39-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fd39-135">Not supported</span></span> |
|[<span data-ttu-id="9fd39-136">message</span><span class="sxs-lookup"><span data-stu-id="9fd39-136">message</span></span>](../resources/message.md) | <span data-ttu-id="9fd39-137">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-137">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="9fd39-138">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-138">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="9fd39-139">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9fd39-139">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="9fd39-140">security alert</span><span class="sxs-lookup"><span data-stu-id="9fd39-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="9fd39-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="9fd39-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9fd39-142">Not supported</span></span> | <span data-ttu-id="9fd39-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="9fd39-144">user</span><span class="sxs-lookup"><span data-stu-id="9fd39-144">user</span></span>](../resources/user.md) | <span data-ttu-id="9fd39-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-145">User.Read.All</span></span> | <span data-ttu-id="9fd39-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-146">User.Read.All</span></span> | <span data-ttu-id="9fd39-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fd39-147">User.Read.All</span></span> |

> <span data-ttu-id="9fd39-148">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="9fd39-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="9fd39-149">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="9fd39-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="9fd39-150">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="9fd39-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="9fd39-151">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="9fd39-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="9fd39-152">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="9fd39-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="9fd39-153">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="9fd39-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="9fd39-154">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="9fd39-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="9fd39-155">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9fd39-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="9fd39-156">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="9fd39-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="9fd39-157">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="9fd39-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="9fd39-158">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="9fd39-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="9fd39-159">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fd39-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9fd39-160">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9fd39-160">Optional query parameters</span></span>

<span data-ttu-id="9fd39-161">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9fd39-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fd39-162">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fd39-162">Request headers</span></span>

| <span data-ttu-id="9fd39-163">Имя</span><span class="sxs-lookup"><span data-stu-id="9fd39-163">Name</span></span>       | <span data-ttu-id="9fd39-164">Тип</span><span class="sxs-lookup"><span data-stu-id="9fd39-164">Type</span></span> | <span data-ttu-id="9fd39-165">Описание</span><span class="sxs-lookup"><span data-stu-id="9fd39-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9fd39-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fd39-166">Authorization</span></span>  | <span data-ttu-id="9fd39-167">string</span><span class="sxs-lookup"><span data-stu-id="9fd39-167">string</span></span>  | <span data-ttu-id="9fd39-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fd39-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fd39-170">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fd39-170">Request body</span></span>

<span data-ttu-id="9fd39-171">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fd39-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fd39-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fd39-172">Response</span></span>

<span data-ttu-id="9fd39-173">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fd39-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fd39-174">Пример</span><span class="sxs-lookup"><span data-stu-id="9fd39-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9fd39-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fd39-175">Request</span></span>

<span data-ttu-id="9fd39-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fd39-176">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9fd39-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd39-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fd39-178">C#</span><span class="sxs-lookup"><span data-stu-id="9fd39-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fd39-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fd39-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fd39-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fd39-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9fd39-181">Java</span><span class="sxs-lookup"><span data-stu-id="9fd39-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9fd39-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fd39-182">Response</span></span>

<span data-ttu-id="9fd39-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fd39-183">Here is an example of the response.</span></span>
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
  "creatorId": "string"
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
