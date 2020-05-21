---
title: Перечисление транзитивных servicePrincipal memberOf
description: Получение групп и ролей каталогов, членом которых является данный участник службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: fa3885224c44294d147fbf0ca15ce23492c4ee1b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336801"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="c35b6-103">Перечисление транзитивных servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="c35b6-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="c35b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c35b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c35b6-105">Получение групп и ролей каталогов, участником которых является данный [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="c35b6-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="c35b6-106">Эта операция является транзитивным и включает все группы, вложенные в состав участника службы.</span><span class="sxs-lookup"><span data-stu-id="c35b6-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="c35b6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c35b6-107">Permissions</span></span>
<span data-ttu-id="c35b6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c35b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c35b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c35b6-110">Permission type</span></span>      | <span data-ttu-id="c35b6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c35b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c35b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c35b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c35b6-113">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c35b6-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c35b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c35b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c35b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c35b6-115">Not supported.</span></span>    |
|<span data-ttu-id="c35b6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c35b6-116">Application</span></span> | <span data-ttu-id="c35b6-117">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c35b6-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c35b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c35b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c35b6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c35b6-119">Optional query parameters</span></span>
<span data-ttu-id="c35b6-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="c35b6-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="c35b6-121">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только перечисление directoryrole, членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="c35b6-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="c35b6-122">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="c35b6-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="c35b6-123">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="c35b6-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="c35b6-124">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="c35b6-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c35b6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c35b6-125">Request headers</span></span>

| <span data-ttu-id="c35b6-126">Имя</span><span class="sxs-lookup"><span data-stu-id="c35b6-126">Name</span></span>       | <span data-ttu-id="c35b6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c35b6-127">Type</span></span> | <span data-ttu-id="c35b6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c35b6-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c35b6-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c35b6-129">Authorization</span></span>  | <span data-ttu-id="c35b6-130">string</span><span class="sxs-lookup"><span data-stu-id="c35b6-130">string</span></span>  | <span data-ttu-id="c35b6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c35b6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c35b6-133">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="c35b6-133">ConsistencyLevel</span></span> | <span data-ttu-id="c35b6-134">закончить.</span><span class="sxs-lookup"><span data-stu-id="c35b6-134">eventual.</span></span> <span data-ttu-id="c35b6-135">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="c35b6-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="c35b6-136">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="c35b6-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c35b6-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c35b6-137">Request body</span></span>
<span data-ttu-id="c35b6-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c35b6-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c35b6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c35b6-139">Response</span></span>

<span data-ttu-id="c35b6-140">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c35b6-140">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c35b6-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="c35b6-141">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="c35b6-142">Пример 1: получение групп и ролей каталогов, членом которых является транзитивное участник службы</span><span class="sxs-lookup"><span data-stu-id="c35b6-142">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="c35b6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c35b6-143">Request</span></span>

<span data-ttu-id="c35b6-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c35b6-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c35b6-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c35b6-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="c35b6-146">C#</span><span class="sxs-lookup"><span data-stu-id="c35b6-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c35b6-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c35b6-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c35b6-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c35b6-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c35b6-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c35b6-149">Response</span></span>

<span data-ttu-id="c35b6-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c35b6-150">The following is an example of the response.</span></span> 
> <span data-ttu-id="c35b6-151">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c35b6-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c35b6-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c35b6-152">All of the properties will be returned from an actual call.</span></span>

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
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="c35b6-153">Пример 2: получение только количества всех транзитивных членств</span><span class="sxs-lookup"><span data-stu-id="c35b6-153">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="c35b6-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="c35b6-154">Request</span></span>

<span data-ttu-id="c35b6-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c35b6-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c35b6-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="c35b6-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c35b6-157">C#</span><span class="sxs-lookup"><span data-stu-id="c35b6-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c35b6-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c35b6-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c35b6-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c35b6-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c35b6-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c35b6-160">Response</span></span>

<span data-ttu-id="c35b6-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c35b6-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="c35b6-162">294</span><span class="sxs-lookup"><span data-stu-id="c35b6-162">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="c35b6-163">Пример 3: Использование приведения OData для получения только счетчика транзитивного членства в группах</span><span class="sxs-lookup"><span data-stu-id="c35b6-163">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="c35b6-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="c35b6-164">Request</span></span>

<span data-ttu-id="c35b6-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c35b6-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c35b6-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="c35b6-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c35b6-167">C#</span><span class="sxs-lookup"><span data-stu-id="c35b6-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c35b6-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c35b6-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c35b6-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c35b6-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c35b6-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="c35b6-170">Response</span></span>

<span data-ttu-id="c35b6-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c35b6-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="c35b6-172">294</span><span class="sxs-lookup"><span data-stu-id="c35b6-172">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="c35b6-173">Пример 4: использование $search и функции OData для получения сведений о членстве в группах с отображаемыми именами, содержащими "видео", в том числе от числа возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="c35b6-173">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c35b6-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="c35b6-174">Request</span></span>

<span data-ttu-id="c35b6-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c35b6-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c35b6-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="c35b6-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="c35b6-177">C#</span><span class="sxs-lookup"><span data-stu-id="c35b6-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c35b6-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c35b6-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c35b6-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c35b6-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c35b6-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="c35b6-180">Response</span></span>

<span data-ttu-id="c35b6-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c35b6-181">The following is an example of the response.</span></span>
><span data-ttu-id="c35b6-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c35b6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c35b6-184">Пример 5: используйте $filter и приведение OData для получения сведений о членстве в группах с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="c35b6-184">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c35b6-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="c35b6-185">Request</span></span>

<span data-ttu-id="c35b6-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c35b6-186">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c35b6-187">Ответ</span><span class="sxs-lookup"><span data-stu-id="c35b6-187">Response</span></span>

<span data-ttu-id="c35b6-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c35b6-188">The following is an example of the response.</span></span>
><span data-ttu-id="c35b6-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c35b6-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List servicePrincipal transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
