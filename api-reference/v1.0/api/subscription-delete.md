---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 50cd70ed1284b9ea165118db6af3141a6dadec6a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459890"
---
# <a name="delete-subscription"></a><span data-ttu-id="4956d-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="4956d-103">Delete subscription</span></span>

<span data-ttu-id="4956d-104">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="4956d-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="4956d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4956d-105">Permissions</span></span>

<span data-ttu-id="4956d-106">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4956d-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4956d-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4956d-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4956d-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="4956d-108">Supported resource</span></span> | <span data-ttu-id="4956d-109">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4956d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4956d-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4956d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4956d-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4956d-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="4956d-112">contact</span><span class="sxs-lookup"><span data-stu-id="4956d-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="4956d-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-113">Contacts.Read</span></span> | <span data-ttu-id="4956d-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-114">Contacts.Read</span></span> | <span data-ttu-id="4956d-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-115">Contacts.Read</span></span> |
|<span data-ttu-id="4956d-116">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="4956d-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="4956d-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4956d-117">Not supported</span></span> | <span data-ttu-id="4956d-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4956d-118">Files.ReadWrite</span></span> | <span data-ttu-id="4956d-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4956d-119">Not supported</span></span> |
|<span data-ttu-id="4956d-120">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="4956d-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="4956d-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4956d-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="4956d-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4956d-122">Not supported</span></span> | <span data-ttu-id="4956d-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4956d-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="4956d-124">event</span><span class="sxs-lookup"><span data-stu-id="4956d-124">event</span></span>](../resources/event.md) | <span data-ttu-id="4956d-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-125">Calendars.Read</span></span> | <span data-ttu-id="4956d-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-126">Calendars.Read</span></span> | <span data-ttu-id="4956d-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-127">Calendars.Read</span></span> |
|[<span data-ttu-id="4956d-128">group</span><span class="sxs-lookup"><span data-stu-id="4956d-128">group</span></span>](../resources/group.md) | <span data-ttu-id="4956d-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4956d-129">Group.Read.All</span></span> | <span data-ttu-id="4956d-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4956d-130">Not supported</span></span> | <span data-ttu-id="4956d-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4956d-131">Group.Read.All</span></span> |
|[<span data-ttu-id="4956d-132">group conversation</span><span class="sxs-lookup"><span data-stu-id="4956d-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="4956d-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4956d-133">Group.Read.All</span></span> | <span data-ttu-id="4956d-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4956d-134">Not supported</span></span> | <span data-ttu-id="4956d-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4956d-135">Not supported</span></span> |
|[<span data-ttu-id="4956d-136">message</span><span class="sxs-lookup"><span data-stu-id="4956d-136">message</span></span>](../resources/message.md) | <span data-ttu-id="4956d-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-137">Mail.Read</span></span> | <span data-ttu-id="4956d-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-138">Mail.Read</span></span> | <span data-ttu-id="4956d-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4956d-139">Mail.Read</span></span> |
|[<span data-ttu-id="4956d-140">security alert</span><span class="sxs-lookup"><span data-stu-id="4956d-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="4956d-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4956d-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="4956d-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4956d-142">Not supported</span></span> | <span data-ttu-id="4956d-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4956d-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="4956d-144">user</span><span class="sxs-lookup"><span data-stu-id="4956d-144">user</span></span>](../resources/user.md) | <span data-ttu-id="4956d-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4956d-145">User.Read.All</span></span> | <span data-ttu-id="4956d-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4956d-146">User.Read.All</span></span> | <span data-ttu-id="4956d-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4956d-147">User.Read.All</span></span> |

> <span data-ttu-id="4956d-148">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="4956d-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="4956d-149">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="4956d-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="4956d-150">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="4956d-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="4956d-151">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="4956d-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="4956d-152">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="4956d-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="4956d-153">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="4956d-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="4956d-154">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="4956d-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="4956d-155">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4956d-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="4956d-156">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="4956d-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="4956d-157">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="4956d-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="4956d-158">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="4956d-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="4956d-159">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4956d-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4956d-160">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4956d-160">Request headers</span></span>

| <span data-ttu-id="4956d-161">Имя</span><span class="sxs-lookup"><span data-stu-id="4956d-161">Name</span></span>       | <span data-ttu-id="4956d-162">Тип</span><span class="sxs-lookup"><span data-stu-id="4956d-162">Type</span></span> | <span data-ttu-id="4956d-163">Описание</span><span class="sxs-lookup"><span data-stu-id="4956d-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4956d-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="4956d-164">Authorization</span></span>  | <span data-ttu-id="4956d-165">string</span><span class="sxs-lookup"><span data-stu-id="4956d-165">string</span></span>  | <span data-ttu-id="4956d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4956d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4956d-168">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4956d-168">Request body</span></span>

<span data-ttu-id="4956d-169">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4956d-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4956d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="4956d-170">Response</span></span>

<span data-ttu-id="4956d-171">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4956d-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4956d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="4956d-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4956d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="4956d-173">Request</span></span>

<span data-ttu-id="4956d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4956d-174">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4956d-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="4956d-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4956d-176">C#</span><span class="sxs-lookup"><span data-stu-id="4956d-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4956d-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="4956d-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4956d-178">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4956d-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4956d-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="4956d-179">Response</span></span>

<span data-ttu-id="4956d-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4956d-180">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
