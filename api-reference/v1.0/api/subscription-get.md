---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 5d2590afad93560bab0a72eb8edd007779f4711b
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108580"
---
# <a name="get-subscription"></a><span data-ttu-id="c31dd-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="c31dd-103">Get subscription</span></span>

<span data-ttu-id="c31dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c31dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c31dd-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="c31dd-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="c31dd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c31dd-106">Permissions</span></span>

<span data-ttu-id="c31dd-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c31dd-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c31dd-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c31dd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c31dd-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="c31dd-109">Supported resource</span></span> | <span data-ttu-id="c31dd-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c31dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c31dd-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c31dd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c31dd-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c31dd-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="c31dd-113">contact</span><span class="sxs-lookup"><span data-stu-id="c31dd-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c31dd-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-114">Contacts.Read</span></span> | <span data-ttu-id="c31dd-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-115">Contacts.Read</span></span> | <span data-ttu-id="c31dd-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-116">Contacts.Read</span></span> |
|<span data-ttu-id="c31dd-117">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="c31dd-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="c31dd-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c31dd-118">Not supported</span></span> | <span data-ttu-id="c31dd-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c31dd-119">Files.ReadWrite</span></span> | <span data-ttu-id="c31dd-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c31dd-120">Not supported</span></span> |
|<span data-ttu-id="c31dd-121">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="c31dd-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="c31dd-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="c31dd-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c31dd-123">Not supported</span></span> | <span data-ttu-id="c31dd-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="c31dd-125">event</span><span class="sxs-lookup"><span data-stu-id="c31dd-125">event</span></span>](../resources/event.md) | <span data-ttu-id="c31dd-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-126">Calendars.Read</span></span> | <span data-ttu-id="c31dd-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-127">Calendars.Read</span></span> | <span data-ttu-id="c31dd-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-128">Calendars.Read</span></span> |
|[<span data-ttu-id="c31dd-129">group</span><span class="sxs-lookup"><span data-stu-id="c31dd-129">group</span></span>](../resources/group.md) | <span data-ttu-id="c31dd-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-130">Group.Read.All</span></span> | <span data-ttu-id="c31dd-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c31dd-131">Not supported</span></span> | <span data-ttu-id="c31dd-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-132">Group.Read.All</span></span> |
|[<span data-ttu-id="c31dd-133">group conversation</span><span class="sxs-lookup"><span data-stu-id="c31dd-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="c31dd-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-134">Group.Read.All</span></span> | <span data-ttu-id="c31dd-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c31dd-135">Not supported</span></span> | <span data-ttu-id="c31dd-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c31dd-136">Not supported</span></span> |
|[<span data-ttu-id="c31dd-137">list</span><span class="sxs-lookup"><span data-stu-id="c31dd-137">list</span></span>](../resources/list.md) | <span data-ttu-id="c31dd-138">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-138">Sites.ReadWrite.All</span></span> | <span data-ttu-id="c31dd-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c31dd-139">Not supported</span></span> | <span data-ttu-id="c31dd-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-140">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="c31dd-141">message</span><span class="sxs-lookup"><span data-stu-id="c31dd-141">message</span></span>](../resources/message.md) | <span data-ttu-id="c31dd-142">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-142">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c31dd-143">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-143">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c31dd-144">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c31dd-144">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="c31dd-145">security alert</span><span class="sxs-lookup"><span data-stu-id="c31dd-145">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="c31dd-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-146">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="c31dd-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c31dd-147">Not supported</span></span> | <span data-ttu-id="c31dd-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-148">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="c31dd-149">user</span><span class="sxs-lookup"><span data-stu-id="c31dd-149">user</span></span>](../resources/user.md) | <span data-ttu-id="c31dd-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-150">User.Read.All</span></span> | <span data-ttu-id="c31dd-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-151">User.Read.All</span></span> | <span data-ttu-id="c31dd-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c31dd-152">User.Read.All</span></span> |

> <span data-ttu-id="c31dd-153">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="c31dd-153">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="c31dd-154">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="c31dd-154">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="c31dd-155">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="c31dd-155">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="c31dd-156">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="c31dd-156">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="c31dd-157">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="c31dd-157">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="c31dd-158">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="c31dd-158">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="c31dd-159">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="c31dd-159">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="c31dd-160">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c31dd-160">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="c31dd-161">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="c31dd-161">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="c31dd-162">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c31dd-162">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="c31dd-163">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="c31dd-163">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="c31dd-164">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c31dd-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c31dd-165">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c31dd-165">Optional query parameters</span></span>

<span data-ttu-id="c31dd-166">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c31dd-166">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c31dd-167">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c31dd-167">Request headers</span></span>

| <span data-ttu-id="c31dd-168">Имя</span><span class="sxs-lookup"><span data-stu-id="c31dd-168">Name</span></span>       | <span data-ttu-id="c31dd-169">Тип</span><span class="sxs-lookup"><span data-stu-id="c31dd-169">Type</span></span> | <span data-ttu-id="c31dd-170">Описание</span><span class="sxs-lookup"><span data-stu-id="c31dd-170">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c31dd-171">Authorization</span><span class="sxs-lookup"><span data-stu-id="c31dd-171">Authorization</span></span>  | <span data-ttu-id="c31dd-172">string</span><span class="sxs-lookup"><span data-stu-id="c31dd-172">string</span></span>  | <span data-ttu-id="c31dd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c31dd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c31dd-175">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c31dd-175">Request body</span></span>

<span data-ttu-id="c31dd-176">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c31dd-176">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c31dd-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="c31dd-177">Response</span></span>

<span data-ttu-id="c31dd-178">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c31dd-178">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c31dd-179">Пример</span><span class="sxs-lookup"><span data-stu-id="c31dd-179">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c31dd-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="c31dd-180">Request</span></span>

<span data-ttu-id="c31dd-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c31dd-181">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c31dd-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="c31dd-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="c31dd-183">C#</span><span class="sxs-lookup"><span data-stu-id="c31dd-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c31dd-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c31dd-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c31dd-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c31dd-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c31dd-186">Java</span><span class="sxs-lookup"><span data-stu-id="c31dd-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c31dd-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="c31dd-187">Response</span></span>

<span data-ttu-id="c31dd-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c31dd-188">Here is an example of the response.</span></span>
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
