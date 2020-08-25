---
title: Перечисление user memberOf
description: Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь. Эта операция не является транзитивной.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0c5b1e89bcc234894c83abee9ac52ab2ff0fa0b3
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873295"
---
# <a name="list-user-memberof"></a><span data-ttu-id="7505d-104">Перечисление user memberOf</span><span class="sxs-lookup"><span data-stu-id="7505d-104">List user memberOf</span></span>

<span data-ttu-id="7505d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7505d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7505d-106">Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="7505d-106">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="7505d-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="7505d-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="7505d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7505d-108">Permissions</span></span>

<span data-ttu-id="7505d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7505d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7505d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7505d-111">Permission type</span></span> | <span data-ttu-id="7505d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7505d-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="7505d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7505d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7505d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7505d-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="7505d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7505d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7505d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7505d-116">Not supported.</span></span> |
| <span data-ttu-id="7505d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7505d-117">Application</span></span> | <span data-ttu-id="7505d-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7505d-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7505d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7505d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7505d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7505d-120">Optional query parameters</span></span>

<span data-ttu-id="7505d-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7505d-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="7505d-122">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только перечисление directoryrole, членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="7505d-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="7505d-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="7505d-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="7505d-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="7505d-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="7505d-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="7505d-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7505d-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7505d-126">Request headers</span></span>

| <span data-ttu-id="7505d-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7505d-127">Header</span></span> | <span data-ttu-id="7505d-128">Значение</span><span class="sxs-lookup"><span data-stu-id="7505d-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="7505d-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7505d-129">Authorization</span></span>  | <span data-ttu-id="7505d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7505d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7505d-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="7505d-132">ConsistencyLevel</span></span> | <span data-ttu-id="7505d-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="7505d-133">eventual.</span></span> <span data-ttu-id="7505d-134">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="7505d-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="7505d-135">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="7505d-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7505d-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7505d-136">Request body</span></span>

<span data-ttu-id="7505d-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7505d-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7505d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7505d-138">Response</span></span>

<span data-ttu-id="7505d-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7505d-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7505d-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="7505d-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="7505d-141">Пример 1: получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь</span><span class="sxs-lookup"><span data-stu-id="7505d-141">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="7505d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7505d-142">Request</span></span>

<span data-ttu-id="7505d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7505d-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7505d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7505d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="7505d-145">C#</span><span class="sxs-lookup"><span data-stu-id="7505d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7505d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7505d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7505d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7505d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7505d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="7505d-148">Response</span></span>

<span data-ttu-id="7505d-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7505d-149">The following is an example of the response.</span></span>
><span data-ttu-id="7505d-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7505d-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7505d-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7505d-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="7505d-152">Пример 2: получение только счетчика всех групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь</span><span class="sxs-lookup"><span data-stu-id="7505d-152">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="7505d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="7505d-153">Request</span></span>

<span data-ttu-id="7505d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7505d-154">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7505d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="7505d-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7505d-156">C#</span><span class="sxs-lookup"><span data-stu-id="7505d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7505d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7505d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7505d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7505d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7505d-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="7505d-159">Response</span></span>

<span data-ttu-id="7505d-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7505d-160">The following is an example of the response.</span></span>
><span data-ttu-id="7505d-161">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7505d-161">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7505d-162">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7505d-162">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="7505d-163">893</span><span class="sxs-lookup"><span data-stu-id="7505d-163">893</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="7505d-164">Пример 3: Использование приведения OData для получения только количества участников группы</span><span class="sxs-lookup"><span data-stu-id="7505d-164">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="7505d-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="7505d-165">Request</span></span>

<span data-ttu-id="7505d-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7505d-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7505d-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="7505d-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7505d-168">C#</span><span class="sxs-lookup"><span data-stu-id="7505d-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7505d-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7505d-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7505d-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7505d-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7505d-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="7505d-171">Response</span></span>

<span data-ttu-id="7505d-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7505d-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="7505d-173">294</span><span class="sxs-lookup"><span data-stu-id="7505d-173">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="7505d-174">Пример 4: используйте $search и приведение OData для получения членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="7505d-174">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7505d-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="7505d-175">Request</span></span>

<span data-ttu-id="7505d-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7505d-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7505d-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="7505d-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7505d-178">C#</span><span class="sxs-lookup"><span data-stu-id="7505d-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7505d-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7505d-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7505d-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7505d-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7505d-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="7505d-181">Response</span></span>

<span data-ttu-id="7505d-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7505d-182">The following is an example of the response.</span></span>
><span data-ttu-id="7505d-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7505d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="7505d-185">Пример 5: используйте $filter и приведение OData для получения групп с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="7505d-185">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7505d-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="7505d-186">Request</span></span>

<span data-ttu-id="7505d-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7505d-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7505d-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="7505d-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7505d-189">C#</span><span class="sxs-lookup"><span data-stu-id="7505d-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7505d-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7505d-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7505d-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7505d-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7505d-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="7505d-192">Response</span></span>

<span data-ttu-id="7505d-193">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7505d-193">The following is an example of the response.</span></span>
><span data-ttu-id="7505d-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7505d-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
