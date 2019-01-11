---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
ms.openlocfilehash: 0feb4ffd49099eabb92e5519b25233100f2acbe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846839"
---
# <a name="get-subscription"></a><span data-ttu-id="cfda1-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="cfda1-103">Get subscription</span></span>

> <span data-ttu-id="cfda1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cfda1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfda1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfda1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cfda1-106">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="cfda1-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfda1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfda1-107">Permissions</span></span>

<span data-ttu-id="cfda1-p102">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfda1-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfda1-110">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="cfda1-110">Resource type / Item</span></span>        | <span data-ttu-id="cfda1-111">Разрешение</span><span class="sxs-lookup"><span data-stu-id="cfda1-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="cfda1-112">Contacts</span><span class="sxs-lookup"><span data-stu-id="cfda1-112">Contacts</span></span>                    | <span data-ttu-id="cfda1-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cfda1-113">Contacts.Read</span></span>       |
| <span data-ttu-id="cfda1-114">Беседы</span><span class="sxs-lookup"><span data-stu-id="cfda1-114">Conversations</span></span>               | <span data-ttu-id="cfda1-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfda1-115">Group.Read.All</span></span>      |
| <span data-ttu-id="cfda1-116">События</span><span class="sxs-lookup"><span data-stu-id="cfda1-116">Events</span></span>                      | <span data-ttu-id="cfda1-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cfda1-117">Calendars.Read</span></span>      |
| <span data-ttu-id="cfda1-118">Сообщения</span><span class="sxs-lookup"><span data-stu-id="cfda1-118">Messages</span></span>                    | <span data-ttu-id="cfda1-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cfda1-119">Mail.Read</span></span>           |
| <span data-ttu-id="cfda1-120">Группы</span><span class="sxs-lookup"><span data-stu-id="cfda1-120">Groups</span></span>                      | <span data-ttu-id="cfda1-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfda1-121">Group.Read.All</span></span>      |
| <span data-ttu-id="cfda1-122">Пользователи</span><span class="sxs-lookup"><span data-stu-id="cfda1-122">Users</span></span>                       | <span data-ttu-id="cfda1-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfda1-123">User.Read.All</span></span>       |
| <span data-ttu-id="cfda1-124">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="cfda1-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="cfda1-125">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="cfda1-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="cfda1-126">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="cfda1-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="cfda1-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfda1-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="cfda1-128">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="cfda1-128">Security alert</span></span>              | <span data-ttu-id="cfda1-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfda1-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="cfda1-130">***Примечание:*** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cfda1-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="cfda1-131">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="cfda1-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="cfda1-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfda1-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfda1-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cfda1-133">Optional query parameters</span></span>

<span data-ttu-id="cfda1-134">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cfda1-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfda1-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfda1-135">Request headers</span></span>

| <span data-ttu-id="cfda1-136">Имя</span><span class="sxs-lookup"><span data-stu-id="cfda1-136">Name</span></span>       | <span data-ttu-id="cfda1-137">Тип</span><span class="sxs-lookup"><span data-stu-id="cfda1-137">Type</span></span> | <span data-ttu-id="cfda1-138">Описание</span><span class="sxs-lookup"><span data-stu-id="cfda1-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="cfda1-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfda1-139">Authorization</span></span>  | <span data-ttu-id="cfda1-140">string</span><span class="sxs-lookup"><span data-stu-id="cfda1-140">string</span></span>  | <span data-ttu-id="cfda1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfda1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfda1-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cfda1-143">Request body</span></span>

<span data-ttu-id="cfda1-144">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfda1-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfda1-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfda1-145">Response</span></span>

<span data-ttu-id="cfda1-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cfda1-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfda1-147">Пример</span><span class="sxs-lookup"><span data-stu-id="cfda1-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cfda1-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfda1-148">Request</span></span>

<span data-ttu-id="cfda1-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfda1-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="cfda1-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="cfda1-150">Response</span></span>

<span data-ttu-id="cfda1-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cfda1-151">Here is an example of the response.</span></span>
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
