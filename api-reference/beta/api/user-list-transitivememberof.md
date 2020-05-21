---
title: Список транзитивных пользователей memberOf
description: Получение групп, ролей каталогов и административных единиц, участником которых является пользователь. Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 3918706c2eb39ad8fc7ff11499e147c732c90728
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336750"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="7dd76-104">Список транзитивных пользователей memberOf</span><span class="sxs-lookup"><span data-stu-id="7dd76-104">List user transitive memberOf</span></span>

<span data-ttu-id="7dd76-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dd76-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dd76-106">Получение групп, ролей каталогов и административных единиц, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="7dd76-106">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="7dd76-107">Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.</span><span class="sxs-lookup"><span data-stu-id="7dd76-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dd76-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dd76-108">Permissions</span></span>

<span data-ttu-id="7dd76-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dd76-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7dd76-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dd76-111">Permission type</span></span> | <span data-ttu-id="7dd76-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dd76-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="7dd76-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dd76-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7dd76-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7dd76-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="7dd76-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dd76-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dd76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dd76-116">Not supported.</span></span> |
| <span data-ttu-id="7dd76-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dd76-117">Application</span></span> | <span data-ttu-id="7dd76-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dd76-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dd76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dd76-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7dd76-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7dd76-120">Optional query parameters</span></span>

<span data-ttu-id="7dd76-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="7dd76-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="7dd76-122">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только транзитивное членство в группах.</span><span class="sxs-lookup"><span data-stu-id="7dd76-122">OData cast is also enabled, for example, you can cast to get just the transitive membership in groups.</span></span> <span data-ttu-id="7dd76-123">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="7dd76-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="7dd76-124">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd76-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="7dd76-125">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="7dd76-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dd76-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dd76-126">Request headers</span></span>

| <span data-ttu-id="7dd76-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7dd76-127">Header</span></span> | <span data-ttu-id="7dd76-128">Значение</span><span class="sxs-lookup"><span data-stu-id="7dd76-128">Value</span></span> |
|:------ |:----- |
| <span data-ttu-id="7dd76-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dd76-129">Authorization</span></span>  | <span data-ttu-id="7dd76-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7dd76-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7dd76-132">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="7dd76-132">ConsistencyLevel</span></span> | <span data-ttu-id="7dd76-133">закончить.</span><span class="sxs-lookup"><span data-stu-id="7dd76-133">eventual.</span></span> <span data-ttu-id="7dd76-134">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="7dd76-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="7dd76-135">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="7dd76-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dd76-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7dd76-136">Request body</span></span>

<span data-ttu-id="7dd76-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7dd76-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dd76-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd76-138">Response</span></span>

<span data-ttu-id="7dd76-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd76-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7dd76-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="7dd76-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-member-of"></a><span data-ttu-id="7dd76-141">Пример 1: получение групп, ролей каталогов и административных единиц, участником которых является пользователь</span><span class="sxs-lookup"><span data-stu-id="7dd76-141">Example 1: Get groups, directory roles, and administrative units that the user is a member of</span></span>

#### <a name="request"></a><span data-ttu-id="7dd76-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dd76-142">Request</span></span>

<span data-ttu-id="7dd76-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd76-143">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dd76-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dd76-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="7dd76-145">C#</span><span class="sxs-lookup"><span data-stu-id="7dd76-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dd76-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dd76-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dd76-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dd76-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dd76-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd76-148">Response</span></span>

<span data-ttu-id="7dd76-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd76-149">The following is an example of the response.</span></span>
><span data-ttu-id="7dd76-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7dd76-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7dd76-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dd76-151">All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value":[
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"All_Contoso_Licensing",
      "mailEnabled":true,
      "mailNickname":"ContosoMailNickName",
      "securityEnabled":true
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"ContosoAudience_PugetSound",
      "mailEnabled":true,
      "mailNickname":"Contoso_PugetSound",
      "securityEnabled":true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership-in-groups-directory-roles-and-administrative-units"></a><span data-ttu-id="7dd76-152">Пример 2: получение только счетчика транзитивного членства в группах, ролях каталогов и административных единицах</span><span class="sxs-lookup"><span data-stu-id="7dd76-152">Example 2: Get only a count of transitive membership in groups, directory roles, and administrative units</span></span>

#### <a name="request"></a><span data-ttu-id="7dd76-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dd76-153">Request</span></span>

<span data-ttu-id="7dd76-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd76-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dd76-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dd76-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7dd76-156">C#</span><span class="sxs-lookup"><span data-stu-id="7dd76-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dd76-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dd76-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dd76-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dd76-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dd76-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd76-159">Response</span></span>

<span data-ttu-id="7dd76-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd76-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="7dd76-161">893</span><span class="sxs-lookup"><span data-stu-id="7dd76-161">893</span></span>


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="7dd76-162">Пример 3: Использование приведения OData для получения только счетчика транзитивного членства в группах</span><span class="sxs-lookup"><span data-stu-id="7dd76-162">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="7dd76-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dd76-163">Request</span></span>

<span data-ttu-id="7dd76-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd76-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dd76-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dd76-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7dd76-166">C#</span><span class="sxs-lookup"><span data-stu-id="7dd76-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dd76-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dd76-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dd76-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dd76-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dd76-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd76-169">Response</span></span>

<span data-ttu-id="7dd76-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd76-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="7dd76-171">588</span><span class="sxs-lookup"><span data-stu-id="7dd76-171">588</span></span>


### <a name="example-4-use-search-and-odata-cast-to-get-transitive-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="7dd76-172">Пример 4: используйте $search и приведение OData для получения транзитивного членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="7dd76-172">Example 4: Use $search and OData cast to get transitive membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7dd76-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dd76-173">Request</span></span>

<span data-ttu-id="7dd76-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd76-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7dd76-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dd76-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7dd76-176">C#</span><span class="sxs-lookup"><span data-stu-id="7dd76-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dd76-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dd76-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dd76-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dd76-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7dd76-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd76-179">Response</span></span>

<span data-ttu-id="7dd76-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd76-180">The following is an example of the response.</span></span>
><span data-ttu-id="7dd76-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dd76-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-transitive-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="7dd76-183">Пример 5: используйте $filter и приведение OData для получения транзитивного членства в группах с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="7dd76-183">Example 5: Use $filter and OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7dd76-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dd76-184">Request</span></span>

<span data-ttu-id="7dd76-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd76-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7dd76-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="7dd76-186">Response</span></span>

<span data-ttu-id="7dd76-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd76-187">The following is an example of the response.</span></span>
><span data-ttu-id="7dd76-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dd76-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
