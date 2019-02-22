---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c73f01a65a2b81bfa34818f9a7a96f754501bd65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163471"
---
# <a name="get-subscription"></a><span data-ttu-id="fd0a1-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="fd0a1-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd0a1-104">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd0a1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd0a1-105">Permissions</span></span>

<span data-ttu-id="fd0a1-106">В зависимости от ресурса и запрашиваемого типа разрешения (делегированного или приложения) разрешение, указанное в следующей таблице, является минимальным привилегированным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="fd0a1-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd0a1-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd0a1-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="fd0a1-108">Supported resource</span></span> | <span data-ttu-id="fd0a1-109">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd0a1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fd0a1-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd0a1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd0a1-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd0a1-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="fd0a1-112">contact</span><span class="sxs-lookup"><span data-stu-id="fd0a1-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="fd0a1-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-113">Contacts.Read</span></span> | <span data-ttu-id="fd0a1-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-114">Contacts.Read</span></span> | <span data-ttu-id="fd0a1-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-115">Contacts.Read</span></span> |
|<span data-ttu-id="fd0a1-116">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="fd0a1-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="fd0a1-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd0a1-117">Not supported</span></span> | <span data-ttu-id="fd0a1-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd0a1-118">Files.ReadWrite</span></span> | <span data-ttu-id="fd0a1-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd0a1-119">Not supported</span></span> |
|<span data-ttu-id="fd0a1-120">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="fd0a1-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="fd0a1-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="fd0a1-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd0a1-122">Not supported</span></span> | <span data-ttu-id="fd0a1-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="fd0a1-124">event</span><span class="sxs-lookup"><span data-stu-id="fd0a1-124">event</span></span>](../resources/event.md) | <span data-ttu-id="fd0a1-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-125">Calendars.Read</span></span> | <span data-ttu-id="fd0a1-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-126">Calendars.Read</span></span> | <span data-ttu-id="fd0a1-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-127">Calendars.Read</span></span> |
|[<span data-ttu-id="fd0a1-128">group</span><span class="sxs-lookup"><span data-stu-id="fd0a1-128">group</span></span>](../resources/group.md) | <span data-ttu-id="fd0a1-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-129">Group.Read.All</span></span> | <span data-ttu-id="fd0a1-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd0a1-130">Not supported</span></span> | <span data-ttu-id="fd0a1-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-131">Group.Read.All</span></span> |
|[<span data-ttu-id="fd0a1-132">Групповая беседа</span><span class="sxs-lookup"><span data-stu-id="fd0a1-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="fd0a1-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-133">Group.Read.All</span></span> | <span data-ttu-id="fd0a1-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd0a1-134">Not supported</span></span> | <span data-ttu-id="fd0a1-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd0a1-135">Not supported</span></span> |
|[<span data-ttu-id="fd0a1-136">message</span><span class="sxs-lookup"><span data-stu-id="fd0a1-136">message</span></span>](../resources/message.md) | <span data-ttu-id="fd0a1-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-137">Mail.Read</span></span> | <span data-ttu-id="fd0a1-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-138">Mail.Read</span></span> | <span data-ttu-id="fd0a1-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fd0a1-139">Mail.Read</span></span> |
|[<span data-ttu-id="fd0a1-140">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="fd0a1-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="fd0a1-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="fd0a1-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd0a1-142">Not supported</span></span> | <span data-ttu-id="fd0a1-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="fd0a1-144">user</span><span class="sxs-lookup"><span data-stu-id="fd0a1-144">user</span></span>](../resources/user.md) | <span data-ttu-id="fd0a1-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-145">User.Read.All</span></span> | <span data-ttu-id="fd0a1-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-146">User.Read.All</span></span> | <span data-ttu-id="fd0a1-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd0a1-147">User.Read.All</span></span> |

> <span data-ttu-id="fd0a1-148">**Примечание:** Существуют дополнительные ограничения для подписок на OneDrive и элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="fd0a1-149">Ограничения применяются к созданию и управлению подписками (процессами, обновлением и удалением подписок).</span><span class="sxs-lookup"><span data-stu-id="fd0a1-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="fd0a1-150">В личном OneDrive вы можете подписаться на корневую папку или любую подпапку на этом диске.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="fd0a1-151">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="fd0a1-152">Уведомления отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других объектов driveItem в иерархии.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="fd0a1-153">Вы не можете подписаться на **диски** или экземпляры **driveItem** , которые не являются папками, например отдельными файлами.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="fd0a1-154">Делегированное разрешение в Outlook поддерживает подписку на элементы в папках только в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="fd0a1-155">Это означает, например, вы не можете использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="fd0a1-156">Чтобы подписаться на уведомления об изменении контактов, событий или сообщений Outlook в _общих или делегированных_ папках, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="fd0a1-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="fd0a1-157">Используйте соответствующее разрешение приложения, чтобы подписаться на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="fd0a1-158">Не используйте разрешения на общий доступ к Outlook (Contacts. Read. Shared, Calendars. Read. Shared, mail. Read. Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменении элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd0a1-159">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd0a1-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd0a1-160">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fd0a1-160">Optional query parameters</span></span>

<span data-ttu-id="fd0a1-161">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd0a1-162">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd0a1-162">Request headers</span></span>

| <span data-ttu-id="fd0a1-163">Имя</span><span class="sxs-lookup"><span data-stu-id="fd0a1-163">Name</span></span>       | <span data-ttu-id="fd0a1-164">Тип</span><span class="sxs-lookup"><span data-stu-id="fd0a1-164">Type</span></span> | <span data-ttu-id="fd0a1-165">Описание</span><span class="sxs-lookup"><span data-stu-id="fd0a1-165">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="fd0a1-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd0a1-166">Authorization</span></span>  | <span data-ttu-id="fd0a1-167">string</span><span class="sxs-lookup"><span data-stu-id="fd0a1-167">string</span></span>  | <span data-ttu-id="fd0a1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd0a1-170">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd0a1-170">Request body</span></span>

<span data-ttu-id="fd0a1-171">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd0a1-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd0a1-172">Response</span></span>

<span data-ttu-id="fd0a1-173">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd0a1-174">Пример</span><span class="sxs-lookup"><span data-stu-id="fd0a1-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fd0a1-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd0a1-175">Request</span></span>

<span data-ttu-id="fd0a1-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="fd0a1-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd0a1-177">Response</span></span>

<span data-ttu-id="fd0a1-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd0a1-178">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
