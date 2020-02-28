---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 7ff9d85f1befec3e96a76002a10788d7068bf8ab
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331299"
---
# <a name="delete-subscription"></a><span data-ttu-id="d3041-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="d3041-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3041-104">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="d3041-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3041-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3041-105">Permissions</span></span>

<span data-ttu-id="d3041-106">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d3041-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d3041-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3041-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3041-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="d3041-108">Supported resource</span></span> | <span data-ttu-id="d3041-109">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3041-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d3041-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3041-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3041-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3041-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="d3041-112">contact</span><span class="sxs-lookup"><span data-stu-id="d3041-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d3041-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-113">Contacts.Read</span></span> | <span data-ttu-id="d3041-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-114">Contacts.Read</span></span> | <span data-ttu-id="d3041-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-115">Contacts.Read</span></span> |
|<span data-ttu-id="d3041-116">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="d3041-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="d3041-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3041-117">Not supported</span></span> | <span data-ttu-id="d3041-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3041-118">Files.ReadWrite</span></span> | <span data-ttu-id="d3041-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3041-119">Not supported</span></span> |
|<span data-ttu-id="d3041-120">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="d3041-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="d3041-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3041-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="d3041-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3041-122">Not supported</span></span> | <span data-ttu-id="d3041-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3041-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="d3041-124">event</span><span class="sxs-lookup"><span data-stu-id="d3041-124">event</span></span>](../resources/event.md) | <span data-ttu-id="d3041-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-125">Calendars.Read</span></span> | <span data-ttu-id="d3041-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-126">Calendars.Read</span></span> | <span data-ttu-id="d3041-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-127">Calendars.Read</span></span> |
|[<span data-ttu-id="d3041-128">group</span><span class="sxs-lookup"><span data-stu-id="d3041-128">group</span></span>](../resources/group.md) | <span data-ttu-id="d3041-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3041-129">Group.Read.All</span></span> | <span data-ttu-id="d3041-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3041-130">Not supported</span></span> | <span data-ttu-id="d3041-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3041-131">Group.Read.All</span></span> |
|[<span data-ttu-id="d3041-132">group conversation</span><span class="sxs-lookup"><span data-stu-id="d3041-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="d3041-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3041-133">Group.Read.All</span></span> | <span data-ttu-id="d3041-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3041-134">Not supported</span></span> | <span data-ttu-id="d3041-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3041-135">Not supported</span></span> |
|[<span data-ttu-id="d3041-136">list</span><span class="sxs-lookup"><span data-stu-id="d3041-136">list</span></span>](../resources/list.md) | <span data-ttu-id="d3041-137">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3041-137">Sites.ReadWrite.All</span></span> | <span data-ttu-id="d3041-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3041-138">Not supported</span></span> | <span data-ttu-id="d3041-139">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3041-139">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="d3041-140">message</span><span class="sxs-lookup"><span data-stu-id="d3041-140">message</span></span>](../resources/message.md) | <span data-ttu-id="d3041-141">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-141">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d3041-142">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-142">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d3041-143">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d3041-143">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="d3041-144">security alert</span><span class="sxs-lookup"><span data-stu-id="d3041-144">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="d3041-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3041-145">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="d3041-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d3041-146">Not supported</span></span> | <span data-ttu-id="d3041-147">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3041-147">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="d3041-148">user</span><span class="sxs-lookup"><span data-stu-id="d3041-148">user</span></span>](../resources/user.md) | <span data-ttu-id="d3041-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3041-149">User.Read.All</span></span> | <span data-ttu-id="d3041-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3041-150">User.Read.All</span></span> | <span data-ttu-id="d3041-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3041-151">User.Read.All</span></span> |

> <span data-ttu-id="d3041-152">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="d3041-152">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="d3041-153">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="d3041-153">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="d3041-154">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="d3041-154">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="d3041-155">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="d3041-155">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="d3041-156">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="d3041-156">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="d3041-157">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="d3041-157">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="d3041-158">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="d3041-158">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="d3041-159">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3041-159">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="d3041-160">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="d3041-160">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="d3041-161">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d3041-161">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="d3041-162">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="d3041-162">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="d3041-163">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3041-163">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d3041-164">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3041-164">Request headers</span></span>

| <span data-ttu-id="d3041-165">Имя</span><span class="sxs-lookup"><span data-stu-id="d3041-165">Name</span></span>       | <span data-ttu-id="d3041-166">Тип</span><span class="sxs-lookup"><span data-stu-id="d3041-166">Type</span></span> | <span data-ttu-id="d3041-167">Описание</span><span class="sxs-lookup"><span data-stu-id="d3041-167">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d3041-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3041-168">Authorization</span></span>  | <span data-ttu-id="d3041-169">string</span><span class="sxs-lookup"><span data-stu-id="d3041-169">string</span></span>  | <span data-ttu-id="d3041-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3041-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3041-172">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3041-172">Request body</span></span>

<span data-ttu-id="d3041-173">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3041-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3041-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3041-174">Response</span></span>

<span data-ttu-id="d3041-175">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d3041-175">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d3041-176">Пример</span><span class="sxs-lookup"><span data-stu-id="d3041-176">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d3041-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3041-177">Request</span></span>

<span data-ttu-id="d3041-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3041-178">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3041-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3041-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="d3041-180">C#</span><span class="sxs-lookup"><span data-stu-id="d3041-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3041-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3041-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3041-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3041-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d3041-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3041-183">Response</span></span>

<span data-ttu-id="d3041-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3041-184">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
