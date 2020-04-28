---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 94553470bb19bfaccd1824631d183bb931ab0ea8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453116"
---
# <a name="delete-subscription"></a><span data-ttu-id="af006-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="af006-103">Delete subscription</span></span>

<span data-ttu-id="af006-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af006-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af006-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="af006-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="af006-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af006-106">Permissions</span></span>

<span data-ttu-id="af006-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="af006-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="af006-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af006-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="af006-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="af006-109">Supported resource</span></span> | <span data-ttu-id="af006-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af006-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af006-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af006-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af006-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af006-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="af006-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="af006-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="af006-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-114">Not supported</span></span> | <span data-ttu-id="af006-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-115">Not supported</span></span> | <span data-ttu-id="af006-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="af006-116">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="af006-117">contact</span><span class="sxs-lookup"><span data-stu-id="af006-117">contact</span></span>](../resources/contact.md) | <span data-ttu-id="af006-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="af006-118">Contacts.Read</span></span> | <span data-ttu-id="af006-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="af006-119">Contacts.Read</span></span> | <span data-ttu-id="af006-120">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="af006-120">Contacts.Read</span></span> |
|<span data-ttu-id="af006-121">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="af006-121">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="af006-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-122">Not supported</span></span> | <span data-ttu-id="af006-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af006-123">Files.ReadWrite</span></span> | <span data-ttu-id="af006-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-124">Not supported</span></span> |
|<span data-ttu-id="af006-125">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="af006-125">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="af006-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af006-126">Files.ReadWrite.All</span></span> | <span data-ttu-id="af006-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-127">Not supported</span></span> | <span data-ttu-id="af006-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af006-128">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="af006-129">event</span><span class="sxs-lookup"><span data-stu-id="af006-129">event</span></span>](../resources/event.md) | <span data-ttu-id="af006-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="af006-130">Calendars.Read</span></span> | <span data-ttu-id="af006-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="af006-131">Calendars.Read</span></span> | <span data-ttu-id="af006-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="af006-132">Calendars.Read</span></span> |
|[<span data-ttu-id="af006-133">group</span><span class="sxs-lookup"><span data-stu-id="af006-133">group</span></span>](../resources/group.md) | <span data-ttu-id="af006-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="af006-134">Group.Read.All</span></span> | <span data-ttu-id="af006-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-135">Not supported</span></span> | <span data-ttu-id="af006-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="af006-136">Group.Read.All</span></span> |
|[<span data-ttu-id="af006-137">group conversation</span><span class="sxs-lookup"><span data-stu-id="af006-137">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="af006-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="af006-138">Group.Read.All</span></span> | <span data-ttu-id="af006-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-139">Not supported</span></span> | <span data-ttu-id="af006-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-140">Not supported</span></span> |
|[<span data-ttu-id="af006-141">list</span><span class="sxs-lookup"><span data-stu-id="af006-141">list</span></span>](../resources/list.md) | <span data-ttu-id="af006-142">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af006-142">Sites.ReadWrite.All</span></span> | <span data-ttu-id="af006-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-143">Not supported</span></span> | <span data-ttu-id="af006-144">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af006-144">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="af006-145">message</span><span class="sxs-lookup"><span data-stu-id="af006-145">message</span></span>](../resources/message.md) | <span data-ttu-id="af006-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="af006-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="af006-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="af006-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="af006-148">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="af006-148">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="af006-149">security alert</span><span class="sxs-lookup"><span data-stu-id="af006-149">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="af006-150">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af006-150">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="af006-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="af006-151">Not supported</span></span> | <span data-ttu-id="af006-152">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af006-152">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="af006-153">user</span><span class="sxs-lookup"><span data-stu-id="af006-153">user</span></span>](../resources/user.md) | <span data-ttu-id="af006-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="af006-154">User.Read.All</span></span> | <span data-ttu-id="af006-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="af006-155">User.Read.All</span></span> | <span data-ttu-id="af006-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="af006-156">User.Read.All</span></span> |

> <span data-ttu-id="af006-157">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="af006-157">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="af006-158">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="af006-158">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="af006-159">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="af006-159">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="af006-160">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="af006-160">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="af006-161">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="af006-161">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="af006-162">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="af006-162">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="af006-163">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="af006-163">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="af006-164">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="af006-164">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="af006-165">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="af006-165">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="af006-166">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="af006-166">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="af006-167">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="af006-167">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="af006-168">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af006-168">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="af006-169">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af006-169">Request headers</span></span>

| <span data-ttu-id="af006-170">Имя</span><span class="sxs-lookup"><span data-stu-id="af006-170">Name</span></span>       | <span data-ttu-id="af006-171">Тип</span><span class="sxs-lookup"><span data-stu-id="af006-171">Type</span></span> | <span data-ttu-id="af006-172">Описание</span><span class="sxs-lookup"><span data-stu-id="af006-172">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af006-173">Authorization</span><span class="sxs-lookup"><span data-stu-id="af006-173">Authorization</span></span>  | <span data-ttu-id="af006-174">string</span><span class="sxs-lookup"><span data-stu-id="af006-174">string</span></span>  | <span data-ttu-id="af006-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af006-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af006-177">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af006-177">Request body</span></span>

<span data-ttu-id="af006-178">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af006-178">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af006-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="af006-179">Response</span></span>

<span data-ttu-id="af006-180">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="af006-180">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="af006-181">Пример</span><span class="sxs-lookup"><span data-stu-id="af006-181">Example</span></span>

##### <a name="request"></a><span data-ttu-id="af006-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="af006-182">Request</span></span>

<span data-ttu-id="af006-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af006-183">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af006-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="af006-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="af006-185">C#</span><span class="sxs-lookup"><span data-stu-id="af006-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af006-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af006-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af006-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af006-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="af006-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="af006-188">Response</span></span>

<span data-ttu-id="af006-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af006-189">Here is an example of the response.</span></span>
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
