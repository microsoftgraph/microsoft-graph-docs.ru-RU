---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 08bb1904d446355dd4d953d09dc136d5b8a6008f
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394468"
---
# <a name="update-subscription"></a><span data-ttu-id="711b6-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="711b6-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="711b6-104">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="711b6-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="711b6-105">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="711b6-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="711b6-106">Чтобы избежать отсутствия уведомлений, приложение должно хорошо обновлять свои подписки в течение срока их действия.</span><span class="sxs-lookup"><span data-stu-id="711b6-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="711b6-107">В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="711b6-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="711b6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="711b6-108">Permissions</span></span>

<span data-ttu-id="711b6-109">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="711b6-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="711b6-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="711b6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="711b6-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="711b6-111">Supported resource</span></span> | <span data-ttu-id="711b6-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="711b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="711b6-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="711b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="711b6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="711b6-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="711b6-115">каллрекорд</span><span class="sxs-lookup"><span data-stu-id="711b6-115">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="711b6-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-116">Not supported</span></span> | <span data-ttu-id="711b6-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-117">Not supported</span></span> | <span data-ttu-id="711b6-118">Каллрекордс. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="711b6-118">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="711b6-119">contact</span><span class="sxs-lookup"><span data-stu-id="711b6-119">contact</span></span>](../resources/contact.md) | <span data-ttu-id="711b6-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-120">Contacts.Read</span></span> | <span data-ttu-id="711b6-121">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-121">Contacts.Read</span></span> | <span data-ttu-id="711b6-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-122">Contacts.Read</span></span> |
|<span data-ttu-id="711b6-123">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="711b6-123">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="711b6-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-124">Not supported</span></span> | <span data-ttu-id="711b6-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="711b6-125">Files.ReadWrite</span></span> | <span data-ttu-id="711b6-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-126">Not supported</span></span> |
|<span data-ttu-id="711b6-127">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="711b6-127">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="711b6-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="711b6-128">Files.ReadWrite.All</span></span> | <span data-ttu-id="711b6-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-129">Not supported</span></span> | <span data-ttu-id="711b6-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="711b6-130">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="711b6-131">event</span><span class="sxs-lookup"><span data-stu-id="711b6-131">event</span></span>](../resources/event.md) | <span data-ttu-id="711b6-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-132">Calendars.Read</span></span> | <span data-ttu-id="711b6-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-133">Calendars.Read</span></span> | <span data-ttu-id="711b6-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-134">Calendars.Read</span></span> |
|[<span data-ttu-id="711b6-135">group</span><span class="sxs-lookup"><span data-stu-id="711b6-135">group</span></span>](../resources/group.md) | <span data-ttu-id="711b6-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="711b6-136">Group.Read.All</span></span> | <span data-ttu-id="711b6-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-137">Not supported</span></span> | <span data-ttu-id="711b6-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="711b6-138">Group.Read.All</span></span> |
|[<span data-ttu-id="711b6-139">group conversation</span><span class="sxs-lookup"><span data-stu-id="711b6-139">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="711b6-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="711b6-140">Group.Read.All</span></span> | <span data-ttu-id="711b6-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-141">Not supported</span></span> | <span data-ttu-id="711b6-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-142">Not supported</span></span> |
|[<span data-ttu-id="711b6-143">list</span><span class="sxs-lookup"><span data-stu-id="711b6-143">list</span></span>](../resources/list.md) | <span data-ttu-id="711b6-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="711b6-144">Sites.ReadWrite.All</span></span> | <span data-ttu-id="711b6-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-145">Not supported</span></span> | <span data-ttu-id="711b6-146">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="711b6-146">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="711b6-147">message</span><span class="sxs-lookup"><span data-stu-id="711b6-147">message</span></span>](../resources/message.md) | <span data-ttu-id="711b6-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="711b6-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-149">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="711b6-150">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="711b6-150">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="711b6-151">security alert</span><span class="sxs-lookup"><span data-stu-id="711b6-151">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="711b6-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="711b6-152">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="711b6-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="711b6-153">Not supported</span></span> | <span data-ttu-id="711b6-154">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="711b6-154">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="711b6-155">user</span><span class="sxs-lookup"><span data-stu-id="711b6-155">user</span></span>](../resources/user.md) | <span data-ttu-id="711b6-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="711b6-156">User.Read.All</span></span> | <span data-ttu-id="711b6-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="711b6-157">User.Read.All</span></span> | <span data-ttu-id="711b6-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="711b6-158">User.Read.All</span></span> |

> <span data-ttu-id="711b6-159">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="711b6-159">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="711b6-160">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="711b6-160">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="711b6-161">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="711b6-161">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="711b6-162">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="711b6-162">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="711b6-163">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="711b6-163">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="711b6-164">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="711b6-164">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="711b6-165">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="711b6-165">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="711b6-166">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="711b6-166">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="711b6-167">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="711b6-167">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="711b6-168">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="711b6-168">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="711b6-169">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="711b6-169">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="711b6-170">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="711b6-170">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="711b6-171">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="711b6-171">Request headers</span></span>

| <span data-ttu-id="711b6-172">Имя</span><span class="sxs-lookup"><span data-stu-id="711b6-172">Name</span></span>       | <span data-ttu-id="711b6-173">Тип</span><span class="sxs-lookup"><span data-stu-id="711b6-173">Type</span></span> | <span data-ttu-id="711b6-174">Описание</span><span class="sxs-lookup"><span data-stu-id="711b6-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="711b6-175">Authorization</span><span class="sxs-lookup"><span data-stu-id="711b6-175">Authorization</span></span>  | <span data-ttu-id="711b6-176">string</span><span class="sxs-lookup"><span data-stu-id="711b6-176">string</span></span>  | <span data-ttu-id="711b6-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="711b6-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="711b6-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="711b6-179">Response</span></span>

<span data-ttu-id="711b6-180">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="711b6-180">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="711b6-181">Пример</span><span class="sxs-lookup"><span data-stu-id="711b6-181">Example</span></span>

##### <a name="request"></a><span data-ttu-id="711b6-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="711b6-182">Request</span></span>

<span data-ttu-id="711b6-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="711b6-183">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="711b6-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="711b6-184">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="711b6-185">C#</span><span class="sxs-lookup"><span data-stu-id="711b6-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="711b6-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="711b6-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="711b6-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="711b6-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="711b6-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="711b6-188">Response</span></span>

<span data-ttu-id="711b6-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="711b6-189">Here is an example of the response.</span></span>
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
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
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
