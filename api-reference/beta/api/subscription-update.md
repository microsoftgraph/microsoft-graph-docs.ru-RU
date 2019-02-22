---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: e868489ca5eb95cdc2ee8c33176c8da20271bd12
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159537"
---
# <a name="update-subscription"></a><span data-ttu-id="232e4-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="232e4-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="232e4-104">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="232e4-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="232e4-105">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="232e4-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="232e4-106">Чтобы избежать отсутствия уведомлений, приложение должно хорошо обновлять свои подписки в течение срока их действия.</span><span class="sxs-lookup"><span data-stu-id="232e4-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="232e4-107">В [](../resources/subscription.md) этой статье приведены сведения о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="232e4-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="232e4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="232e4-108">Permissions</span></span>

<span data-ttu-id="232e4-109">В зависимости от ресурса и запрашиваемого типа разрешения (делегированного или приложения) разрешение, указанное в следующей таблице, является минимальным привилегированным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="232e4-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="232e4-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="232e4-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="232e4-111">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="232e4-111">Supported resource</span></span> | <span data-ttu-id="232e4-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="232e4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="232e4-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="232e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="232e4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="232e4-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="232e4-115">contact</span><span class="sxs-lookup"><span data-stu-id="232e4-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="232e4-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-116">Contacts.Read</span></span> | <span data-ttu-id="232e4-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-117">Contacts.Read</span></span> | <span data-ttu-id="232e4-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-118">Contacts.Read</span></span> |
|<span data-ttu-id="232e4-119">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="232e4-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="232e4-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="232e4-120">Not supported</span></span> | <span data-ttu-id="232e4-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="232e4-121">Files.ReadWrite</span></span> | <span data-ttu-id="232e4-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="232e4-122">Not supported</span></span> |
|<span data-ttu-id="232e4-123">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="232e4-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="232e4-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="232e4-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="232e4-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="232e4-125">Not supported</span></span> | <span data-ttu-id="232e4-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="232e4-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="232e4-127">event</span><span class="sxs-lookup"><span data-stu-id="232e4-127">event</span></span>](../resources/event.md) | <span data-ttu-id="232e4-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-128">Calendars.Read</span></span> | <span data-ttu-id="232e4-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-129">Calendars.Read</span></span> | <span data-ttu-id="232e4-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-130">Calendars.Read</span></span> |
|[<span data-ttu-id="232e4-131">group</span><span class="sxs-lookup"><span data-stu-id="232e4-131">group</span></span>](../resources/group.md) | <span data-ttu-id="232e4-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="232e4-132">Group.Read.All</span></span> | <span data-ttu-id="232e4-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="232e4-133">Not supported</span></span> | <span data-ttu-id="232e4-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="232e4-134">Group.Read.All</span></span> |
|[<span data-ttu-id="232e4-135">Групповая беседа</span><span class="sxs-lookup"><span data-stu-id="232e4-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="232e4-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="232e4-136">Group.Read.All</span></span> | <span data-ttu-id="232e4-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="232e4-137">Not supported</span></span> | <span data-ttu-id="232e4-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="232e4-138">Not supported</span></span> |
|[<span data-ttu-id="232e4-139">message</span><span class="sxs-lookup"><span data-stu-id="232e4-139">message</span></span>](../resources/message.md) | <span data-ttu-id="232e4-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-140">Mail.Read</span></span> | <span data-ttu-id="232e4-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-141">Mail.Read</span></span> | <span data-ttu-id="232e4-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="232e4-142">Mail.Read</span></span> |
|[<span data-ttu-id="232e4-143">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="232e4-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="232e4-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="232e4-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="232e4-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="232e4-145">Not supported</span></span> | <span data-ttu-id="232e4-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="232e4-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="232e4-147">user</span><span class="sxs-lookup"><span data-stu-id="232e4-147">user</span></span>](../resources/user.md) | <span data-ttu-id="232e4-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="232e4-148">User.Read.All</span></span> | <span data-ttu-id="232e4-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="232e4-149">User.Read.All</span></span> | <span data-ttu-id="232e4-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="232e4-150">User.Read.All</span></span> |

> <span data-ttu-id="232e4-151">**Примечание:** Существуют дополнительные ограничения для подписок на OneDrive и элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="232e4-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="232e4-152">Ограничения применяются к созданию и управлению подписками (процессами, обновлением и удалением подписок).</span><span class="sxs-lookup"><span data-stu-id="232e4-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="232e4-153">В личном OneDrive вы можете подписаться на корневую папку или любую подпапку на этом диске.</span><span class="sxs-lookup"><span data-stu-id="232e4-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="232e4-154">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="232e4-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="232e4-155">Уведомления отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других объектов driveItem в иерархии.</span><span class="sxs-lookup"><span data-stu-id="232e4-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="232e4-156">Вы не можете подписаться на **диски** или экземпляры **driveItem** , которые не являются папками, например отдельными файлами.</span><span class="sxs-lookup"><span data-stu-id="232e4-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="232e4-157">Делегированное разрешение в Outlook поддерживает подписку на элементы в папках только в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="232e4-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="232e4-158">Это означает, например, вы не можете использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="232e4-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="232e4-159">Чтобы подписаться на уведомления об изменении контактов, событий или сообщений Outlook в _общих или делегированных_ папках, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="232e4-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="232e4-160">Используйте соответствующее разрешение приложения, чтобы подписаться на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="232e4-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="232e4-161">Не используйте разрешения на общий доступ к Outlook (Contacts. Read. Shared, Calendars. Read. Shared, mail. Read. Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменении элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="232e4-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="232e4-162">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="232e4-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="232e4-163">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="232e4-163">Request headers</span></span>

| <span data-ttu-id="232e4-164">Имя</span><span class="sxs-lookup"><span data-stu-id="232e4-164">Name</span></span>       | <span data-ttu-id="232e4-165">Тип</span><span class="sxs-lookup"><span data-stu-id="232e4-165">Type</span></span> | <span data-ttu-id="232e4-166">Описание</span><span class="sxs-lookup"><span data-stu-id="232e4-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="232e4-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="232e4-167">Authorization</span></span>  | <span data-ttu-id="232e4-168">string</span><span class="sxs-lookup"><span data-stu-id="232e4-168">string</span></span>  | <span data-ttu-id="232e4-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="232e4-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="232e4-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="232e4-171">Response</span></span>

<span data-ttu-id="232e4-172">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="232e4-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="232e4-173">Пример</span><span class="sxs-lookup"><span data-stu-id="232e4-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="232e4-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="232e4-174">Request</span></span>

<span data-ttu-id="232e4-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="232e4-175">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="232e4-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="232e4-176">Response</span></span>

<span data-ttu-id="232e4-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="232e4-177">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/subscription-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
