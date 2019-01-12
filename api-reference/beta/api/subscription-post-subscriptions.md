---
title: Создание подписки
description: Подписывается прослушиватель для получения уведомлений при изменении данных в Microsoft Graph ресурсов.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 0640a8de441a07e1abcc02a152f5a9812832db27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916546"
---
# <a name="create-subscription"></a><span data-ttu-id="0e68f-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="0e68f-103">Create subscription</span></span>

> <span data-ttu-id="0e68f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e68f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e68f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e68f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e68f-106">Подписывается прослушиватель для получения уведомлений при изменении данных в Microsoft Graph ресурсов.</span><span class="sxs-lookup"><span data-stu-id="0e68f-106">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e68f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0e68f-107">Permissions</span></span>

<span data-ttu-id="0e68f-108">Создание подписки на требует разрешения на чтение ресурса, для которого приложение будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="0e68f-108">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="0e68f-109">Например, чтобы получать уведомления о сообщениях, ваше приложение должно `Mail.Read` разрешений.</span><span class="sxs-lookup"><span data-stu-id="0e68f-109">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="0e68f-110">В таблице ниже перечислены рекомендуемые разрешения, которые требуются для каждого ресурса.</span><span class="sxs-lookup"><span data-stu-id="0e68f-110">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="0e68f-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e68f-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e68f-112">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="0e68f-112">Resource type / Item</span></span>        | <span data-ttu-id="0e68f-113">Разрешение</span><span class="sxs-lookup"><span data-stu-id="0e68f-113">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="0e68f-114">Contacts</span><span class="sxs-lookup"><span data-stu-id="0e68f-114">Contacts</span></span>                    | <span data-ttu-id="0e68f-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0e68f-115">Contacts.Read</span></span>       |
| <span data-ttu-id="0e68f-116">Беседы</span><span class="sxs-lookup"><span data-stu-id="0e68f-116">Conversations</span></span>               | <span data-ttu-id="0e68f-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e68f-117">Group.Read.All</span></span>      |
| <span data-ttu-id="0e68f-118">События</span><span class="sxs-lookup"><span data-stu-id="0e68f-118">Events</span></span>                      | <span data-ttu-id="0e68f-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0e68f-119">Calendars.Read</span></span>      |
| <span data-ttu-id="0e68f-120">Сообщения</span><span class="sxs-lookup"><span data-stu-id="0e68f-120">Messages</span></span>                    | <span data-ttu-id="0e68f-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0e68f-121">Mail.Read</span></span>           |
| <span data-ttu-id="0e68f-122">Группы</span><span class="sxs-lookup"><span data-stu-id="0e68f-122">Groups</span></span>                      | <span data-ttu-id="0e68f-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e68f-123">Group.Read.All</span></span>      |
| <span data-ttu-id="0e68f-124">Пользователи</span><span class="sxs-lookup"><span data-stu-id="0e68f-124">Users</span></span>                       | <span data-ttu-id="0e68f-125">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e68f-125">User.Read.All</span></span>       |
| <span data-ttu-id="0e68f-126">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="0e68f-126">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="0e68f-127">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="0e68f-127">Files.ReadWrite</span></span>     |
| <span data-ttu-id="0e68f-128">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="0e68f-128">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="0e68f-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e68f-129">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="0e68f-130">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="0e68f-130">Security alert</span></span>              | <span data-ttu-id="0e68f-131">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e68f-131">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="0e68f-132">**Примечание:** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="0e68f-132">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="0e68f-133">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="0e68f-133">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="0e68f-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e68f-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="0e68f-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e68f-135">Request headers</span></span>

| <span data-ttu-id="0e68f-136">Имя</span><span class="sxs-lookup"><span data-stu-id="0e68f-136">Name</span></span>       | <span data-ttu-id="0e68f-137">Тип</span><span class="sxs-lookup"><span data-stu-id="0e68f-137">Type</span></span> | <span data-ttu-id="0e68f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0e68f-138">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e68f-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e68f-139">Authorization</span></span>  | <span data-ttu-id="0e68f-140">string</span><span class="sxs-lookup"><span data-stu-id="0e68f-140">string</span></span>  | <span data-ttu-id="0e68f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e68f-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0e68f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e68f-143">Response</span></span>

<span data-ttu-id="0e68f-144">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0e68f-144">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e68f-145">Пример</span><span class="sxs-lookup"><span data-stu-id="0e68f-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0e68f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e68f-146">Request</span></span>

<span data-ttu-id="0e68f-147">В тексте запроса укажите представление объекта [подписки](../resources/subscription.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="0e68f-147">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="0e68f-148">`clientState` Поле является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0e68f-148">The `clientState` field is optional.</span></span>

<span data-ttu-id="0e68f-149">Этот пример запроса создает подписки для уведомлений о новых сообщений, полученных в настоящее время входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e68f-149">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="0e68f-150">Ниже приведены допустимые значения для свойства ресурса:</span><span class="sxs-lookup"><span data-stu-id="0e68f-150">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="0e68f-151">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="0e68f-151">Resource type</span></span> | <span data-ttu-id="0e68f-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="0e68f-152">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="0e68f-153">Почта</span><span class="sxs-lookup"><span data-stu-id="0e68f-153">Mail</span></span>|<span data-ttu-id="0e68f-154">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="0e68f-154">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="0e68f-155">me/messages</span><span class="sxs-lookup"><span data-stu-id="0e68f-155">me/messages</span></span>|
|<span data-ttu-id="0e68f-156">Контакты</span><span class="sxs-lookup"><span data-stu-id="0e68f-156">Contacts</span></span>|<span data-ttu-id="0e68f-157">me/contacts</span><span class="sxs-lookup"><span data-stu-id="0e68f-157">me/contacts</span></span>|
|<span data-ttu-id="0e68f-158">Календари</span><span class="sxs-lookup"><span data-stu-id="0e68f-158">Calendars</span></span>|<span data-ttu-id="0e68f-159">me/events</span><span class="sxs-lookup"><span data-stu-id="0e68f-159">me/events</span></span>|
|<span data-ttu-id="0e68f-160">Пользователи</span><span class="sxs-lookup"><span data-stu-id="0e68f-160">Users</span></span>|<span data-ttu-id="0e68f-161">users</span><span class="sxs-lookup"><span data-stu-id="0e68f-161">users</span></span>|
|<span data-ttu-id="0e68f-162">Группы</span><span class="sxs-lookup"><span data-stu-id="0e68f-162">Groups</span></span>|<span data-ttu-id="0e68f-163">группы</span><span class="sxs-lookup"><span data-stu-id="0e68f-163">groups</span></span>|
|<span data-ttu-id="0e68f-164">Conversations</span><span class="sxs-lookup"><span data-stu-id="0e68f-164">Conversations</span></span>|<span data-ttu-id="0e68f-165">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="0e68f-165">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="0e68f-166">Drives</span><span class="sxs-lookup"><span data-stu-id="0e68f-166">Drives</span></span>|<span data-ttu-id="0e68f-167">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="0e68f-167">me/drive/root</span></span>|
|<span data-ttu-id="0e68f-168">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="0e68f-168">Security alert</span></span>|<span data-ttu-id="0e68f-169">Оповещение системы безопасности /? $filter = состояние eq «Создать»</span><span class="sxs-lookup"><span data-stu-id="0e68f-169">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="0e68f-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e68f-170">Response</span></span>

<span data-ttu-id="0e68f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e68f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="0e68f-174">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="0e68f-174">Notification endpoint validation</span></span>

<span data-ttu-id="0e68f-175">Конечная точка уведомления подписки (указанного в `notificationUrl` свойство) должен быть способен отвечать на запрос проверки, как описано в [Настройка уведомлений для изменения в данные пользователя](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="0e68f-175">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="0e68f-176">Если не удается выполнить проверку, запрос на создание подписки возвращает ошибку 400 Ошибочный запрос.</span><span class="sxs-lookup"><span data-stu-id="0e68f-176">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
