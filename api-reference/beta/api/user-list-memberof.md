---
title: Перечисление user memberOf
description: Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь. Эта операция не является транзитивной.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dcfed2df7e65bb3f628636bf787d9bcfce63a239
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016865"
---
# <a name="list-user-memberof"></a><span data-ttu-id="62952-104">Перечисление user memberOf</span><span class="sxs-lookup"><span data-stu-id="62952-104">List user memberOf</span></span>

<span data-ttu-id="62952-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62952-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62952-106">Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="62952-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="62952-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="62952-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="62952-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62952-108">Permissions</span></span>

<span data-ttu-id="62952-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62952-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62952-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62952-111">Permission type</span></span> | <span data-ttu-id="62952-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62952-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="62952-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62952-113">Delegated (work or school account)</span></span> | <span data-ttu-id="62952-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62952-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="62952-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62952-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62952-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62952-116">Not supported.</span></span> |
| <span data-ttu-id="62952-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62952-117">Application</span></span> | <span data-ttu-id="62952-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62952-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62952-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62952-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62952-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62952-120">Optional query parameters</span></span>

<span data-ttu-id="62952-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="62952-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="62952-122">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="62952-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="62952-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="62952-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="62952-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="62952-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="62952-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="62952-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62952-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62952-126">Request headers</span></span>

| <span data-ttu-id="62952-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62952-127">Header</span></span> | <span data-ttu-id="62952-128">Значение</span><span class="sxs-lookup"><span data-stu-id="62952-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="62952-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62952-129">Authorization</span></span>  | <span data-ttu-id="62952-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62952-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62952-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="62952-132">ConsistencyLevel</span></span> | <span data-ttu-id="62952-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="62952-133">eventual.</span></span> <span data-ttu-id="62952-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="62952-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="62952-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="62952-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62952-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62952-136">Request body</span></span>

<span data-ttu-id="62952-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62952-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62952-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="62952-138">Response</span></span>

<span data-ttu-id="62952-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62952-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62952-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="62952-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="62952-141">Пример 1: получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь</span><span class="sxs-lookup"><span data-stu-id="62952-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="62952-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="62952-142">Request</span></span>

<span data-ttu-id="62952-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62952-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62952-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="62952-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="62952-145">C#</span><span class="sxs-lookup"><span data-stu-id="62952-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62952-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62952-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62952-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62952-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62952-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="62952-148">Response</span></span>

<span data-ttu-id="62952-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62952-149">The following is an example of the response.</span></span>
><span data-ttu-id="62952-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62952-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="62952-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62952-151">All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.group",
      "displayName": "All Users",
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="62952-152">Пример 2: получение только счетчика всех групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь</span><span class="sxs-lookup"><span data-stu-id="62952-152">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="62952-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="62952-153">Request</span></span>

<span data-ttu-id="62952-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62952-154">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62952-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="62952-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="62952-156">C#</span><span class="sxs-lookup"><span data-stu-id="62952-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62952-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62952-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62952-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62952-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62952-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="62952-159">Response</span></span>

<span data-ttu-id="62952-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62952-160">The following is an example of the response.</span></span>
><span data-ttu-id="62952-161">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62952-161">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="62952-162">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62952-162">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="62952-163">893</span><span class="sxs-lookup"><span data-stu-id="62952-163">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="62952-164">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="62952-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="62952-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="62952-165">Request</span></span>

<span data-ttu-id="62952-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62952-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62952-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="62952-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="62952-168">C#</span><span class="sxs-lookup"><span data-stu-id="62952-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62952-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62952-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62952-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62952-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62952-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="62952-171">Response</span></span>

<span data-ttu-id="62952-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62952-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="62952-173">294</span><span class="sxs-lookup"><span data-stu-id="62952-173">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="62952-174">Пример 4: используйте $search и приведение OData для получения членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="62952-174">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="62952-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="62952-175">Request</span></span>

<span data-ttu-id="62952-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62952-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62952-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="62952-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="62952-178">C#</span><span class="sxs-lookup"><span data-stu-id="62952-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62952-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62952-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62952-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62952-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62952-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="62952-181">Response</span></span>

<span data-ttu-id="62952-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62952-182">The following is an example of the response.</span></span>
><span data-ttu-id="62952-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62952-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="62952-185">Пример 5: используйте $filter и приведение OData для получения групп с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="62952-185">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="62952-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="62952-186">Request</span></span>

<span data-ttu-id="62952-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62952-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62952-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="62952-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="62952-189">C#</span><span class="sxs-lookup"><span data-stu-id="62952-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62952-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62952-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62952-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62952-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62952-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="62952-192">Response</span></span>

<span data-ttu-id="62952-193">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62952-193">The following is an example of the response.</span></span>
><span data-ttu-id="62952-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62952-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


