---
title: Перечисление user transitive memberOf
description: Получение групп, ролей каталогов, участником которых является пользователь. Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4ddc73c3cbe702759d12e3875b91e743decdbe8c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904337"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="f2ac5-104">Перечисление user transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="f2ac5-104">List user transitive memberOf</span></span>

<span data-ttu-id="f2ac5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2ac5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2ac5-106">Получение групп, ролей каталогов, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-106">Get groups, directory roles that the user is a member of.</span></span> <span data-ttu-id="f2ac5-107">Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-107">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2ac5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2ac5-108">Permissions</span></span>

<span data-ttu-id="f2ac5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2ac5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2ac5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2ac5-111">Permission type</span></span>      | <span data-ttu-id="f2ac5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2ac5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2ac5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2ac5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f2ac5-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2ac5-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2ac5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2ac5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2ac5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-116">Not supported.</span></span>    |
|<span data-ttu-id="f2ac5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2ac5-117">Application</span></span> | <span data-ttu-id="f2ac5-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2ac5-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f2ac5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2ac5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2ac5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2ac5-120">Optional query parameters</span></span>

<span data-ttu-id="f2ac5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="f2ac5-122">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только транзитивное членство в группах.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-122">OData cast is also enabled, for example, you can cast to get just the transitive membership in groups.</span></span> <span data-ttu-id="f2ac5-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="f2ac5-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="f2ac5-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2ac5-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2ac5-126">Request headers</span></span>

| <span data-ttu-id="f2ac5-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2ac5-127">Header</span></span>       | <span data-ttu-id="f2ac5-128">Значение</span><span class="sxs-lookup"><span data-stu-id="f2ac5-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2ac5-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2ac5-129">Authorization</span></span>  | <span data-ttu-id="f2ac5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f2ac5-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="f2ac5-132">ConsistencyLevel</span></span> | <span data-ttu-id="f2ac5-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-133">eventual.</span></span> <span data-ttu-id="f2ac5-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="f2ac5-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2ac5-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2ac5-136">Request body</span></span>

<span data-ttu-id="f2ac5-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2ac5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ac5-138">Response</span></span>

<span data-ttu-id="f2ac5-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2ac5-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2ac5-140">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-member-of"></a><span data-ttu-id="f2ac5-141">Пример 1: получение групп, ролей каталогов и административных единиц, участником которых является пользователь</span><span class="sxs-lookup"><span data-stu-id="f2ac5-141">Example 1: Get groups, directory roles, and administrative units that the user is a member of</span></span>

#### <a name="request"></a><span data-ttu-id="f2ac5-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2ac5-142">Request</span></span>

<span data-ttu-id="f2ac5-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2ac5-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ac5-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="f2ac5-145">C#</span><span class="sxs-lookup"><span data-stu-id="f2ac5-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2ac5-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2ac5-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2ac5-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2ac5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2ac5-148">Java</span><span class="sxs-lookup"><span data-stu-id="f2ac5-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f2ac5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ac5-149">Response</span></span>

<span data-ttu-id="f2ac5-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-150">The following is an example of the response.</span></span>

><span data-ttu-id="f2ac5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value":[
    {
      "@odata.type":"#microsoft.graph.group",
      "displayName":"All_Contoso_Licensing",
      "mailEnabled":true,
      "mailNickname":"ContosoMailNickName",
      "securityEnabled":true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership-in-groups-directory-roles-and-administrative-units"></a><span data-ttu-id="f2ac5-153">Пример 2: получение только счетчика транзитивного членства в группах, ролях каталогов и административных единицах</span><span class="sxs-lookup"><span data-stu-id="f2ac5-153">Example 2: Get only a count of transitive membership in groups, directory roles, and administrative units</span></span>

#### <a name="request"></a><span data-ttu-id="f2ac5-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2ac5-154">Request</span></span>

<span data-ttu-id="f2ac5-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2ac5-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ac5-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="f2ac5-157">C#</span><span class="sxs-lookup"><span data-stu-id="f2ac5-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2ac5-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2ac5-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2ac5-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2ac5-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2ac5-160">Java</span><span class="sxs-lookup"><span data-stu-id="f2ac5-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f2ac5-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ac5-161">Response</span></span>

<span data-ttu-id="f2ac5-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="f2ac5-163">Пример 3. Использование OData cast для получения только количества транзитивных участников в группах</span><span class="sxs-lookup"><span data-stu-id="f2ac5-163">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="f2ac5-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2ac5-164">Request</span></span>

<span data-ttu-id="f2ac5-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2ac5-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ac5-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="f2ac5-167">C#</span><span class="sxs-lookup"><span data-stu-id="f2ac5-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2ac5-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2ac5-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2ac5-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2ac5-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2ac5-170">Java</span><span class="sxs-lookup"><span data-stu-id="f2ac5-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f2ac5-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ac5-171">Response</span></span>

<span data-ttu-id="f2ac5-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
  } -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`588`

### <a name="example-4-use-search-and-odata-cast-to-get-transitive-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="f2ac5-173">Пример 4: используйте $search и приведение OData для получения транзитивного членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-173">Example 4: Use $search and OData cast to get transitive membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f2ac5-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2ac5-174">Request</span></span>

<span data-ttu-id="f2ac5-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2ac5-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ac5-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="f2ac5-177">C#</span><span class="sxs-lookup"><span data-stu-id="f2ac5-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2ac5-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2ac5-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2ac5-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2ac5-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2ac5-180">Java</span><span class="sxs-lookup"><span data-stu-id="f2ac5-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f2ac5-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ac5-181">Response</span></span>

<span data-ttu-id="f2ac5-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-182">The following is an example of the response.</span></span>

><span data-ttu-id="f2ac5-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-transitive-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="f2ac5-185">Пример 5: используйте $filter и приведение OData для получения транзитивного членства в группах с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-185">Example 5: Use $filter and OData cast to get transitive membership in groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f2ac5-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2ac5-186">Request</span></span>

<span data-ttu-id="f2ac5-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2ac5-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ac5-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="f2ac5-189">C#</span><span class="sxs-lookup"><span data-stu-id="f2ac5-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2ac5-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2ac5-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2ac5-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2ac5-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2ac5-192">Java</span><span class="sxs-lookup"><span data-stu-id="f2ac5-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f2ac5-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ac5-193">Response</span></span>

<span data-ttu-id="f2ac5-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-194">The following is an example of the response.</span></span>

><span data-ttu-id="f2ac5-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2ac5-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
<!-- {
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
