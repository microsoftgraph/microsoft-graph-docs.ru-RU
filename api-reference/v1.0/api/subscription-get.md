---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 4c55c81fdb26bb706ad270e5d53ded712ea69b22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956978"
---
# <a name="get-subscription"></a><span data-ttu-id="2434a-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="2434a-103">Get subscription</span></span>

<span data-ttu-id="2434a-104">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="2434a-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="2434a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2434a-105">Permissions</span></span>

<span data-ttu-id="2434a-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2434a-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2434a-108">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="2434a-108">Resource type / Item</span></span>        | <span data-ttu-id="2434a-109">Разрешение</span><span class="sxs-lookup"><span data-stu-id="2434a-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="2434a-110">Contacts</span><span class="sxs-lookup"><span data-stu-id="2434a-110">Contacts</span></span>                    | <span data-ttu-id="2434a-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2434a-111">Contacts.Read</span></span>       |
| <span data-ttu-id="2434a-112">Беседы</span><span class="sxs-lookup"><span data-stu-id="2434a-112">Conversations</span></span>               | <span data-ttu-id="2434a-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2434a-113">Group.Read.All</span></span>      |
| <span data-ttu-id="2434a-114">События</span><span class="sxs-lookup"><span data-stu-id="2434a-114">Events</span></span>                      | <span data-ttu-id="2434a-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2434a-115">Calendars.Read</span></span>      |
| <span data-ttu-id="2434a-116">Сообщения</span><span class="sxs-lookup"><span data-stu-id="2434a-116">Messages</span></span>                    | <span data-ttu-id="2434a-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2434a-117">Mail.Read</span></span>           |
| <span data-ttu-id="2434a-118">Группы</span><span class="sxs-lookup"><span data-stu-id="2434a-118">Groups</span></span>                      | <span data-ttu-id="2434a-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2434a-119">Group.Read.All</span></span>      |
| <span data-ttu-id="2434a-120">Users</span><span class="sxs-lookup"><span data-stu-id="2434a-120">Users</span></span>                       | <span data-ttu-id="2434a-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2434a-121">User.Read.All</span></span>       |
| <span data-ttu-id="2434a-122">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="2434a-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="2434a-123">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="2434a-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="2434a-124">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="2434a-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="2434a-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2434a-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="2434a-126">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="2434a-126">Security alert</span></span>| <span data-ttu-id="2434a-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2434a-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2434a-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2434a-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2434a-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2434a-129">Optional query parameters</span></span>

<span data-ttu-id="2434a-130">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2434a-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2434a-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2434a-131">Request headers</span></span>

| <span data-ttu-id="2434a-132">Имя</span><span class="sxs-lookup"><span data-stu-id="2434a-132">Name</span></span>       | <span data-ttu-id="2434a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2434a-133">Type</span></span> | <span data-ttu-id="2434a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2434a-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2434a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="2434a-135">Authorization</span></span>  | <span data-ttu-id="2434a-136">строка</span><span class="sxs-lookup"><span data-stu-id="2434a-136">string</span></span>  | <span data-ttu-id="2434a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2434a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2434a-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2434a-139">Request body</span></span>

<span data-ttu-id="2434a-140">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2434a-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2434a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2434a-141">Response</span></span>

<span data-ttu-id="2434a-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2434a-142">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2434a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2434a-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2434a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2434a-144">Request</span></span>

<span data-ttu-id="2434a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2434a-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="2434a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2434a-146">Response</span></span>

<span data-ttu-id="2434a-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2434a-147">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
