---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 3328291435e3d6ce067b21a604d76ce46ee5ea2e
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394475"
---
# <a name="delete-subscription"></a><span data-ttu-id="9530e-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="9530e-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9530e-104">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="9530e-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="9530e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9530e-105">Permissions</span></span>

<span data-ttu-id="9530e-106">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9530e-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="9530e-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9530e-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9530e-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="9530e-108">Supported resource</span></span> | <span data-ttu-id="9530e-109">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9530e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9530e-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9530e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9530e-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9530e-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="9530e-112">каллрекорд</span><span class="sxs-lookup"><span data-stu-id="9530e-112">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="9530e-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-113">Not supported</span></span> | <span data-ttu-id="9530e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-114">Not supported</span></span> | <span data-ttu-id="9530e-115">Каллрекордс. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="9530e-115">CallRecords.Read.All</span></span>  |
|[<span data-ttu-id="9530e-116">contact</span><span class="sxs-lookup"><span data-stu-id="9530e-116">contact</span></span>](../resources/contact.md) | <span data-ttu-id="9530e-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-117">Contacts.Read</span></span> | <span data-ttu-id="9530e-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-118">Contacts.Read</span></span> | <span data-ttu-id="9530e-119">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-119">Contacts.Read</span></span> |
|<span data-ttu-id="9530e-120">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="9530e-120">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="9530e-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-121">Not supported</span></span> | <span data-ttu-id="9530e-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9530e-122">Files.ReadWrite</span></span> | <span data-ttu-id="9530e-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-123">Not supported</span></span> |
|<span data-ttu-id="9530e-124">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="9530e-124">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="9530e-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9530e-125">Files.ReadWrite.All</span></span> | <span data-ttu-id="9530e-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-126">Not supported</span></span> | <span data-ttu-id="9530e-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9530e-127">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="9530e-128">event</span><span class="sxs-lookup"><span data-stu-id="9530e-128">event</span></span>](../resources/event.md) | <span data-ttu-id="9530e-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-129">Calendars.Read</span></span> | <span data-ttu-id="9530e-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-130">Calendars.Read</span></span> | <span data-ttu-id="9530e-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-131">Calendars.Read</span></span> |
|[<span data-ttu-id="9530e-132">group</span><span class="sxs-lookup"><span data-stu-id="9530e-132">group</span></span>](../resources/group.md) | <span data-ttu-id="9530e-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9530e-133">Group.Read.All</span></span> | <span data-ttu-id="9530e-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-134">Not supported</span></span> | <span data-ttu-id="9530e-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9530e-135">Group.Read.All</span></span> |
|[<span data-ttu-id="9530e-136">group conversation</span><span class="sxs-lookup"><span data-stu-id="9530e-136">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="9530e-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9530e-137">Group.Read.All</span></span> | <span data-ttu-id="9530e-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-138">Not supported</span></span> | <span data-ttu-id="9530e-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-139">Not supported</span></span> |
|[<span data-ttu-id="9530e-140">list</span><span class="sxs-lookup"><span data-stu-id="9530e-140">list</span></span>](../resources/list.md) | <span data-ttu-id="9530e-141">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9530e-141">Sites.ReadWrite.All</span></span> | <span data-ttu-id="9530e-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-142">Not supported</span></span> | <span data-ttu-id="9530e-143">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9530e-143">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="9530e-144">message</span><span class="sxs-lookup"><span data-stu-id="9530e-144">message</span></span>](../resources/message.md) | <span data-ttu-id="9530e-145">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-145">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="9530e-146">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-146">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="9530e-147">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9530e-147">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="9530e-148">security alert</span><span class="sxs-lookup"><span data-stu-id="9530e-148">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="9530e-149">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9530e-149">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="9530e-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9530e-150">Not supported</span></span> | <span data-ttu-id="9530e-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9530e-151">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="9530e-152">user</span><span class="sxs-lookup"><span data-stu-id="9530e-152">user</span></span>](../resources/user.md) | <span data-ttu-id="9530e-153">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9530e-153">User.Read.All</span></span> | <span data-ttu-id="9530e-154">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9530e-154">User.Read.All</span></span> | <span data-ttu-id="9530e-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9530e-155">User.Read.All</span></span> |

> <span data-ttu-id="9530e-156">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="9530e-156">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="9530e-157">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="9530e-157">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="9530e-158">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="9530e-158">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="9530e-159">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="9530e-159">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="9530e-160">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="9530e-160">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="9530e-161">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="9530e-161">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="9530e-162">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="9530e-162">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="9530e-163">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9530e-163">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="9530e-164">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="9530e-164">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="9530e-165">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="9530e-165">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="9530e-166">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="9530e-166">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="9530e-167">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9530e-167">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9530e-168">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9530e-168">Request headers</span></span>

| <span data-ttu-id="9530e-169">Имя</span><span class="sxs-lookup"><span data-stu-id="9530e-169">Name</span></span>       | <span data-ttu-id="9530e-170">Тип</span><span class="sxs-lookup"><span data-stu-id="9530e-170">Type</span></span> | <span data-ttu-id="9530e-171">Описание</span><span class="sxs-lookup"><span data-stu-id="9530e-171">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9530e-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="9530e-172">Authorization</span></span>  | <span data-ttu-id="9530e-173">string</span><span class="sxs-lookup"><span data-stu-id="9530e-173">string</span></span>  | <span data-ttu-id="9530e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9530e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9530e-176">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9530e-176">Request body</span></span>

<span data-ttu-id="9530e-177">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9530e-177">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9530e-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="9530e-178">Response</span></span>

<span data-ttu-id="9530e-179">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9530e-179">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9530e-180">Пример</span><span class="sxs-lookup"><span data-stu-id="9530e-180">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9530e-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="9530e-181">Request</span></span>

<span data-ttu-id="9530e-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9530e-182">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9530e-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="9530e-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="9530e-184">C#</span><span class="sxs-lookup"><span data-stu-id="9530e-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9530e-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9530e-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9530e-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9530e-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9530e-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="9530e-187">Response</span></span>

<span data-ttu-id="9530e-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9530e-188">Here is an example of the response.</span></span>
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
