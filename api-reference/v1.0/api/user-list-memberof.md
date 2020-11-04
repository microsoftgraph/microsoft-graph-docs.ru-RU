---
title: Список memberOf
description: 'Получение групп и ролей каталога, непосредственным участником которых является пользователь. '
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: f0d4c3f45cc45700b64b54a87e5043c1356ea660
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905891"
---
# <a name="list-memberof"></a><span data-ttu-id="1f91e-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="1f91e-103">List memberOf</span></span>

<span data-ttu-id="1f91e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f91e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f91e-105">Получение [групп](../resources/group.md) и [ролей каталога](../resources/directoryrole.md), непосредственным членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="1f91e-105">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1f91e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f91e-106">Permissions</span></span>
<span data-ttu-id="1f91e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f91e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f91e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f91e-109">Permission type</span></span>      | <span data-ttu-id="1f91e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f91e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f91e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f91e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f91e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f91e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1f91e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f91e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f91e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f91e-114">Not supported.</span></span>    |
|<span data-ttu-id="1f91e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f91e-115">Application</span></span> | <span data-ttu-id="1f91e-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f91e-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1f91e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f91e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f91e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f91e-118">Optional query parameters</span></span>

<span data-ttu-id="1f91e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1f91e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="1f91e-120">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="1f91e-120">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="1f91e-121">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="1f91e-121">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="1f91e-122">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="1f91e-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="1f91e-123">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="1f91e-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="1f91e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f91e-124">Request headers</span></span>
| <span data-ttu-id="1f91e-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f91e-125">Header</span></span>       | <span data-ttu-id="1f91e-126">Значение</span><span class="sxs-lookup"><span data-stu-id="1f91e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f91e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f91e-127">Authorization</span></span>  | <span data-ttu-id="1f91e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f91e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f91e-130">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="1f91e-130">ConsistencyLevel</span></span> | <span data-ttu-id="1f91e-131">необязательный.</span><span class="sxs-lookup"><span data-stu-id="1f91e-131">eventual.</span></span> <span data-ttu-id="1f91e-132">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="1f91e-132">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="1f91e-133">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="1f91e-133">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f91e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f91e-134">Request body</span></span>
<span data-ttu-id="1f91e-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f91e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f91e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f91e-136">Response</span></span>

<span data-ttu-id="1f91e-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f91e-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f91e-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f91e-138">Examples</span></span>

### <a name="example-1-get-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="1f91e-139">Пример 1. Получение групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="1f91e-139">Example 1: Get groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="1f91e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f91e-140">Request</span></span>

<span data-ttu-id="1f91e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f91e-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f91e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f91e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="1f91e-143">C#</span><span class="sxs-lookup"><span data-stu-id="1f91e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f91e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f91e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f91e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f91e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f91e-146">Java</span><span class="sxs-lookup"><span data-stu-id="1f91e-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f91e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f91e-147">Response</span></span>

<span data-ttu-id="1f91e-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f91e-148">The following is an example of the response.</span></span>

><span data-ttu-id="1f91e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f91e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-groups-directory-roles-and-administrative-units-that-the-user-is-a-direct-member-of"></a><span data-ttu-id="1f91e-151">Пример 2. Получение только количества всех групп, ролей каталогов и административных единиц, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="1f91e-151">Example 2: Get only a count of all groups, directory roles, and administrative units that the user is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="1f91e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f91e-152">Request</span></span>

<span data-ttu-id="1f91e-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f91e-153">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f91e-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f91e-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_memberof_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1f91e-155">C#</span><span class="sxs-lookup"><span data-stu-id="1f91e-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-memberof-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f91e-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f91e-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-memberof-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f91e-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f91e-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-memberof-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f91e-158">Java</span><span class="sxs-lookup"><span data-stu-id="1f91e-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-memberof-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f91e-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f91e-159">Response</span></span>

<span data-ttu-id="1f91e-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f91e-160">The following is an example of the response.</span></span>

><span data-ttu-id="1f91e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f91e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="1f91e-163">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="1f91e-163">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="1f91e-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f91e-164">Request</span></span>

<span data-ttu-id="1f91e-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f91e-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f91e-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f91e-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1f91e-167">C#</span><span class="sxs-lookup"><span data-stu-id="1f91e-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f91e-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f91e-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f91e-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f91e-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f91e-170">Java</span><span class="sxs-lookup"><span data-stu-id="1f91e-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f91e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f91e-171">Response</span></span>

<span data-ttu-id="1f91e-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f91e-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-4-use-search-and-odata-cast-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="1f91e-173">Пример 4. Использование параметра $search и приведения к OData для получения участия пользователей в группах с отображаемыми именами, содержащими буквы «tier», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="1f91e-173">Example 4: Use $search and OData cast to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1f91e-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f91e-174">Request</span></span>

<span data-ttu-id="1f91e-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f91e-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f91e-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f91e-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1f91e-177">C#</span><span class="sxs-lookup"><span data-stu-id="1f91e-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f91e-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f91e-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f91e-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f91e-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f91e-180">Java</span><span class="sxs-lookup"><span data-stu-id="1f91e-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f91e-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f91e-181">Response</span></span>

<span data-ttu-id="1f91e-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f91e-182">The following is an example of the response.</span></span>

><span data-ttu-id="1f91e-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f91e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="1f91e-185">Пример 5. Использование параметра $filter и приведения к OData для получения групп с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="1f91e-185">Example 5: Use $filter and OData cast to get groups with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="1f91e-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f91e-186">Request</span></span>

<span data-ttu-id="1f91e-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f91e-187">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1f91e-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f91e-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a') 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="1f91e-189">C#</span><span class="sxs-lookup"><span data-stu-id="1f91e-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f91e-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f91e-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f91e-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f91e-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f91e-192">Java</span><span class="sxs-lookup"><span data-stu-id="1f91e-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f91e-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f91e-193">Response</span></span>

<span data-ttu-id="1f91e-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f91e-194">The following is an example of the response.</span></span>

><span data-ttu-id="1f91e-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f91e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
