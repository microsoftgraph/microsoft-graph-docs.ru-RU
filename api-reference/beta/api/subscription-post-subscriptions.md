---
title: Создание подписки
description: Подписывается прослушиватель для получения уведомлений при изменении данных в Microsoft Graph ресурсов.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 002dd88c7db2650be2303e7df6f86ce9a5fbdaa9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527579"
---
# <a name="create-subscription"></a><span data-ttu-id="b3b2b-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="b3b2b-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3b2b-104">Подписывается прослушиватель для получения уведомлений при изменении данных в Microsoft Graph ресурсов.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-104">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3b2b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3b2b-105">Permissions</span></span>

<span data-ttu-id="b3b2b-106">Создание подписки на требует разрешения на чтение ресурса, для которого приложение будет получать уведомления.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-106">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="b3b2b-107">Например, чтобы получать уведомления о сообщениях, ваше приложение должно `Mail.Read` разрешений.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-107">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="b3b2b-108">В таблице ниже перечислены рекомендуемые разрешения, которые требуются для каждого ресурса.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-108">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="b3b2b-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3b2b-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3b2b-110">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="b3b2b-110">Resource type / Item</span></span>        | <span data-ttu-id="b3b2b-111">Разрешение</span><span class="sxs-lookup"><span data-stu-id="b3b2b-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="b3b2b-112">Contacts</span><span class="sxs-lookup"><span data-stu-id="b3b2b-112">Contacts</span></span>                    | <span data-ttu-id="b3b2b-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b3b2b-113">Contacts.Read</span></span>       |
| <span data-ttu-id="b3b2b-114">Беседы</span><span class="sxs-lookup"><span data-stu-id="b3b2b-114">Conversations</span></span>               | <span data-ttu-id="b3b2b-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3b2b-115">Group.Read.All</span></span>      |
| <span data-ttu-id="b3b2b-116">События</span><span class="sxs-lookup"><span data-stu-id="b3b2b-116">Events</span></span>                      | <span data-ttu-id="b3b2b-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b3b2b-117">Calendars.Read</span></span>      |
| <span data-ttu-id="b3b2b-118">Сообщения</span><span class="sxs-lookup"><span data-stu-id="b3b2b-118">Messages</span></span>                    | <span data-ttu-id="b3b2b-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b3b2b-119">Mail.Read</span></span>           |
| <span data-ttu-id="b3b2b-120">Группы</span><span class="sxs-lookup"><span data-stu-id="b3b2b-120">Groups</span></span>                      | <span data-ttu-id="b3b2b-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3b2b-121">Group.Read.All</span></span>      |
| <span data-ttu-id="b3b2b-122">Пользователи</span><span class="sxs-lookup"><span data-stu-id="b3b2b-122">Users</span></span>                       | <span data-ttu-id="b3b2b-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3b2b-123">User.Read.All</span></span>       |
| <span data-ttu-id="b3b2b-124">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="b3b2b-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="b3b2b-125">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="b3b2b-126">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="b3b2b-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="b3b2b-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3b2b-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="b3b2b-128">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="b3b2b-128">Security alert</span></span>              | <span data-ttu-id="b3b2b-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3b2b-129">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="b3b2b-130">**Примечание:** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-130">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="b3b2b-131">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b3b2b-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3b2b-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="b3b2b-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3b2b-133">Request headers</span></span>

| <span data-ttu-id="b3b2b-134">Имя</span><span class="sxs-lookup"><span data-stu-id="b3b2b-134">Name</span></span>       | <span data-ttu-id="b3b2b-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b3b2b-135">Type</span></span> | <span data-ttu-id="b3b2b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b3b2b-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b3b2b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3b2b-137">Authorization</span></span>  | <span data-ttu-id="b3b2b-138">string</span><span class="sxs-lookup"><span data-stu-id="b3b2b-138">string</span></span>  | <span data-ttu-id="b3b2b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b3b2b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3b2b-141">Response</span></span>

<span data-ttu-id="b3b2b-142">В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3b2b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b3b2b-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3b2b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3b2b-144">Request</span></span>

<span data-ttu-id="b3b2b-145">В тексте запроса укажите представление объекта [подписки](../resources/subscription.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-145">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="b3b2b-146">`clientState` Поле является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-146">The `clientState` field is optional.</span></span>

<span data-ttu-id="b3b2b-147">Этот пример запроса создает подписки для уведомлений о новых сообщений, полученных в настоящее время входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-147">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="b3b2b-148">Ниже приведены допустимые значения для свойства ресурса:</span><span class="sxs-lookup"><span data-stu-id="b3b2b-148">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="b3b2b-149">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="b3b2b-149">Resource type</span></span> | <span data-ttu-id="b3b2b-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3b2b-150">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="b3b2b-151">Почта</span><span class="sxs-lookup"><span data-stu-id="b3b2b-151">Mail</span></span>|<span data-ttu-id="b3b2b-152">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="b3b2b-152">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="b3b2b-153">me/messages</span><span class="sxs-lookup"><span data-stu-id="b3b2b-153">me/messages</span></span>|
|<span data-ttu-id="b3b2b-154">Контакты</span><span class="sxs-lookup"><span data-stu-id="b3b2b-154">Contacts</span></span>|<span data-ttu-id="b3b2b-155">me/contacts</span><span class="sxs-lookup"><span data-stu-id="b3b2b-155">me/contacts</span></span>|
|<span data-ttu-id="b3b2b-156">Календари</span><span class="sxs-lookup"><span data-stu-id="b3b2b-156">Calendars</span></span>|<span data-ttu-id="b3b2b-157">me/events</span><span class="sxs-lookup"><span data-stu-id="b3b2b-157">me/events</span></span>|
|<span data-ttu-id="b3b2b-158">Пользователи</span><span class="sxs-lookup"><span data-stu-id="b3b2b-158">Users</span></span>|<span data-ttu-id="b3b2b-159">users</span><span class="sxs-lookup"><span data-stu-id="b3b2b-159">users</span></span>|
|<span data-ttu-id="b3b2b-160">Группы</span><span class="sxs-lookup"><span data-stu-id="b3b2b-160">Groups</span></span>|<span data-ttu-id="b3b2b-161">группы</span><span class="sxs-lookup"><span data-stu-id="b3b2b-161">groups</span></span>|
|<span data-ttu-id="b3b2b-162">Беседы</span><span class="sxs-lookup"><span data-stu-id="b3b2b-162">Conversations</span></span>|<span data-ttu-id="b3b2b-163">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="b3b2b-163">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="b3b2b-164">Drives</span><span class="sxs-lookup"><span data-stu-id="b3b2b-164">Drives</span></span>|<span data-ttu-id="b3b2b-165">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="b3b2b-165">me/drive/root</span></span>|
|<span data-ttu-id="b3b2b-166">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="b3b2b-166">Security alert</span></span>|<span data-ttu-id="b3b2b-167">Оповещение системы безопасности /? $filter = состояние eq «Создать»</span><span class="sxs-lookup"><span data-stu-id="b3b2b-167">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="b3b2b-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3b2b-168">Response</span></span>

<span data-ttu-id="b3b2b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b3b2b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="b3b2b-172">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="b3b2b-172">Notification endpoint validation</span></span>

<span data-ttu-id="b3b2b-173">Конечная точка уведомления подписки (указанного в `notificationUrl` свойство) должен быть способен отвечать на запрос проверки, как описано в [Настройка уведомлений для изменения в данные пользователя](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="b3b2b-173">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="b3b2b-174">Если не удается выполнить проверку, запрос на создание подписки возвращает ошибку 400 Ошибочный запрос.</span><span class="sxs-lookup"><span data-stu-id="b3b2b-174">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
