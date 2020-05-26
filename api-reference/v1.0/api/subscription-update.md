---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 1278c6f61ddb62165ef125acc810d5ae6dde0454
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353170"
---
# <a name="update-subscription"></a><span data-ttu-id="1afd2-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="1afd2-103">Update subscription</span></span>

<span data-ttu-id="1afd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1afd2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1afd2-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="1afd2-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="1afd2-106">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="1afd2-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="1afd2-107">Чтобы избежать отсутствия уведомлений об изменениях, приложение должно правильно обновить свои подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="1afd2-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="1afd2-108">В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1afd2-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="1afd2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1afd2-109">Permissions</span></span>

<span data-ttu-id="1afd2-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1afd2-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="1afd2-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1afd2-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1afd2-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="1afd2-112">Supported resource</span></span> | <span data-ttu-id="1afd2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1afd2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1afd2-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1afd2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1afd2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1afd2-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="1afd2-116">contact</span><span class="sxs-lookup"><span data-stu-id="1afd2-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="1afd2-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-117">Contacts.Read</span></span> | <span data-ttu-id="1afd2-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-118">Contacts.Read</span></span> | <span data-ttu-id="1afd2-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-119">Contacts.Read</span></span> |
|<span data-ttu-id="1afd2-120">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="1afd2-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="1afd2-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1afd2-121">Not supported</span></span> | <span data-ttu-id="1afd2-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1afd2-122">Files.ReadWrite</span></span> | <span data-ttu-id="1afd2-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1afd2-123">Not supported</span></span> |
|<span data-ttu-id="1afd2-124">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="1afd2-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="1afd2-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="1afd2-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1afd2-126">Not supported</span></span> | <span data-ttu-id="1afd2-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="1afd2-128">event</span><span class="sxs-lookup"><span data-stu-id="1afd2-128">event</span></span>](../resources/event.md) | <span data-ttu-id="1afd2-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-129">Calendars.Read</span></span> | <span data-ttu-id="1afd2-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-130">Calendars.Read</span></span> | <span data-ttu-id="1afd2-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-131">Calendars.Read</span></span> |
|[<span data-ttu-id="1afd2-132">group</span><span class="sxs-lookup"><span data-stu-id="1afd2-132">group</span></span>](../resources/group.md) | <span data-ttu-id="1afd2-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-133">Group.Read.All</span></span> | <span data-ttu-id="1afd2-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1afd2-134">Not supported</span></span> | <span data-ttu-id="1afd2-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-135">Group.Read.All</span></span> |
|[<span data-ttu-id="1afd2-136">group conversation</span><span class="sxs-lookup"><span data-stu-id="1afd2-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="1afd2-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-137">Group.Read.All</span></span> | <span data-ttu-id="1afd2-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1afd2-138">Not supported</span></span> | <span data-ttu-id="1afd2-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1afd2-139">Not supported</span></span> |
|[<span data-ttu-id="1afd2-140">list</span><span class="sxs-lookup"><span data-stu-id="1afd2-140">list</span></span>](../resources/list.md) | <span data-ttu-id="1afd2-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="1afd2-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1afd2-142">Not supported</span></span> | <span data-ttu-id="1afd2-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="1afd2-144">message</span><span class="sxs-lookup"><span data-stu-id="1afd2-144">message</span></span>](../resources/message.md) | <span data-ttu-id="1afd2-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1afd2-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1afd2-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1afd2-147">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="1afd2-148">security alert</span><span class="sxs-lookup"><span data-stu-id="1afd2-148">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="1afd2-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="1afd2-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1afd2-150">Not supported</span></span> | <span data-ttu-id="1afd2-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="1afd2-152">user</span><span class="sxs-lookup"><span data-stu-id="1afd2-152">user</span></span>](../resources/user.md) | <span data-ttu-id="1afd2-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-153">User.Read.All</span></span> | <span data-ttu-id="1afd2-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-154">User.Read.All</span></span> | <span data-ttu-id="1afd2-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1afd2-155">User.Read.All</span></span> |

> <span data-ttu-id="1afd2-156">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="1afd2-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="1afd2-157">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="1afd2-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="1afd2-158">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="1afd2-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="1afd2-159">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="1afd2-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="1afd2-160">Уведомления об изменениях отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других объектов driveItem в иерархии.</span><span class="sxs-lookup"><span data-stu-id="1afd2-160">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="1afd2-161">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="1afd2-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="1afd2-162">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="1afd2-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="1afd2-163">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1afd2-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="1afd2-164">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="1afd2-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="1afd2-165">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1afd2-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="1afd2-166">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="1afd2-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="1afd2-167">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1afd2-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1afd2-168">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1afd2-168">Request headers</span></span>

| <span data-ttu-id="1afd2-169">Имя</span><span class="sxs-lookup"><span data-stu-id="1afd2-169">Name</span></span>       | <span data-ttu-id="1afd2-170">Тип</span><span class="sxs-lookup"><span data-stu-id="1afd2-170">Type</span></span> | <span data-ttu-id="1afd2-171">Описание</span><span class="sxs-lookup"><span data-stu-id="1afd2-171">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1afd2-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="1afd2-172">Authorization</span></span>  | <span data-ttu-id="1afd2-173">string</span><span class="sxs-lookup"><span data-stu-id="1afd2-173">string</span></span>  | <span data-ttu-id="1afd2-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1afd2-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1afd2-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="1afd2-176">Response</span></span>

<span data-ttu-id="1afd2-177">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1afd2-177">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="1afd2-178">Сведения о том, как возвращаются ошибки, приведены в разделе [ошибочные ответы][error-response].</span><span class="sxs-lookup"><span data-stu-id="1afd2-178">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="1afd2-179">Пример</span><span class="sxs-lookup"><span data-stu-id="1afd2-179">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1afd2-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="1afd2-180">Request</span></span>

<span data-ttu-id="1afd2-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1afd2-181">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1afd2-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="1afd2-182">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1afd2-183">C#</span><span class="sxs-lookup"><span data-stu-id="1afd2-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1afd2-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1afd2-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1afd2-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1afd2-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1afd2-186">Java</span><span class="sxs-lookup"><span data-stu-id="1afd2-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1afd2-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="1afd2-187">Response</span></span>

<span data-ttu-id="1afd2-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1afd2-188">Here is an example of the response.</span></span>
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
