---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
ms.openlocfilehash: 75b01a72310f9e9d227f4d185d13f6ee7dfdf835
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025498"
---
# <a name="update-subscription"></a><span data-ttu-id="68039-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="68039-103">Update subscription</span></span>

<span data-ttu-id="68039-104">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="68039-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="68039-105">Срок действия подписок после продолжительность времени, зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="68039-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="68039-106">Во избежание отсутствует уведомлений, приложение следует обновлять его подписки еще до которых истек срок действия.</span><span class="sxs-lookup"><span data-stu-id="68039-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="68039-107">В разделе [подписки](../resources/subscription.md) для Максимальная длина подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="68039-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="68039-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68039-108">Permissions</span></span>

<span data-ttu-id="68039-p102">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68039-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68039-111">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="68039-111">Resource type / Item</span></span>        | <span data-ttu-id="68039-112">Разрешение</span><span class="sxs-lookup"><span data-stu-id="68039-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="68039-113">Contacts</span><span class="sxs-lookup"><span data-stu-id="68039-113">Contacts</span></span>                    | <span data-ttu-id="68039-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="68039-114">Contacts.Read</span></span>       |
| <span data-ttu-id="68039-115">Беседы</span><span class="sxs-lookup"><span data-stu-id="68039-115">Conversations</span></span>               | <span data-ttu-id="68039-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="68039-116">Group.Read.All</span></span>      |
| <span data-ttu-id="68039-117">События</span><span class="sxs-lookup"><span data-stu-id="68039-117">Events</span></span>                      | <span data-ttu-id="68039-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="68039-118">Calendars.Read</span></span>      |
| <span data-ttu-id="68039-119">Сообщения</span><span class="sxs-lookup"><span data-stu-id="68039-119">Messages</span></span>                    | <span data-ttu-id="68039-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="68039-120">Mail.Read</span></span>           |
| <span data-ttu-id="68039-121">Groups</span><span class="sxs-lookup"><span data-stu-id="68039-121">Groups</span></span>                      | <span data-ttu-id="68039-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="68039-122">Group.Read.All</span></span>      |
| <span data-ttu-id="68039-123">Users</span><span class="sxs-lookup"><span data-stu-id="68039-123">Users</span></span>                       | <span data-ttu-id="68039-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="68039-124">User.Read.All</span></span>       |
| <span data-ttu-id="68039-125">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="68039-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="68039-126">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="68039-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="68039-127">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="68039-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="68039-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68039-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="68039-129">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="68039-129">Security alert</span></span>| <span data-ttu-id="68039-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68039-130">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68039-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68039-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="68039-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68039-132">Request headers</span></span>

| <span data-ttu-id="68039-133">Имя</span><span class="sxs-lookup"><span data-stu-id="68039-133">Name</span></span>       | <span data-ttu-id="68039-134">Тип</span><span class="sxs-lookup"><span data-stu-id="68039-134">Type</span></span> | <span data-ttu-id="68039-135">Описание</span><span class="sxs-lookup"><span data-stu-id="68039-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="68039-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="68039-136">Authorization</span></span>  | <span data-ttu-id="68039-137">string</span><span class="sxs-lookup"><span data-stu-id="68039-137">string</span></span>  | <span data-ttu-id="68039-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68039-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="68039-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="68039-140">Response</span></span>

<span data-ttu-id="68039-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68039-141">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68039-142">Пример</span><span class="sxs-lookup"><span data-stu-id="68039-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="68039-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="68039-143">Request</span></span>

<span data-ttu-id="68039-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68039-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="68039-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="68039-145">Response</span></span>

<span data-ttu-id="68039-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68039-146">Here is an example of the response.</span></span>
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
  "clientState":"subscription-identifier",
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
