---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c7dd20810cd9fdacec697345d42690f85bc3b8b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522366"
---
# <a name="get-subscription"></a><span data-ttu-id="ddd4d-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="ddd4d-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddd4d-104">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddd4d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddd4d-105">Permissions</span></span>

<span data-ttu-id="ddd4d-p101">В приведенной ниже таблице перечислены рекомендуемые разрешения для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddd4d-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddd4d-108">Тип ресурса или элемент</span><span class="sxs-lookup"><span data-stu-id="ddd4d-108">Resource type / Item</span></span>        | <span data-ttu-id="ddd4d-109">Разрешение</span><span class="sxs-lookup"><span data-stu-id="ddd4d-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="ddd4d-110">Contacts</span><span class="sxs-lookup"><span data-stu-id="ddd4d-110">Contacts</span></span>                    | <span data-ttu-id="ddd4d-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ddd4d-111">Contacts.Read</span></span>       |
| <span data-ttu-id="ddd4d-112">Беседы</span><span class="sxs-lookup"><span data-stu-id="ddd4d-112">Conversations</span></span>               | <span data-ttu-id="ddd4d-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddd4d-113">Group.Read.All</span></span>      |
| <span data-ttu-id="ddd4d-114">События</span><span class="sxs-lookup"><span data-stu-id="ddd4d-114">Events</span></span>                      | <span data-ttu-id="ddd4d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ddd4d-115">Calendars.Read</span></span>      |
| <span data-ttu-id="ddd4d-116">Сообщения</span><span class="sxs-lookup"><span data-stu-id="ddd4d-116">Messages</span></span>                    | <span data-ttu-id="ddd4d-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ddd4d-117">Mail.Read</span></span>           |
| <span data-ttu-id="ddd4d-118">Группы</span><span class="sxs-lookup"><span data-stu-id="ddd4d-118">Groups</span></span>                      | <span data-ttu-id="ddd4d-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddd4d-119">Group.Read.All</span></span>      |
| <span data-ttu-id="ddd4d-120">Пользователи</span><span class="sxs-lookup"><span data-stu-id="ddd4d-120">Users</span></span>                       | <span data-ttu-id="ddd4d-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddd4d-121">User.Read.All</span></span>       |
| <span data-ttu-id="ddd4d-122">Диск (хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="ddd4d-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="ddd4d-123">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="ddd4d-124">На дисках (содержимое общих SharePoint и диски)</span><span class="sxs-lookup"><span data-stu-id="ddd4d-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="ddd4d-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddd4d-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="ddd4d-126">Предупреждение системы безопасности</span><span class="sxs-lookup"><span data-stu-id="ddd4d-126">Security alert</span></span>              | <span data-ttu-id="ddd4d-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddd4d-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="ddd4d-128">***Примечание:*** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="ddd4d-129">Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="ddd4d-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddd4d-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddd4d-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ddd4d-131">Optional query parameters</span></span>

<span data-ttu-id="ddd4d-132">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddd4d-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddd4d-133">Request headers</span></span>

| <span data-ttu-id="ddd4d-134">Имя</span><span class="sxs-lookup"><span data-stu-id="ddd4d-134">Name</span></span>       | <span data-ttu-id="ddd4d-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ddd4d-135">Type</span></span> | <span data-ttu-id="ddd4d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ddd4d-136">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="ddd4d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddd4d-137">Authorization</span></span>  | <span data-ttu-id="ddd4d-138">string</span><span class="sxs-lookup"><span data-stu-id="ddd4d-138">string</span></span>  | <span data-ttu-id="ddd4d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddd4d-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddd4d-141">Request body</span></span>

<span data-ttu-id="ddd4d-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddd4d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddd4d-143">Response</span></span>

<span data-ttu-id="ddd4d-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-144">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd4d-145">Пример</span><span class="sxs-lookup"><span data-stu-id="ddd4d-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ddd4d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddd4d-146">Request</span></span>

<span data-ttu-id="ddd4d-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="ddd4d-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddd4d-148">Response</span></span>

<span data-ttu-id="ddd4d-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ddd4d-149">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
