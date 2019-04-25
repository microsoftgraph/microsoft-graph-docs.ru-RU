---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 97df6f59d4a8acfacec479e718970feef0c77632
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520664"
---
# <a name="delete-subscription"></a><span data-ttu-id="66944-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="66944-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66944-104">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="66944-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="66944-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66944-105">Permissions</span></span>

<span data-ttu-id="66944-106">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="66944-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="66944-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66944-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66944-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="66944-108">Supported resource</span></span> | <span data-ttu-id="66944-109">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66944-109">Delegated (work or school account)</span></span> | <span data-ttu-id="66944-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66944-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66944-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66944-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="66944-112">contact</span><span class="sxs-lookup"><span data-stu-id="66944-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="66944-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66944-113">Contacts.Read</span></span> | <span data-ttu-id="66944-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66944-114">Contacts.Read</span></span> | <span data-ttu-id="66944-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="66944-115">Contacts.Read</span></span> |
|<span data-ttu-id="66944-116">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="66944-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="66944-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="66944-117">Not supported</span></span> | <span data-ttu-id="66944-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66944-118">Files.ReadWrite</span></span> | <span data-ttu-id="66944-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="66944-119">Not supported</span></span> |
|<span data-ttu-id="66944-120">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="66944-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="66944-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66944-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="66944-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="66944-122">Not supported</span></span> | <span data-ttu-id="66944-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66944-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="66944-124">event</span><span class="sxs-lookup"><span data-stu-id="66944-124">event</span></span>](../resources/event.md) | <span data-ttu-id="66944-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66944-125">Calendars.Read</span></span> | <span data-ttu-id="66944-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66944-126">Calendars.Read</span></span> | <span data-ttu-id="66944-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="66944-127">Calendars.Read</span></span> |
|[<span data-ttu-id="66944-128">group</span><span class="sxs-lookup"><span data-stu-id="66944-128">group</span></span>](../resources/group.md) | <span data-ttu-id="66944-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66944-129">Group.Read.All</span></span> | <span data-ttu-id="66944-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="66944-130">Not supported</span></span> | <span data-ttu-id="66944-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66944-131">Group.Read.All</span></span> |
|[<span data-ttu-id="66944-132">group conversation</span><span class="sxs-lookup"><span data-stu-id="66944-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="66944-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="66944-133">Group.Read.All</span></span> | <span data-ttu-id="66944-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="66944-134">Not supported</span></span> | <span data-ttu-id="66944-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="66944-135">Not supported</span></span> |
|[<span data-ttu-id="66944-136">message</span><span class="sxs-lookup"><span data-stu-id="66944-136">message</span></span>](../resources/message.md) | <span data-ttu-id="66944-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66944-137">Mail.Read</span></span> | <span data-ttu-id="66944-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66944-138">Mail.Read</span></span> | <span data-ttu-id="66944-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="66944-139">Mail.Read</span></span> |
|[<span data-ttu-id="66944-140">security alert</span><span class="sxs-lookup"><span data-stu-id="66944-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="66944-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66944-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="66944-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="66944-142">Not supported</span></span> | <span data-ttu-id="66944-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66944-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="66944-144">user</span><span class="sxs-lookup"><span data-stu-id="66944-144">user</span></span>](../resources/user.md) | <span data-ttu-id="66944-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="66944-145">User.Read.All</span></span> | <span data-ttu-id="66944-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="66944-146">User.Read.All</span></span> | <span data-ttu-id="66944-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="66944-147">User.Read.All</span></span> |

> <span data-ttu-id="66944-148">**Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook.</span><span class="sxs-lookup"><span data-stu-id="66944-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="66944-149">Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).</span><span class="sxs-lookup"><span data-stu-id="66944-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="66944-150">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="66944-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="66944-151">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="66944-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="66944-152">Уведомления отправляются для требуемых типов изменений папки, на которую оформлена подписка, или любого файла, папки и других экземпляров driveItem в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="66944-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="66944-153">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="66944-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="66944-154">В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="66944-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="66944-155">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="66944-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="66944-156">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="66944-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="66944-157">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="66944-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="66944-158">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="66944-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="66944-159">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66944-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="66944-160">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66944-160">Request headers</span></span>

| <span data-ttu-id="66944-161">Имя</span><span class="sxs-lookup"><span data-stu-id="66944-161">Name</span></span>       | <span data-ttu-id="66944-162">Тип</span><span class="sxs-lookup"><span data-stu-id="66944-162">Type</span></span> | <span data-ttu-id="66944-163">Описание</span><span class="sxs-lookup"><span data-stu-id="66944-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66944-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="66944-164">Authorization</span></span>  | <span data-ttu-id="66944-165">string</span><span class="sxs-lookup"><span data-stu-id="66944-165">string</span></span>  | <span data-ttu-id="66944-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66944-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66944-168">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66944-168">Request body</span></span>

<span data-ttu-id="66944-169">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66944-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66944-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="66944-170">Response</span></span>

<span data-ttu-id="66944-171">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="66944-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="66944-172">Пример</span><span class="sxs-lookup"><span data-stu-id="66944-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66944-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="66944-173">Request</span></span>

<span data-ttu-id="66944-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66944-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="66944-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="66944-175">Response</span></span>

<span data-ttu-id="66944-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66944-176">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
