---
title: Список транзитивных групп memberOf
description: Получение групп и административных единиц, участником которых является группа.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 81504242e1f5fed670cc783dfc500c4502272ffc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895834"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="2fd77-103">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="2fd77-103">List group transitive memberOf</span></span>

<span data-ttu-id="2fd77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fd77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fd77-105">Получение групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="2fd77-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="2fd77-106">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="2fd77-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="2fd77-107">В отличие от того, что получает группы Microsoft 365 пользователя, возвращаются все типы групп, а не только группы Майкрософт 365.</span><span class="sxs-lookup"><span data-stu-id="2fd77-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fd77-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2fd77-108">Permissions</span></span>

<span data-ttu-id="2fd77-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2fd77-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2fd77-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fd77-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fd77-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fd77-111">Permission type</span></span> | <span data-ttu-id="2fd77-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fd77-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="2fd77-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fd77-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2fd77-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2fd77-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="2fd77-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fd77-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fd77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fd77-116">Not supported.</span></span> |
| <span data-ttu-id="2fd77-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fd77-117">Application</span></span> | <span data-ttu-id="2fd77-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fd77-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2fd77-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fd77-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2fd77-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2fd77-120">Optional query parameters</span></span>

<span data-ttu-id="2fd77-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="2fd77-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="2fd77-122">Приведение OData также включено, например, можно выполнить приведение для получения только транзитивных участников группы.</span><span class="sxs-lookup"><span data-stu-id="2fd77-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="2fd77-123">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="2fd77-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="2fd77-124">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="2fd77-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="2fd77-125">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="2fd77-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fd77-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fd77-126">Request headers</span></span>

| <span data-ttu-id="2fd77-127">Имя</span><span class="sxs-lookup"><span data-stu-id="2fd77-127">Name</span></span> | <span data-ttu-id="2fd77-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2fd77-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="2fd77-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fd77-129">Authorization</span></span>  | <span data-ttu-id="2fd77-130">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="2fd77-130">Bearer {token}.</span></span> <span data-ttu-id="2fd77-131">Required.</span><span class="sxs-lookup"><span data-stu-id="2fd77-131">Required.</span></span> |
| <span data-ttu-id="2fd77-132">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="2fd77-132">ConsistencyLevel</span></span> | <span data-ttu-id="2fd77-133">закончить.</span><span class="sxs-lookup"><span data-stu-id="2fd77-133">eventual.</span></span> <span data-ttu-id="2fd77-134">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="2fd77-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="2fd77-135">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="2fd77-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fd77-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fd77-136">Request body</span></span>

<span data-ttu-id="2fd77-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2fd77-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fd77-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fd77-138">Response</span></span>

<span data-ttu-id="2fd77-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2fd77-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2fd77-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="2fd77-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="2fd77-141">Пример 1: получение групп и административных единиц, в которых группа является транзитивным участником</span><span class="sxs-lookup"><span data-stu-id="2fd77-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="2fd77-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fd77-142">Request</span></span>

<span data-ttu-id="2fd77-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fd77-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fd77-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd77-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="2fd77-145">C#</span><span class="sxs-lookup"><span data-stu-id="2fd77-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fd77-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fd77-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fd77-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fd77-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2fd77-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fd77-148">Response</span></span>

<span data-ttu-id="2fd77-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2fd77-149">The following is an example of the response.</span></span>
><span data-ttu-id="2fd77-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2fd77-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2fd77-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fd77-151">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "ContosoGroup1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="2fd77-152">Пример 2: получение только количества всех транзитивных членств</span><span class="sxs-lookup"><span data-stu-id="2fd77-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="2fd77-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fd77-153">Request</span></span>

<span data-ttu-id="2fd77-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fd77-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2fd77-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd77-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2fd77-156">C#</span><span class="sxs-lookup"><span data-stu-id="2fd77-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fd77-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fd77-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fd77-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fd77-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fd77-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fd77-159">Response</span></span>

<span data-ttu-id="2fd77-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2fd77-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="2fd77-161">294</span><span class="sxs-lookup"><span data-stu-id="2fd77-161">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="2fd77-162">Пример 3: Использование приведения OData для получения только счетчика транзитивного членства в группах</span><span class="sxs-lookup"><span data-stu-id="2fd77-162">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="2fd77-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fd77-163">Request</span></span>

<span data-ttu-id="2fd77-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fd77-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2fd77-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd77-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2fd77-166">C#</span><span class="sxs-lookup"><span data-stu-id="2fd77-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fd77-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fd77-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fd77-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fd77-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fd77-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fd77-169">Response</span></span>

<span data-ttu-id="2fd77-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2fd77-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="2fd77-171">294</span><span class="sxs-lookup"><span data-stu-id="2fd77-171">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="2fd77-172">Пример 4: использование функции CAST и $search для получения членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="2fd77-172">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2fd77-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fd77-173">Request</span></span>

<span data-ttu-id="2fd77-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fd77-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2fd77-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fd77-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="2fd77-176">C#</span><span class="sxs-lookup"><span data-stu-id="2fd77-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fd77-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fd77-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fd77-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fd77-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fd77-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fd77-179">Response</span></span>

<span data-ttu-id="2fd77-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2fd77-180">The following is an example of the response.</span></span>
><span data-ttu-id="2fd77-181">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="2fd77-181">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2fd77-182">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2fd77-182">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="2fd77-183">Пример 5: использование функции CAST и $filter для получения членства с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="2fd77-183">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="2fd77-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fd77-184">Request</span></span>

<span data-ttu-id="2fd77-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fd77-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="2fd77-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="2fd77-186">Response</span></span>

<span data-ttu-id="2fd77-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2fd77-187">The following is an example of the response.</span></span>
><span data-ttu-id="2fd77-188">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="2fd77-188">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2fd77-189">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2fd77-189">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
