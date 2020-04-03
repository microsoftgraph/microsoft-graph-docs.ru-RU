---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d8a434c6760635fef602b77bbc6631d52c666f40
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108461"
---
# <a name="update-subscription"></a><span data-ttu-id="d3448-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="d3448-103">Update subscription</span></span>

<span data-ttu-id="d3448-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3448-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3448-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="d3448-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="d3448-106">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="d3448-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="d3448-107">Чтобы избежать отсутствия уведомлений, приложение должно хорошо обновлять свои подписки в течение срока их действия.</span><span class="sxs-lookup"><span data-stu-id="d3448-107">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="d3448-108">В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d3448-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3448-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3448-109">Permissions</span></span>

<span data-ttu-id="d3448-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d3448-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d3448-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3448-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3448-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="d3448-112">Supported resource</span></span> | <span data-ttu-id="d3448-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3448-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d3448-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3448-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3448-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3448-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="d3448-116">contact</span><span class="sxs-lookup"><span data-stu-id="d3448-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d3448-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-117">Contacts.Read</span></span> | <span data-ttu-id="d3448-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-118">Contacts.Read</span></span> | <span data-ttu-id="d3448-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-119">Contacts.Read</span></span> |
|<span data-ttu-id="d3448-120">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="d3448-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="d3448-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3448-121">Not supported</span></span> | <span data-ttu-id="d3448-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3448-122">Files.ReadWrite</span></span> | <span data-ttu-id="d3448-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3448-123">Not supported</span></span> |
|<span data-ttu-id="d3448-124">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="d3448-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="d3448-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3448-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="d3448-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3448-126">Not supported</span></span> | <span data-ttu-id="d3448-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3448-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="d3448-128">event</span><span class="sxs-lookup"><span data-stu-id="d3448-128">event</span></span>](../resources/event.md) | <span data-ttu-id="d3448-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-129">Calendars.Read</span></span> | <span data-ttu-id="d3448-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-130">Calendars.Read</span></span> | <span data-ttu-id="d3448-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-131">Calendars.Read</span></span> |
|[<span data-ttu-id="d3448-132">group</span><span class="sxs-lookup"><span data-stu-id="d3448-132">group</span></span>](../resources/group.md) | <span data-ttu-id="d3448-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3448-133">Group.Read.All</span></span> | <span data-ttu-id="d3448-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3448-134">Not supported</span></span> | <span data-ttu-id="d3448-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3448-135">Group.Read.All</span></span> |
|[<span data-ttu-id="d3448-136">group conversation</span><span class="sxs-lookup"><span data-stu-id="d3448-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="d3448-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3448-137">Group.Read.All</span></span> | <span data-ttu-id="d3448-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3448-138">Not supported</span></span> | <span data-ttu-id="d3448-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3448-139">Not supported</span></span> |
|[<span data-ttu-id="d3448-140">list</span><span class="sxs-lookup"><span data-stu-id="d3448-140">list</span></span>](../resources/list.md) | <span data-ttu-id="d3448-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3448-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="d3448-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3448-142">Not supported</span></span> | <span data-ttu-id="d3448-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3448-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="d3448-144">message</span><span class="sxs-lookup"><span data-stu-id="d3448-144">message</span></span>](../resources/message.md) | <span data-ttu-id="d3448-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d3448-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d3448-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d3448-147">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="d3448-148">security alert</span><span class="sxs-lookup"><span data-stu-id="d3448-148">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="d3448-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3448-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="d3448-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3448-150">Not supported</span></span> | <span data-ttu-id="d3448-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3448-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="d3448-152">user</span><span class="sxs-lookup"><span data-stu-id="d3448-152">user</span></span>](../resources/user.md) | <span data-ttu-id="d3448-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3448-153">User.Read.All</span></span> | <span data-ttu-id="d3448-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3448-154">User.Read.All</span></span> | <span data-ttu-id="d3448-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3448-155">User.Read.All</span></span> |

> <span data-ttu-id="d3448-156">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="d3448-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="d3448-157">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="d3448-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="d3448-158">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="d3448-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="d3448-159">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="d3448-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="d3448-160">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="d3448-160">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="d3448-161">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="d3448-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="d3448-162">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="d3448-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="d3448-163">Это означает, например, вы не можете использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3448-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="d3448-164">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="d3448-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="d3448-165">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d3448-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="d3448-166">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="d3448-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="d3448-167">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3448-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d3448-168">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3448-168">Request headers</span></span>

| <span data-ttu-id="d3448-169">Имя</span><span class="sxs-lookup"><span data-stu-id="d3448-169">Name</span></span>       | <span data-ttu-id="d3448-170">Тип</span><span class="sxs-lookup"><span data-stu-id="d3448-170">Type</span></span> | <span data-ttu-id="d3448-171">Описание</span><span class="sxs-lookup"><span data-stu-id="d3448-171">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d3448-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3448-172">Authorization</span></span>  | <span data-ttu-id="d3448-173">string</span><span class="sxs-lookup"><span data-stu-id="d3448-173">string</span></span>  | <span data-ttu-id="d3448-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3448-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d3448-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3448-176">Response</span></span>

<span data-ttu-id="d3448-177">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3448-177">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3448-178">Пример</span><span class="sxs-lookup"><span data-stu-id="d3448-178">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d3448-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3448-179">Request</span></span>

<span data-ttu-id="d3448-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3448-180">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3448-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3448-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="d3448-182">C#</span><span class="sxs-lookup"><span data-stu-id="d3448-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3448-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3448-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3448-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3448-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3448-185">Java</span><span class="sxs-lookup"><span data-stu-id="d3448-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d3448-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3448-186">Response</span></span>

<span data-ttu-id="d3448-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3448-187">Here is an example of the response.</span></span>
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
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
