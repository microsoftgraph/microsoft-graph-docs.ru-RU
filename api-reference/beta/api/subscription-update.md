---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
ms.openlocfilehash: e2021e22d84ad9e05429db7980d37cbd1574843c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076740"
---
# <a name="update-subscription"></a><span data-ttu-id="c1043-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="c1043-103">Update subscription</span></span>

> <span data-ttu-id="c1043-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1043-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1043-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1043-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1043-106">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="c1043-106">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="c1043-107">Срок действия подписок после продолжительность времени, зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="c1043-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="c1043-108">Во избежание отсутствует уведомлений, приложение следует обновлять его подписки еще до которых истек срок действия.</span><span class="sxs-lookup"><span data-stu-id="c1043-108">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="c1043-109">В разделе [подписки](../resources/subscription.md) для Максимальная длина подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c1043-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1043-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1043-110">Permissions</span></span>

<span data-ttu-id="c1043-p103">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1043-p103">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1043-113">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="c1043-113">Resource type / Item</span></span>        | <span data-ttu-id="c1043-114">Разрешение</span><span class="sxs-lookup"><span data-stu-id="c1043-114">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="c1043-115">Contacts</span><span class="sxs-lookup"><span data-stu-id="c1043-115">Contacts</span></span>                    | <span data-ttu-id="c1043-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c1043-116">Contacts.Read</span></span>       |
| <span data-ttu-id="c1043-117">Беседы</span><span class="sxs-lookup"><span data-stu-id="c1043-117">Conversations</span></span>               | <span data-ttu-id="c1043-118">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1043-118">Group.Read.All</span></span>      |
| <span data-ttu-id="c1043-119">События</span><span class="sxs-lookup"><span data-stu-id="c1043-119">Events</span></span>                      | <span data-ttu-id="c1043-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c1043-120">Calendars.Read</span></span>      |
| <span data-ttu-id="c1043-121">Сообщения</span><span class="sxs-lookup"><span data-stu-id="c1043-121">Messages</span></span>                    | <span data-ttu-id="c1043-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c1043-122">Mail.Read</span></span>           |
| <span data-ttu-id="c1043-123">Groups</span><span class="sxs-lookup"><span data-stu-id="c1043-123">Groups</span></span>                      | <span data-ttu-id="c1043-124">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1043-124">Group.Read.All</span></span>      |
| <span data-ttu-id="c1043-125">Users</span><span class="sxs-lookup"><span data-stu-id="c1043-125">Users</span></span>                       | <span data-ttu-id="c1043-126">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1043-126">User.Read.All</span></span>       |
| <span data-ttu-id="c1043-127">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="c1043-127">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="c1043-128">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="c1043-128">Files.ReadWrite</span></span>     |
| <span data-ttu-id="c1043-129">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="c1043-129">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="c1043-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1043-130">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="c1043-131">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="c1043-131">Security alert</span></span>               | <span data-ttu-id="c1043-132">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1043-132">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="c1043-133">***Примечание:*** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c1043-133">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="c1043-134">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c1043-134">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="c1043-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1043-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c1043-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1043-136">Request headers</span></span>

| <span data-ttu-id="c1043-137">Имя</span><span class="sxs-lookup"><span data-stu-id="c1043-137">Name</span></span>       | <span data-ttu-id="c1043-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c1043-138">Type</span></span> | <span data-ttu-id="c1043-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c1043-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c1043-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1043-140">Authorization</span></span>  | <span data-ttu-id="c1043-141">string</span><span class="sxs-lookup"><span data-stu-id="c1043-141">string</span></span>  | <span data-ttu-id="c1043-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1043-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c1043-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1043-144">Response</span></span>

<span data-ttu-id="c1043-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1043-145">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1043-146">Пример</span><span class="sxs-lookup"><span data-stu-id="c1043-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c1043-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1043-147">Request</span></span>

<span data-ttu-id="c1043-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1043-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="c1043-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1043-149">Response</span></span>

<span data-ttu-id="c1043-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1043-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
