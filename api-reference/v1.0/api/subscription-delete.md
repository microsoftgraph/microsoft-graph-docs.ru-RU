---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f1f0dc151748d1f61f002f94243c13ce0f81c94b
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353179"
---
# <a name="delete-subscription"></a><span data-ttu-id="b5d51-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="b5d51-103">Delete subscription</span></span>

<span data-ttu-id="b5d51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5d51-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5d51-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="b5d51-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5d51-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5d51-106">Permissions</span></span>

<span data-ttu-id="b5d51-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b5d51-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b5d51-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5d51-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5d51-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="b5d51-109">Supported resource</span></span> | <span data-ttu-id="b5d51-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5d51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5d51-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5d51-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5d51-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5d51-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="b5d51-113">contact</span><span class="sxs-lookup"><span data-stu-id="b5d51-113">contact</span></span>](../resources/contact.md) | <span data-ttu-id="b5d51-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-114">Contacts.Read</span></span> | <span data-ttu-id="b5d51-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-115">Contacts.Read</span></span> | <span data-ttu-id="b5d51-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-116">Contacts.Read</span></span> |
|<span data-ttu-id="b5d51-117">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="b5d51-117">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="b5d51-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5d51-118">Not supported</span></span> | <span data-ttu-id="b5d51-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5d51-119">Files.ReadWrite</span></span> | <span data-ttu-id="b5d51-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5d51-120">Not supported</span></span> |
|<span data-ttu-id="b5d51-121">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="b5d51-121">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="b5d51-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-122">Files.ReadWrite.All</span></span> | <span data-ttu-id="b5d51-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5d51-123">Not supported</span></span> | <span data-ttu-id="b5d51-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-124">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="b5d51-125">event</span><span class="sxs-lookup"><span data-stu-id="b5d51-125">event</span></span>](../resources/event.md) | <span data-ttu-id="b5d51-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-126">Calendars.Read</span></span> | <span data-ttu-id="b5d51-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-127">Calendars.Read</span></span> | <span data-ttu-id="b5d51-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-128">Calendars.Read</span></span> |
|[<span data-ttu-id="b5d51-129">group</span><span class="sxs-lookup"><span data-stu-id="b5d51-129">group</span></span>](../resources/group.md) | <span data-ttu-id="b5d51-130">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-130">Group.Read.All</span></span> | <span data-ttu-id="b5d51-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5d51-131">Not supported</span></span> | <span data-ttu-id="b5d51-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-132">Group.Read.All</span></span> |
|[<span data-ttu-id="b5d51-133">group conversation</span><span class="sxs-lookup"><span data-stu-id="b5d51-133">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="b5d51-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-134">Group.Read.All</span></span> | <span data-ttu-id="b5d51-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5d51-135">Not supported</span></span> | <span data-ttu-id="b5d51-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5d51-136">Not supported</span></span> |
|[<span data-ttu-id="b5d51-137">list</span><span class="sxs-lookup"><span data-stu-id="b5d51-137">list</span></span>](../resources/list.md) | <span data-ttu-id="b5d51-138">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-138">Sites.ReadWrite.All</span></span> | <span data-ttu-id="b5d51-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5d51-139">Not supported</span></span> | <span data-ttu-id="b5d51-140">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-140">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="b5d51-141">message</span><span class="sxs-lookup"><span data-stu-id="b5d51-141">message</span></span>](../resources/message.md) | <span data-ttu-id="b5d51-142">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-142">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b5d51-143">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-143">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b5d51-144">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b5d51-144">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="b5d51-145">security alert</span><span class="sxs-lookup"><span data-stu-id="b5d51-145">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="b5d51-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-146">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="b5d51-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5d51-147">Not supported</span></span> | <span data-ttu-id="b5d51-148">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-148">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="b5d51-149">user</span><span class="sxs-lookup"><span data-stu-id="b5d51-149">user</span></span>](../resources/user.md) | <span data-ttu-id="b5d51-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-150">User.Read.All</span></span> | <span data-ttu-id="b5d51-151">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-151">User.Read.All</span></span> | <span data-ttu-id="b5d51-152">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5d51-152">User.Read.All</span></span> |

> <span data-ttu-id="b5d51-153">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="b5d51-153">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="b5d51-154">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="b5d51-154">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="b5d51-155">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="b5d51-155">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="b5d51-156">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="b5d51-156">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="b5d51-157">Уведомления об изменениях отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других объектов driveItem в иерархии.</span><span class="sxs-lookup"><span data-stu-id="b5d51-157">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="b5d51-158">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="b5d51-158">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="b5d51-159">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="b5d51-159">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="b5d51-160">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5d51-160">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user's mailbox.</span></span>
- <span data-ttu-id="b5d51-161">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="b5d51-161">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="b5d51-162">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b5d51-162">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="b5d51-163">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="b5d51-163">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="b5d51-164">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5d51-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b5d51-165">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5d51-165">Request headers</span></span>

| <span data-ttu-id="b5d51-166">Имя</span><span class="sxs-lookup"><span data-stu-id="b5d51-166">Name</span></span>       | <span data-ttu-id="b5d51-167">Тип</span><span class="sxs-lookup"><span data-stu-id="b5d51-167">Type</span></span> | <span data-ttu-id="b5d51-168">Описание</span><span class="sxs-lookup"><span data-stu-id="b5d51-168">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b5d51-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5d51-169">Authorization</span></span>  | <span data-ttu-id="b5d51-170">string</span><span class="sxs-lookup"><span data-stu-id="b5d51-170">string</span></span>  | <span data-ttu-id="b5d51-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5d51-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5d51-173">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5d51-173">Request body</span></span>

<span data-ttu-id="b5d51-174">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5d51-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5d51-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5d51-175">Response</span></span>

<span data-ttu-id="b5d51-176">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b5d51-176">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="b5d51-177">Сведения о том, как возвращаются ошибки, приведены в разделе [ошибочные ответы][error-response].</span><span class="sxs-lookup"><span data-stu-id="b5d51-177">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="b5d51-178">Пример</span><span class="sxs-lookup"><span data-stu-id="b5d51-178">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5d51-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5d51-179">Request</span></span>

<span data-ttu-id="b5d51-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5d51-180">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5d51-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5d51-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="b5d51-182">C#</span><span class="sxs-lookup"><span data-stu-id="b5d51-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5d51-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5d51-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5d51-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5d51-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5d51-185">Java</span><span class="sxs-lookup"><span data-stu-id="b5d51-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5d51-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5d51-186">Response</span></span>

<span data-ttu-id="b5d51-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5d51-187">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
