---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b74046ae383f6744f13b4309884557a4d38db2be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509754"
---
# <a name="delete-subscription"></a><span data-ttu-id="a433e-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="a433e-103">Delete subscription</span></span>

<span data-ttu-id="a433e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a433e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a433e-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="a433e-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="a433e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a433e-106">Permissions</span></span>

<span data-ttu-id="a433e-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a433e-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a433e-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a433e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a433e-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="a433e-109">Supported resource</span></span> | <span data-ttu-id="a433e-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a433e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a433e-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a433e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a433e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a433e-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="a433e-113">contact</span><span class="sxs-lookup"><span data-stu-id="a433e-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a433e-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-114">Contacts.Read</span></span> | <span data-ttu-id="a433e-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-115">Contacts.Read</span></span> | <span data-ttu-id="a433e-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-116">Contacts.Read</span></span> |
|<span data-ttu-id="a433e-117">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="a433e-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a433e-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a433e-118">Not supported</span></span> | <span data-ttu-id="a433e-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a433e-119">Files.ReadWrite</span></span> | <span data-ttu-id="a433e-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a433e-120">Not supported</span></span> |
|<span data-ttu-id="a433e-121">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="a433e-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a433e-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a433e-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="a433e-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a433e-123">Not supported</span></span> | <span data-ttu-id="a433e-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a433e-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a433e-125">event</span><span class="sxs-lookup"><span data-stu-id="a433e-125">event</span></span>](../resources/event.md) | <span data-ttu-id="a433e-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-126">Calendars.Read</span></span> | <span data-ttu-id="a433e-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-127">Calendars.Read</span></span> | <span data-ttu-id="a433e-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-128">Calendars.Read</span></span> |
|[<span data-ttu-id="a433e-129">group</span><span class="sxs-lookup"><span data-stu-id="a433e-129">group</span></span>](../resources/group.md) | <span data-ttu-id="a433e-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a433e-130">Group.Read.All</span></span> | <span data-ttu-id="a433e-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a433e-131">Not supported</span></span> | <span data-ttu-id="a433e-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a433e-132">Group.Read.All</span></span> |
|[<span data-ttu-id="a433e-133">group conversation</span><span class="sxs-lookup"><span data-stu-id="a433e-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a433e-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a433e-134">Group.Read.All</span></span> | <span data-ttu-id="a433e-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a433e-135">Not supported</span></span> | <span data-ttu-id="a433e-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a433e-136">Not supported</span></span> |
|[<span data-ttu-id="a433e-137">message</span><span class="sxs-lookup"><span data-stu-id="a433e-137">message</span></span>](../resources/message.md) | <span data-ttu-id="a433e-138">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-138">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a433e-139">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-139">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a433e-140">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a433e-140">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="a433e-141">security alert</span><span class="sxs-lookup"><span data-stu-id="a433e-141">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="a433e-142">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a433e-142">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a433e-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a433e-143">Not supported</span></span> | <span data-ttu-id="a433e-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a433e-144">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="a433e-145">user</span><span class="sxs-lookup"><span data-stu-id="a433e-145">user</span></span>](../resources/user.md) | <span data-ttu-id="a433e-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a433e-146">User.Read.All</span></span> | <span data-ttu-id="a433e-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a433e-147">User.Read.All</span></span> | <span data-ttu-id="a433e-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a433e-148">User.Read.All</span></span> |

> <span data-ttu-id="a433e-149">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="a433e-149">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="a433e-150">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="a433e-150">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="a433e-151">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="a433e-151">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a433e-152">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="a433e-152">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a433e-153">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="a433e-153">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="a433e-154">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="a433e-154">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="a433e-155">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="a433e-155">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a433e-156">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a433e-156">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="a433e-157">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="a433e-157">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a433e-158">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a433e-158">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a433e-159">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="a433e-159">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="a433e-160">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a433e-160">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a433e-161">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a433e-161">Request headers</span></span>

| <span data-ttu-id="a433e-162">Имя</span><span class="sxs-lookup"><span data-stu-id="a433e-162">Name</span></span>       | <span data-ttu-id="a433e-163">Тип</span><span class="sxs-lookup"><span data-stu-id="a433e-163">Type</span></span> | <span data-ttu-id="a433e-164">Описание</span><span class="sxs-lookup"><span data-stu-id="a433e-164">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a433e-165">Authorization</span><span class="sxs-lookup"><span data-stu-id="a433e-165">Authorization</span></span>  | <span data-ttu-id="a433e-166">string</span><span class="sxs-lookup"><span data-stu-id="a433e-166">string</span></span>  | <span data-ttu-id="a433e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a433e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a433e-169">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a433e-169">Request body</span></span>

<span data-ttu-id="a433e-170">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a433e-170">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a433e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="a433e-171">Response</span></span>

<span data-ttu-id="a433e-172">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a433e-172">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a433e-173">Пример</span><span class="sxs-lookup"><span data-stu-id="a433e-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a433e-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="a433e-174">Request</span></span>

<span data-ttu-id="a433e-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a433e-175">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a433e-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="a433e-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="a433e-177">C#</span><span class="sxs-lookup"><span data-stu-id="a433e-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a433e-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a433e-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a433e-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a433e-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a433e-180">Java</span><span class="sxs-lookup"><span data-stu-id="a433e-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a433e-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="a433e-181">Response</span></span>

<span data-ttu-id="a433e-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a433e-182">Here is an example of the response.</span></span>
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
