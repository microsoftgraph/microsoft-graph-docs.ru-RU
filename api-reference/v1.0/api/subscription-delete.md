---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 97df6f59d4a8acfacec479e718970feef0c77632
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161434"
---
# <a name="delete-subscription"></a><span data-ttu-id="6e3c6-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="6e3c6-103">Delete subscription</span></span>

<span data-ttu-id="6e3c6-104">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e3c6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e3c6-105">Permissions</span></span>

<span data-ttu-id="6e3c6-106">В зависимости от ресурса и запрашиваемого типа разрешения (делегированного или приложения) разрешение, указанное в следующей таблице, является минимальным привилегированным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6e3c6-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e3c6-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e3c6-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="6e3c6-108">Supported resource</span></span> | <span data-ttu-id="6e3c6-109">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e3c6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6e3c6-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e3c6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e3c6-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e3c6-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6e3c6-112">contact</span><span class="sxs-lookup"><span data-stu-id="6e3c6-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6e3c6-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-113">Contacts.Read</span></span> | <span data-ttu-id="6e3c6-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-114">Contacts.Read</span></span> | <span data-ttu-id="6e3c6-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-115">Contacts.Read</span></span> |
|<span data-ttu-id="6e3c6-116">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="6e3c6-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6e3c6-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e3c6-117">Not supported</span></span> | <span data-ttu-id="6e3c6-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e3c6-118">Files.ReadWrite</span></span> | <span data-ttu-id="6e3c6-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e3c6-119">Not supported</span></span> |
|<span data-ttu-id="6e3c6-120">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6e3c6-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6e3c6-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="6e3c6-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e3c6-122">Not supported</span></span> | <span data-ttu-id="6e3c6-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6e3c6-124">event</span><span class="sxs-lookup"><span data-stu-id="6e3c6-124">event</span></span>](../resources/event.md) | <span data-ttu-id="6e3c6-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-125">Calendars.Read</span></span> | <span data-ttu-id="6e3c6-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-126">Calendars.Read</span></span> | <span data-ttu-id="6e3c6-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-127">Calendars.Read</span></span> |
|[<span data-ttu-id="6e3c6-128">group</span><span class="sxs-lookup"><span data-stu-id="6e3c6-128">group</span></span>](../resources/group.md) | <span data-ttu-id="6e3c6-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-129">Group.Read.All</span></span> | <span data-ttu-id="6e3c6-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e3c6-130">Not supported</span></span> | <span data-ttu-id="6e3c6-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-131">Group.Read.All</span></span> |
|[<span data-ttu-id="6e3c6-132">Групповая беседа</span><span class="sxs-lookup"><span data-stu-id="6e3c6-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6e3c6-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-133">Group.Read.All</span></span> | <span data-ttu-id="6e3c6-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e3c6-134">Not supported</span></span> | <span data-ttu-id="6e3c6-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e3c6-135">Not supported</span></span> |
|[<span data-ttu-id="6e3c6-136">message</span><span class="sxs-lookup"><span data-stu-id="6e3c6-136">message</span></span>](../resources/message.md) | <span data-ttu-id="6e3c6-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-137">Mail.Read</span></span> | <span data-ttu-id="6e3c6-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-138">Mail.Read</span></span> | <span data-ttu-id="6e3c6-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6e3c6-139">Mail.Read</span></span> |
|[<span data-ttu-id="6e3c6-140">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="6e3c6-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6e3c6-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6e3c6-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e3c6-142">Not supported</span></span> | <span data-ttu-id="6e3c6-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="6e3c6-144">user</span><span class="sxs-lookup"><span data-stu-id="6e3c6-144">user</span></span>](../resources/user.md) | <span data-ttu-id="6e3c6-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-145">User.Read.All</span></span> | <span data-ttu-id="6e3c6-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-146">User.Read.All</span></span> | <span data-ttu-id="6e3c6-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3c6-147">User.Read.All</span></span> |

> <span data-ttu-id="6e3c6-148">**Примечание:** Существуют дополнительные ограничения для подписок на OneDrive и элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="6e3c6-149">Ограничения применяются к созданию и управлению подписками (процессами, обновлением и удалением подписок).</span><span class="sxs-lookup"><span data-stu-id="6e3c6-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="6e3c6-150">В личном OneDrive вы можете подписаться на корневую папку или любую подпапку на этом диске.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6e3c6-151">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6e3c6-152">Уведомления отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других объектов driveItem в иерархии.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="6e3c6-153">Вы не можете подписаться на **диски** или экземпляры **driveItem** , которые не являются папками, например отдельными файлами.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="6e3c6-154">Делегированное разрешение в Outlook поддерживает подписку на элементы в папках только в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6e3c6-155">Это означает, например, вы не можете использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6e3c6-156">Чтобы подписаться на уведомления об изменении контактов, событий или сообщений Outlook в _общих или делегированных_ папках, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="6e3c6-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6e3c6-157">Используйте соответствующее разрешение приложения, чтобы подписаться на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6e3c6-158">Не используйте разрешения на общий доступ к Outlook (Contacts. Read. Shared, Calendars. Read. Shared, mail. Read. Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменении элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="6e3c6-159">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e3c6-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6e3c6-160">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e3c6-160">Request headers</span></span>

| <span data-ttu-id="6e3c6-161">Имя</span><span class="sxs-lookup"><span data-stu-id="6e3c6-161">Name</span></span>       | <span data-ttu-id="6e3c6-162">Тип</span><span class="sxs-lookup"><span data-stu-id="6e3c6-162">Type</span></span> | <span data-ttu-id="6e3c6-163">Описание</span><span class="sxs-lookup"><span data-stu-id="6e3c6-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6e3c6-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e3c6-164">Authorization</span></span>  | <span data-ttu-id="6e3c6-165">string</span><span class="sxs-lookup"><span data-stu-id="6e3c6-165">string</span></span>  | <span data-ttu-id="6e3c6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e3c6-168">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e3c6-168">Request body</span></span>

<span data-ttu-id="6e3c6-169">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e3c6-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e3c6-170">Response</span></span>

<span data-ttu-id="6e3c6-171">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6e3c6-172">Пример</span><span class="sxs-lookup"><span data-stu-id="6e3c6-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6e3c6-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e3c6-173">Request</span></span>

<span data-ttu-id="6e3c6-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="6e3c6-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e3c6-175">Response</span></span>

<span data-ttu-id="6e3c6-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6e3c6-176">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
