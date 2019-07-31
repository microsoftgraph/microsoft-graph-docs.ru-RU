---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: cc37f1fa204c7211ee2489d6b94283b045a5cf97
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977820"
---
# <a name="update-subscription"></a><span data-ttu-id="b162d-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="b162d-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b162d-104">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="b162d-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="b162d-105">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="b162d-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="b162d-106">Чтобы избежать отсутствия уведомлений, приложение должно хорошо обновлять свои подписки в течение срока их действия.</span><span class="sxs-lookup"><span data-stu-id="b162d-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="b162d-107">В [](../resources/subscription.md) этой статье приведены сведения о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="b162d-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="b162d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b162d-108">Permissions</span></span>

<span data-ttu-id="b162d-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b162d-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b162d-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b162d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b162d-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="b162d-111">Supported resource</span></span> | <span data-ttu-id="b162d-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b162d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b162d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b162d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b162d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b162d-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="b162d-115">contact</span><span class="sxs-lookup"><span data-stu-id="b162d-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="b162d-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-116">Contacts.Read</span></span> | <span data-ttu-id="b162d-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-117">Contacts.Read</span></span> | <span data-ttu-id="b162d-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-118">Contacts.Read</span></span> |
|<span data-ttu-id="b162d-119">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="b162d-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="b162d-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b162d-120">Not supported</span></span> | <span data-ttu-id="b162d-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b162d-121">Files.ReadWrite</span></span> | <span data-ttu-id="b162d-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b162d-122">Not supported</span></span> |
|<span data-ttu-id="b162d-123">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="b162d-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="b162d-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b162d-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="b162d-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b162d-125">Not supported</span></span> | <span data-ttu-id="b162d-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b162d-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="b162d-127">event</span><span class="sxs-lookup"><span data-stu-id="b162d-127">event</span></span>](../resources/event.md) | <span data-ttu-id="b162d-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-128">Calendars.Read</span></span> | <span data-ttu-id="b162d-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-129">Calendars.Read</span></span> | <span data-ttu-id="b162d-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-130">Calendars.Read</span></span> |
|[<span data-ttu-id="b162d-131">group</span><span class="sxs-lookup"><span data-stu-id="b162d-131">group</span></span>](../resources/group.md) | <span data-ttu-id="b162d-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b162d-132">Group.Read.All</span></span> | <span data-ttu-id="b162d-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b162d-133">Not supported</span></span> | <span data-ttu-id="b162d-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b162d-134">Group.Read.All</span></span> |
|[<span data-ttu-id="b162d-135">group conversation</span><span class="sxs-lookup"><span data-stu-id="b162d-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="b162d-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b162d-136">Group.Read.All</span></span> | <span data-ttu-id="b162d-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b162d-137">Not supported</span></span> | <span data-ttu-id="b162d-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b162d-138">Not supported</span></span> |
|[<span data-ttu-id="b162d-139">message</span><span class="sxs-lookup"><span data-stu-id="b162d-139">message</span></span>](../resources/message.md) | <span data-ttu-id="b162d-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-140">Mail.Read</span></span> | <span data-ttu-id="b162d-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-141">Mail.Read</span></span> | <span data-ttu-id="b162d-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b162d-142">Mail.Read</span></span> |
|[<span data-ttu-id="b162d-143">security alert</span><span class="sxs-lookup"><span data-stu-id="b162d-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="b162d-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b162d-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="b162d-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b162d-145">Not supported</span></span> | <span data-ttu-id="b162d-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b162d-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="b162d-147">user</span><span class="sxs-lookup"><span data-stu-id="b162d-147">user</span></span>](../resources/user.md) | <span data-ttu-id="b162d-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b162d-148">User.Read.All</span></span> | <span data-ttu-id="b162d-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b162d-149">User.Read.All</span></span> | <span data-ttu-id="b162d-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b162d-150">User.Read.All</span></span> |

> <span data-ttu-id="b162d-151">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="b162d-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="b162d-152">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="b162d-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="b162d-153">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="b162d-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="b162d-154">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="b162d-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="b162d-155">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="b162d-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="b162d-156">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="b162d-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="b162d-157">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="b162d-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="b162d-158">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b162d-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="b162d-159">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="b162d-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="b162d-160">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b162d-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="b162d-161">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="b162d-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="b162d-162">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b162d-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b162d-163">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b162d-163">Request headers</span></span>

| <span data-ttu-id="b162d-164">Имя</span><span class="sxs-lookup"><span data-stu-id="b162d-164">Name</span></span>       | <span data-ttu-id="b162d-165">Тип</span><span class="sxs-lookup"><span data-stu-id="b162d-165">Type</span></span> | <span data-ttu-id="b162d-166">Описание</span><span class="sxs-lookup"><span data-stu-id="b162d-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b162d-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="b162d-167">Authorization</span></span>  | <span data-ttu-id="b162d-168">string</span><span class="sxs-lookup"><span data-stu-id="b162d-168">string</span></span>  | <span data-ttu-id="b162d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b162d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b162d-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="b162d-171">Response</span></span>

<span data-ttu-id="b162d-172">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b162d-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b162d-173">Пример</span><span class="sxs-lookup"><span data-stu-id="b162d-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b162d-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="b162d-174">Request</span></span>

<span data-ttu-id="b162d-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b162d-175">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b162d-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="b162d-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b162d-177">C#</span><span class="sxs-lookup"><span data-stu-id="b162d-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b162d-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="b162d-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b162d-179">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b162d-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b162d-180">Java</span><span class="sxs-lookup"><span data-stu-id="b162d-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b162d-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="b162d-181">Response</span></span>

<span data-ttu-id="b162d-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b162d-182">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
