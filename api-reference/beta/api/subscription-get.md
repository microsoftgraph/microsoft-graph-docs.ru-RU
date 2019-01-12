---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 165fd990d7dbec64eb61b9e06d05b51b40bf1212
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934886"
---
# <a name="get-subscription"></a><span data-ttu-id="cf410-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="cf410-103">Get subscription</span></span>

> <span data-ttu-id="cf410-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cf410-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf410-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf410-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf410-106">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="cf410-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf410-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf410-107">Permissions</span></span>

<span data-ttu-id="cf410-p102">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf410-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf410-110">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="cf410-110">Resource type / Item</span></span>        | <span data-ttu-id="cf410-111">Разрешение</span><span class="sxs-lookup"><span data-stu-id="cf410-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="cf410-112">Contacts</span><span class="sxs-lookup"><span data-stu-id="cf410-112">Contacts</span></span>                    | <span data-ttu-id="cf410-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cf410-113">Contacts.Read</span></span>       |
| <span data-ttu-id="cf410-114">Беседы</span><span class="sxs-lookup"><span data-stu-id="cf410-114">Conversations</span></span>               | <span data-ttu-id="cf410-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf410-115">Group.Read.All</span></span>      |
| <span data-ttu-id="cf410-116">События</span><span class="sxs-lookup"><span data-stu-id="cf410-116">Events</span></span>                      | <span data-ttu-id="cf410-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cf410-117">Calendars.Read</span></span>      |
| <span data-ttu-id="cf410-118">Сообщения</span><span class="sxs-lookup"><span data-stu-id="cf410-118">Messages</span></span>                    | <span data-ttu-id="cf410-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cf410-119">Mail.Read</span></span>           |
| <span data-ttu-id="cf410-120">Группы</span><span class="sxs-lookup"><span data-stu-id="cf410-120">Groups</span></span>                      | <span data-ttu-id="cf410-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf410-121">Group.Read.All</span></span>      |
| <span data-ttu-id="cf410-122">Пользователи</span><span class="sxs-lookup"><span data-stu-id="cf410-122">Users</span></span>                       | <span data-ttu-id="cf410-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf410-123">User.Read.All</span></span>       |
| <span data-ttu-id="cf410-124">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="cf410-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="cf410-125">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="cf410-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="cf410-126">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="cf410-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="cf410-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf410-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="cf410-128">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="cf410-128">Security alert</span></span>              | <span data-ttu-id="cf410-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf410-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="cf410-130">***Примечание:*** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cf410-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="cf410-131">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="cf410-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="cf410-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf410-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf410-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf410-133">Optional query parameters</span></span>

<span data-ttu-id="cf410-134">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cf410-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf410-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf410-135">Request headers</span></span>

| <span data-ttu-id="cf410-136">Имя</span><span class="sxs-lookup"><span data-stu-id="cf410-136">Name</span></span>       | <span data-ttu-id="cf410-137">Тип</span><span class="sxs-lookup"><span data-stu-id="cf410-137">Type</span></span> | <span data-ttu-id="cf410-138">Описание</span><span class="sxs-lookup"><span data-stu-id="cf410-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="cf410-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf410-139">Authorization</span></span>  | <span data-ttu-id="cf410-140">string</span><span class="sxs-lookup"><span data-stu-id="cf410-140">string</span></span>  | <span data-ttu-id="cf410-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf410-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf410-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf410-143">Request body</span></span>

<span data-ttu-id="cf410-144">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf410-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf410-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf410-145">Response</span></span>

<span data-ttu-id="cf410-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf410-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf410-147">Пример</span><span class="sxs-lookup"><span data-stu-id="cf410-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf410-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf410-148">Request</span></span>

<span data-ttu-id="cf410-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf410-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="cf410-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf410-150">Response</span></span>

<span data-ttu-id="cf410-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf410-151">Here is an example of the response.</span></span>
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
