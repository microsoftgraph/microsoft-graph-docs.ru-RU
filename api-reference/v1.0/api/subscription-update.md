---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: aee0ca84cccd371c307b405357516d8fda61deab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038034"
---
# <a name="update-subscription"></a><span data-ttu-id="eaead-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="eaead-103">Update subscription</span></span>

<span data-ttu-id="eaead-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaead-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eaead-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="eaead-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="eaead-106">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="eaead-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="eaead-107">Чтобы избежать отсутствия уведомлений об изменениях, приложение должно правильно обновить свои подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="eaead-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="eaead-108">В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="eaead-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaead-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eaead-109">Permissions</span></span>

<span data-ttu-id="eaead-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="eaead-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="eaead-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaead-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eaead-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="eaead-112">Supported resource</span></span> | <span data-ttu-id="eaead-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaead-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eaead-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaead-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaead-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="eaead-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="eaead-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="eaead-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="eaead-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-117">Not supported</span></span> | <span data-ttu-id="eaead-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-118">Not supported</span></span> | <span data-ttu-id="eaead-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaead-119">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="eaead-120">contact</span><span class="sxs-lookup"><span data-stu-id="eaead-120">contact</span></span>](../resources/contact.md) | <span data-ttu-id="eaead-121">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-121">Contacts.Read</span></span> | <span data-ttu-id="eaead-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-122">Contacts.Read</span></span> | <span data-ttu-id="eaead-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-123">Contacts.Read</span></span> |
|<span data-ttu-id="eaead-124">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="eaead-124">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="eaead-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-125">Not supported</span></span> | <span data-ttu-id="eaead-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaead-126">Files.ReadWrite</span></span> | <span data-ttu-id="eaead-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-127">Not supported</span></span> |
|<span data-ttu-id="eaead-128">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="eaead-128">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="eaead-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaead-129">Files.ReadWrite.All</span></span> | <span data-ttu-id="eaead-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-130">Not supported</span></span> | <span data-ttu-id="eaead-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaead-131">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="eaead-132">event</span><span class="sxs-lookup"><span data-stu-id="eaead-132">event</span></span>](../resources/event.md) | <span data-ttu-id="eaead-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-133">Calendars.Read</span></span> | <span data-ttu-id="eaead-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-134">Calendars.Read</span></span> | <span data-ttu-id="eaead-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-135">Calendars.Read</span></span> |
|[<span data-ttu-id="eaead-136">group</span><span class="sxs-lookup"><span data-stu-id="eaead-136">group</span></span>](../resources/group.md) | <span data-ttu-id="eaead-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaead-137">Group.Read.All</span></span> | <span data-ttu-id="eaead-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-138">Not supported</span></span> | <span data-ttu-id="eaead-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaead-139">Group.Read.All</span></span> |
|[<span data-ttu-id="eaead-140">group conversation</span><span class="sxs-lookup"><span data-stu-id="eaead-140">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="eaead-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaead-141">Group.Read.All</span></span> | <span data-ttu-id="eaead-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-142">Not supported</span></span> | <span data-ttu-id="eaead-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-143">Not supported</span></span> |
|[<span data-ttu-id="eaead-144">list</span><span class="sxs-lookup"><span data-stu-id="eaead-144">list</span></span>](../resources/list.md) | <span data-ttu-id="eaead-145">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaead-145">Sites.ReadWrite.All</span></span> | <span data-ttu-id="eaead-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-146">Not supported</span></span> | <span data-ttu-id="eaead-147">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaead-147">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="eaead-148">message</span><span class="sxs-lookup"><span data-stu-id="eaead-148">message</span></span>](../resources/message.md) | <span data-ttu-id="eaead-149">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-149">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="eaead-150">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-150">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="eaead-151">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="eaead-151">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="eaead-152">security alert</span><span class="sxs-lookup"><span data-stu-id="eaead-152">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="eaead-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaead-153">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="eaead-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eaead-154">Not supported</span></span> | <span data-ttu-id="eaead-155">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaead-155">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="eaead-156">user</span><span class="sxs-lookup"><span data-stu-id="eaead-156">user</span></span>](../resources/user.md) | <span data-ttu-id="eaead-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaead-157">User.Read.All</span></span> | <span data-ttu-id="eaead-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaead-158">User.Read.All</span></span> | <span data-ttu-id="eaead-159">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaead-159">User.Read.All</span></span> |

> <span data-ttu-id="eaead-160">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="eaead-160">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="eaead-161">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="eaead-161">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="eaead-162">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="eaead-162">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="eaead-163">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="eaead-163">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="eaead-164">Уведомления об изменениях отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="eaead-164">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="eaead-165">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="eaead-165">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="eaead-166">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="eaead-166">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="eaead-167">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="eaead-167">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="eaead-168">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="eaead-168">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="eaead-169">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="eaead-169">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="eaead-170">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="eaead-170">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="eaead-171">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaead-171">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eaead-172">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaead-172">Request headers</span></span>

| <span data-ttu-id="eaead-173">Имя</span><span class="sxs-lookup"><span data-stu-id="eaead-173">Name</span></span>       | <span data-ttu-id="eaead-174">Тип</span><span class="sxs-lookup"><span data-stu-id="eaead-174">Type</span></span> | <span data-ttu-id="eaead-175">Описание</span><span class="sxs-lookup"><span data-stu-id="eaead-175">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eaead-176">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaead-176">Authorization</span></span>  | <span data-ttu-id="eaead-177">string</span><span class="sxs-lookup"><span data-stu-id="eaead-177">string</span></span>  | <span data-ttu-id="eaead-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaead-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="eaead-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaead-180">Response</span></span>

<span data-ttu-id="eaead-181">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eaead-181">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="eaead-182">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="eaead-182">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="eaead-183">Пример</span><span class="sxs-lookup"><span data-stu-id="eaead-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eaead-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaead-184">Request</span></span>

<span data-ttu-id="eaead-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaead-185">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eaead-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="eaead-186">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eaead-187">C#</span><span class="sxs-lookup"><span data-stu-id="eaead-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eaead-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eaead-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eaead-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eaead-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eaead-190">Java</span><span class="sxs-lookup"><span data-stu-id="eaead-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eaead-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaead-191">Response</span></span>

<span data-ttu-id="eaead-192">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eaead-192">Here is an example of the response.</span></span>
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

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

