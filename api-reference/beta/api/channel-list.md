---
title: Перечисление каналов
description: Получение списка каналов в команде.
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 67079a369f666ab3b689a7a80f51ee58f437bedc
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275691"
---
# <a name="list-channels"></a><span data-ttu-id="36609-103">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="36609-103">List channels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36609-104">Получение списка [каналов](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="36609-104">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="36609-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36609-105">Permissions</span></span>

<span data-ttu-id="36609-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36609-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36609-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36609-108">Permission type</span></span>      | <span data-ttu-id="36609-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36609-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36609-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36609-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36609-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36609-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="36609-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36609-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36609-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36609-113">Not supported.</span></span>    |
|<span data-ttu-id="36609-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36609-114">Application</span></span> | <span data-ttu-id="36609-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36609-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="36609-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="36609-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="36609-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="36609-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="36609-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36609-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36609-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="36609-119">Optional query parameters</span></span>
<span data-ttu-id="36609-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="36609-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36609-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36609-121">Request headers</span></span>

| <span data-ttu-id="36609-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36609-122">Header</span></span>       | <span data-ttu-id="36609-123">Значение</span><span class="sxs-lookup"><span data-stu-id="36609-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36609-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36609-124">Authorization</span></span>  | <span data-ttu-id="36609-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36609-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36609-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36609-127">Request body</span></span>

<span data-ttu-id="36609-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36609-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36609-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="36609-129">Response</span></span>

<span data-ttu-id="36609-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36609-130">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36609-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="36609-131">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="36609-132">Пример 1. Список всех каналов</span><span class="sxs-lookup"><span data-stu-id="36609-132">Example 1: List all users</span></span>

#### <a name="request"></a><span data-ttu-id="36609-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="36609-133">Request</span></span>

<span data-ttu-id="36609-134">Ниже показан пример запроса для получения списка всех каналов.</span><span class="sxs-lookup"><span data-stu-id="36609-134">The following example shows a request to list all channels.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36609-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="36609-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36609-136">C#</span><span class="sxs-lookup"><span data-stu-id="36609-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36609-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36609-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36609-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36609-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="36609-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="36609-139">Response</span></span>

<span data-ttu-id="36609-140">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="36609-140">The following is the response.</span></span>

> <span data-ttu-id="36609-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36609-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="36609-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36609-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="36609-143">Пример 2. Список всех закрытых каналов</span><span class="sxs-lookup"><span data-stu-id="36609-143">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="36609-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="36609-144">Request</span></span>

<span data-ttu-id="36609-145">Ниже показан пример запроса для получения списка всех закрытых каналов.</span><span class="sxs-lookup"><span data-stu-id="36609-145">The following example shows a request to list all private channels.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels?$filter=membershipType eq 'private'
```

#### <a name="response"></a><span data-ttu-id="36609-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="36609-146">Response</span></span>

<span data-ttu-id="36609-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36609-147">The following is an example of the response.</span></span>

> <span data-ttu-id="36609-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36609-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
