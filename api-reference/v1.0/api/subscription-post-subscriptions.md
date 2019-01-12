---
title: Создание подписки
description: Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 7b23968620abcb8f9a20e4a7b3598c21dec72980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913889"
---
# <a name="create-subscription"></a><span data-ttu-id="caa07-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="caa07-103">Create subscription</span></span>

<span data-ttu-id="caa07-104">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления при изменении данных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="caa07-104">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="caa07-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="caa07-105">Permissions</span></span>

<span data-ttu-id="caa07-p101">Создание подписки требует наличия области чтения для ресурса. Например, чтобы получать сообщения уведомлений, приложению необходимо разрешение `Mail.Read`. В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caa07-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="caa07-110">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="caa07-110">Resource type / Item</span></span>        | <span data-ttu-id="caa07-111">Разрешение</span><span class="sxs-lookup"><span data-stu-id="caa07-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="caa07-112">Contacts</span><span class="sxs-lookup"><span data-stu-id="caa07-112">Contacts</span></span>                    | <span data-ttu-id="caa07-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="caa07-113">Contacts.Read</span></span>       |
| <span data-ttu-id="caa07-114">Беседы</span><span class="sxs-lookup"><span data-stu-id="caa07-114">Conversations</span></span>               | <span data-ttu-id="caa07-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="caa07-115">Group.Read.All</span></span>      |
| <span data-ttu-id="caa07-116">События</span><span class="sxs-lookup"><span data-stu-id="caa07-116">Events</span></span>                      | <span data-ttu-id="caa07-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="caa07-117">Calendars.Read</span></span>      |
| <span data-ttu-id="caa07-118">Сообщения</span><span class="sxs-lookup"><span data-stu-id="caa07-118">Messages</span></span>                    | <span data-ttu-id="caa07-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="caa07-119">Mail.Read</span></span>           |
| <span data-ttu-id="caa07-120">Группы</span><span class="sxs-lookup"><span data-stu-id="caa07-120">Groups</span></span>                      | <span data-ttu-id="caa07-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="caa07-121">Group.Read.All</span></span>      |
| <span data-ttu-id="caa07-122">Пользователи</span><span class="sxs-lookup"><span data-stu-id="caa07-122">Users</span></span>                       | <span data-ttu-id="caa07-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="caa07-123">User.Read.All</span></span>       |
| <span data-ttu-id="caa07-124">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="caa07-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="caa07-125">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="caa07-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="caa07-126">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="caa07-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="caa07-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caa07-127">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="caa07-128">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="caa07-128">Security alert</span></span>| <span data-ttu-id="caa07-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caa07-129">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="caa07-130">**Примечание:** Конечная точка /v1.0 позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="caa07-130">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="caa07-131">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="caa07-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="caa07-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caa07-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="caa07-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caa07-133">Request headers</span></span>

| <span data-ttu-id="caa07-134">Имя</span><span class="sxs-lookup"><span data-stu-id="caa07-134">Name</span></span>       | <span data-ttu-id="caa07-135">Тип</span><span class="sxs-lookup"><span data-stu-id="caa07-135">Type</span></span> | <span data-ttu-id="caa07-136">Описание</span><span class="sxs-lookup"><span data-stu-id="caa07-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="caa07-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="caa07-137">Authorization</span></span>  | <span data-ttu-id="caa07-138">string</span><span class="sxs-lookup"><span data-stu-id="caa07-138">string</span></span>  | <span data-ttu-id="caa07-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caa07-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="caa07-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="caa07-141">Response</span></span>

<span data-ttu-id="caa07-142">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="caa07-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caa07-143">Пример</span><span class="sxs-lookup"><span data-stu-id="caa07-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="caa07-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="caa07-144">Request</span></span>

<span data-ttu-id="caa07-145">Ниже представлен пример запроса на отправку уведомления при получении пользователем нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="caa07-145">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="caa07-146">В тексте запроса укажите представление объекта [подписки](../resources/subscription.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="caa07-146">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="caa07-147">`clientState` Поле является необязательным.</span><span class="sxs-lookup"><span data-stu-id="caa07-147">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="caa07-148">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="caa07-148">Resources examples</span></span>

<span data-ttu-id="caa07-149">Ниже приведены допустимые значения свойства ресурса для подписки.</span><span class="sxs-lookup"><span data-stu-id="caa07-149">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="caa07-150">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="caa07-150">Resource type</span></span> | <span data-ttu-id="caa07-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="caa07-151">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="caa07-152">Почта</span><span class="sxs-lookup"><span data-stu-id="caa07-152">Mail</span></span>|<span data-ttu-id="caa07-153">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="caa07-153">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="caa07-154">me/messages</span><span class="sxs-lookup"><span data-stu-id="caa07-154">me/messages</span></span>|
|<span data-ttu-id="caa07-155">Контакты</span><span class="sxs-lookup"><span data-stu-id="caa07-155">Contacts</span></span>|<span data-ttu-id="caa07-156">me/contacts</span><span class="sxs-lookup"><span data-stu-id="caa07-156">me/contacts</span></span>|
|<span data-ttu-id="caa07-157">Календари</span><span class="sxs-lookup"><span data-stu-id="caa07-157">Calendars</span></span>|<span data-ttu-id="caa07-158">me/events</span><span class="sxs-lookup"><span data-stu-id="caa07-158">me/events</span></span>|
|<span data-ttu-id="caa07-159">Пользователи</span><span class="sxs-lookup"><span data-stu-id="caa07-159">Users</span></span>|<span data-ttu-id="caa07-160">users</span><span class="sxs-lookup"><span data-stu-id="caa07-160">users</span></span>|
|<span data-ttu-id="caa07-161">Группы</span><span class="sxs-lookup"><span data-stu-id="caa07-161">Groups</span></span>|<span data-ttu-id="caa07-162">группы</span><span class="sxs-lookup"><span data-stu-id="caa07-162">groups</span></span>|
|<span data-ttu-id="caa07-163">Conversations</span><span class="sxs-lookup"><span data-stu-id="caa07-163">Conversations</span></span>|<span data-ttu-id="caa07-164">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="caa07-164">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="caa07-165">Drives</span><span class="sxs-lookup"><span data-stu-id="caa07-165">Drives</span></span>|<span data-ttu-id="caa07-166">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="caa07-166">me/drive/root</span></span>|
|<span data-ttu-id="caa07-167">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="caa07-167">Security alert</span></span>|<span data-ttu-id="caa07-168">Оповещение системы безопасности /? $filter = состояние eq «Создать»</span><span class="sxs-lookup"><span data-stu-id="caa07-168">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="caa07-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="caa07-169">Response</span></span>

<span data-ttu-id="caa07-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="caa07-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="caa07-173">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="caa07-173">Notification endpoint validation</span></span>

<span data-ttu-id="caa07-174">Конечная точка уведомления подписки (указанного в `notificationUrl` свойство) должен быть способен отвечать на запрос проверки, как описано в [Настройка уведомлений для изменения в данные пользователя](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="caa07-174">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="caa07-175">Если не удается выполнить проверку, запрос на создание подписки возвращает ошибку 400 Ошибочный запрос.</span><span class="sxs-lookup"><span data-stu-id="caa07-175">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
