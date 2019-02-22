---
title: Создание подписки
description: ПодПисывает приложение прослушивателя на получение уведомлений при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a8b8189780ac0b820551fb885adcf843c9ebe8f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140168"
---
# <a name="create-subscription"></a><span data-ttu-id="01472-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="01472-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01472-104">ПодПисывает приложение прослушивателя на получение уведомлений, когда запрошенный тип изменений происходит с указанным ресурсом в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="01472-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="01472-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01472-105">Permissions</span></span>

<span data-ttu-id="01472-106">Для создания подписки необходимо прочитать область действия для ресурса.</span><span class="sxs-lookup"><span data-stu-id="01472-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="01472-107">Например, чтобы получать уведомления о сообщениях, вашему приложению требуется `Mail.Read` разрешение.</span><span class="sxs-lookup"><span data-stu-id="01472-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="01472-108">В зависимости от ресурса и запрашиваемого типа разрешения (делегированного или приложения) разрешение, указанное в следующей таблице, является минимальным привилегированным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="01472-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="01472-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01472-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01472-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="01472-110">Supported resource</span></span> | <span data-ttu-id="01472-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01472-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01472-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01472-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01472-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01472-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="01472-114">contact</span><span class="sxs-lookup"><span data-stu-id="01472-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="01472-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="01472-115">Contacts.Read</span></span> | <span data-ttu-id="01472-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="01472-116">Contacts.Read</span></span> | <span data-ttu-id="01472-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="01472-117">Contacts.Read</span></span> |
|<span data-ttu-id="01472-118">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="01472-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="01472-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01472-119">Not supported</span></span> | <span data-ttu-id="01472-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01472-120">Files.ReadWrite</span></span> | <span data-ttu-id="01472-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01472-121">Not supported</span></span> |
|<span data-ttu-id="01472-122">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="01472-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="01472-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01472-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="01472-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01472-124">Not supported</span></span> | <span data-ttu-id="01472-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01472-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="01472-126">event</span><span class="sxs-lookup"><span data-stu-id="01472-126">event</span></span>](../resources/event.md) | <span data-ttu-id="01472-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01472-127">Calendars.Read</span></span> | <span data-ttu-id="01472-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01472-128">Calendars.Read</span></span> | <span data-ttu-id="01472-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="01472-129">Calendars.Read</span></span> |
|[<span data-ttu-id="01472-130">group</span><span class="sxs-lookup"><span data-stu-id="01472-130">group</span></span>](../resources/group.md) | <span data-ttu-id="01472-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="01472-131">Group.Read.All</span></span> | <span data-ttu-id="01472-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01472-132">Not supported</span></span> | <span data-ttu-id="01472-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="01472-133">Group.Read.All</span></span> |
|[<span data-ttu-id="01472-134">Групповая беседа</span><span class="sxs-lookup"><span data-stu-id="01472-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="01472-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="01472-135">Group.Read.All</span></span> | <span data-ttu-id="01472-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01472-136">Not supported</span></span> | <span data-ttu-id="01472-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01472-137">Not supported</span></span> |
|[<span data-ttu-id="01472-138">message</span><span class="sxs-lookup"><span data-stu-id="01472-138">message</span></span>](../resources/message.md) | <span data-ttu-id="01472-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01472-139">Mail.Read</span></span> | <span data-ttu-id="01472-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01472-140">Mail.Read</span></span> | <span data-ttu-id="01472-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="01472-141">Mail.Read</span></span> |
|[<span data-ttu-id="01472-142">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="01472-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="01472-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01472-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="01472-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="01472-144">Not supported</span></span> | <span data-ttu-id="01472-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01472-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="01472-146">user</span><span class="sxs-lookup"><span data-stu-id="01472-146">user</span></span>](../resources/user.md) | <span data-ttu-id="01472-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="01472-147">User.Read.All</span></span> | <span data-ttu-id="01472-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="01472-148">User.Read.All</span></span> | <span data-ttu-id="01472-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="01472-149">User.Read.All</span></span> |

> <span data-ttu-id="01472-150">**Примечание:** Существуют дополнительные ограничения для подписок на OneDrive и элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="01472-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="01472-151">Ограничения применяются к созданию и управлению подписками (процессами, обновлением и удалением подписок).</span><span class="sxs-lookup"><span data-stu-id="01472-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="01472-152">В личном OneDrive вы можете подписаться на корневую папку или любую подпапку на этом диске.</span><span class="sxs-lookup"><span data-stu-id="01472-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="01472-153">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="01472-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="01472-154">Уведомления отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других экземпляров **driveItem** в иерархии.</span><span class="sxs-lookup"><span data-stu-id="01472-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="01472-155">Вы не можете подписаться на **диски** или экземпляры **driveItem** , которые не являются папками, например отдельными файлами.</span><span class="sxs-lookup"><span data-stu-id="01472-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="01472-156">Делегированное разрешение в Outlook поддерживает подписку на элементы в папках только в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="01472-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="01472-157">Это означает, например, вы не можете использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="01472-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="01472-158">Чтобы подписаться на уведомления об изменении контактов, событий или сообщений Outlook в _общих или делегированных_ папках, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="01472-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="01472-159">Используйте соответствующее разрешение приложения, чтобы подписаться на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="01472-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="01472-160">Не используйте разрешения на общий доступ к Outlook (Contacts. Read. Shared, Calendars. Read. Shared, mail. Read. Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменении элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="01472-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="01472-161">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01472-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="01472-162">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01472-162">Request headers</span></span>

| <span data-ttu-id="01472-163">Имя</span><span class="sxs-lookup"><span data-stu-id="01472-163">Name</span></span>       | <span data-ttu-id="01472-164">Тип</span><span class="sxs-lookup"><span data-stu-id="01472-164">Type</span></span> | <span data-ttu-id="01472-165">Описание</span><span class="sxs-lookup"><span data-stu-id="01472-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01472-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="01472-166">Authorization</span></span>  | <span data-ttu-id="01472-167">string</span><span class="sxs-lookup"><span data-stu-id="01472-167">string</span></span>  | <span data-ttu-id="01472-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01472-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="01472-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="01472-170">Response</span></span>

<span data-ttu-id="01472-171">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01472-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01472-172">Пример</span><span class="sxs-lookup"><span data-stu-id="01472-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="01472-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="01472-173">Request</span></span>

<span data-ttu-id="01472-174">В тексте запроса добавьте представление объекта [Subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01472-174">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="01472-175">`clientState` Поле является необязательным.</span><span class="sxs-lookup"><span data-stu-id="01472-175">The `clientState` field is optional.</span></span>

<span data-ttu-id="01472-176">В этом примере запрос создает подписку на уведомления о новых сообщениях, получаемых пользователем, который вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="01472-176">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="01472-177">Ниже приведены допустимые значения свойства Resource.</span><span class="sxs-lookup"><span data-stu-id="01472-177">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="01472-178">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="01472-178">Resource type</span></span> | <span data-ttu-id="01472-179">Примеры</span><span class="sxs-lookup"><span data-stu-id="01472-179">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="01472-180">Почта</span><span class="sxs-lookup"><span data-stu-id="01472-180">Mail</span></span>|<span data-ttu-id="01472-181">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="01472-181">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="01472-182">me/messages</span><span class="sxs-lookup"><span data-stu-id="01472-182">me/messages</span></span>|
|<span data-ttu-id="01472-183">Контакты</span><span class="sxs-lookup"><span data-stu-id="01472-183">Contacts</span></span>|<span data-ttu-id="01472-184">me/contacts</span><span class="sxs-lookup"><span data-stu-id="01472-184">me/contacts</span></span>|
|<span data-ttu-id="01472-185">Календари</span><span class="sxs-lookup"><span data-stu-id="01472-185">Calendars</span></span>|<span data-ttu-id="01472-186">me/events</span><span class="sxs-lookup"><span data-stu-id="01472-186">me/events</span></span>|
|<span data-ttu-id="01472-187">Пользователи</span><span class="sxs-lookup"><span data-stu-id="01472-187">Users</span></span>|<span data-ttu-id="01472-188">users</span><span class="sxs-lookup"><span data-stu-id="01472-188">users</span></span>|
|<span data-ttu-id="01472-189">Группы</span><span class="sxs-lookup"><span data-stu-id="01472-189">Groups</span></span>|<span data-ttu-id="01472-190">группы</span><span class="sxs-lookup"><span data-stu-id="01472-190">groups</span></span>|
|<span data-ttu-id="01472-191">Conversations</span><span class="sxs-lookup"><span data-stu-id="01472-191">Conversations</span></span>|<span data-ttu-id="01472-192">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="01472-192">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="01472-193">Drives</span><span class="sxs-lookup"><span data-stu-id="01472-193">Drives</span></span>|<span data-ttu-id="01472-194">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="01472-194">me/drive/root</span></span>|
|<span data-ttu-id="01472-195">Оповещение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="01472-195">Security alert</span></span>|<span data-ttu-id="01472-196">безопасность/оповещения? $filter = Status eq ' New '</span><span class="sxs-lookup"><span data-stu-id="01472-196">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="01472-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="01472-197">Response</span></span>

<span data-ttu-id="01472-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01472-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="01472-201">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="01472-201">Notification endpoint validation</span></span>

<span data-ttu-id="01472-202">Конечная точка уведомления о подписке ( `notificationUrl` указанная в свойстве) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в данных пользователя](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="01472-202">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="01472-203">Если проверка завершается неудачно, запрос на создание подписки возвращает сообщение об ошибке "ошибка запроса 400".</span><span class="sxs-lookup"><span data-stu-id="01472-203">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
