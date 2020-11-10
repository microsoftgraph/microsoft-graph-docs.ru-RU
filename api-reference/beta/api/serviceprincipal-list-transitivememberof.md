---
title: Перечисление servicePrincipal transitive memberOf
description: Список групп и ролей каталога, участником которых является этот субъект-служба.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 314d36c467fc5215706cbeb763353c6e03acd154
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973657"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="8a0bd-103">Перечисление servicePrincipal transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="8a0bd-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="8a0bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a0bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a0bd-105">Список групп и ролей каталога, участником которых является этот [субъект-служба](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="8a0bd-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="8a0bd-106">Эта операция является транзитивной и включает все группы, в которых состоит субъект-служба.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a0bd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a0bd-107">Permissions</span></span>
<span data-ttu-id="8a0bd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a0bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a0bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a0bd-110">Permission type</span></span>      | <span data-ttu-id="8a0bd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a0bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a0bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a0bd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a0bd-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a0bd-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8a0bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a0bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a0bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-115">Not supported.</span></span>    |
|<span data-ttu-id="8a0bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a0bd-116">Application</span></span> | <span data-ttu-id="8a0bd-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a0bd-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8a0bd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a0bd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a0bd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8a0bd-119">Optional query parameters</span></span>
<span data-ttu-id="8a0bd-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="8a0bd-121">Кроме того, включено также приведение к OData, например, вы можете получить только directoryRoles, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="8a0bd-122">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="8a0bd-123">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="8a0bd-124">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a0bd-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a0bd-125">Request headers</span></span>

| <span data-ttu-id="8a0bd-126">Имя</span><span class="sxs-lookup"><span data-stu-id="8a0bd-126">Name</span></span>       | <span data-ttu-id="8a0bd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0bd-127">Type</span></span> | <span data-ttu-id="8a0bd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0bd-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8a0bd-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a0bd-129">Authorization</span></span>  | <span data-ttu-id="8a0bd-130">string</span><span class="sxs-lookup"><span data-stu-id="8a0bd-130">string</span></span>  | <span data-ttu-id="8a0bd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a0bd-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="8a0bd-133">ConsistencyLevel</span></span> | <span data-ttu-id="8a0bd-134">необязательный.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-134">eventual.</span></span> <span data-ttu-id="8a0bd-135">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="8a0bd-136">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a0bd-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a0bd-137">Request body</span></span>
<span data-ttu-id="8a0bd-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a0bd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a0bd-139">Response</span></span>

<span data-ttu-id="8a0bd-140">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-140">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a0bd-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="8a0bd-141">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="8a0bd-142">Пример 1: Список групп и ролей каталога, транзитивным участником которых является этот субъект-служба</span><span class="sxs-lookup"><span data-stu-id="8a0bd-142">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="8a0bd-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a0bd-143">Request</span></span>

<span data-ttu-id="8a0bd-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a0bd-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0bd-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="8a0bd-146">C#</span><span class="sxs-lookup"><span data-stu-id="8a0bd-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a0bd-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a0bd-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a0bd-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a0bd-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a0bd-149">Java</span><span class="sxs-lookup"><span data-stu-id="8a0bd-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-tranitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a0bd-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a0bd-150">Response</span></span>

<span data-ttu-id="8a0bd-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-151">The following is an example of the response.</span></span> 
> <span data-ttu-id="8a0bd-152">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-152">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8a0bd-153">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-153">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="8a0bd-154">Пример 2: Получение только количества транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="8a0bd-154">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="8a0bd-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a0bd-155">Request</span></span>

<span data-ttu-id="8a0bd-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a0bd-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0bd-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8a0bd-158">C#</span><span class="sxs-lookup"><span data-stu-id="8a0bd-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a0bd-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a0bd-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a0bd-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a0bd-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a0bd-161">Java</span><span class="sxs-lookup"><span data-stu-id="8a0bd-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a0bd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a0bd-162">Response</span></span>

<span data-ttu-id="8a0bd-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="8a0bd-164">294</span><span class="sxs-lookup"><span data-stu-id="8a0bd-164">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="8a0bd-165">Пример 3. Использование OData cast для получения только количества транзитивных участников в группах</span><span class="sxs-lookup"><span data-stu-id="8a0bd-165">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="8a0bd-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a0bd-166">Request</span></span>

<span data-ttu-id="8a0bd-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a0bd-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0bd-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8a0bd-169">C#</span><span class="sxs-lookup"><span data-stu-id="8a0bd-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a0bd-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a0bd-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a0bd-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a0bd-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a0bd-172">Java</span><span class="sxs-lookup"><span data-stu-id="8a0bd-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a0bd-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a0bd-173">Response</span></span>

<span data-ttu-id="8a0bd-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="8a0bd-175">294</span><span class="sxs-lookup"><span data-stu-id="8a0bd-175">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="8a0bd-176">Пример 4: Использование параметра $search и OData cast для получения участия в группах с отображаемыми именами, содержащими буквы "Video", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="8a0bd-176">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8a0bd-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a0bd-177">Request</span></span>

<span data-ttu-id="8a0bd-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-178">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a0bd-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0bd-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8a0bd-180">C#</span><span class="sxs-lookup"><span data-stu-id="8a0bd-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a0bd-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a0bd-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a0bd-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a0bd-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a0bd-183">Java</span><span class="sxs-lookup"><span data-stu-id="8a0bd-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tier-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a0bd-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a0bd-184">Response</span></span>

<span data-ttu-id="8a0bd-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-185">The following is an example of the response.</span></span>
><span data-ttu-id="8a0bd-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="8a0bd-188">Пример 5: Использование параметра $search и OData cast для получения участия в группах с отображаемым именем, которое начинается на «а», включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="8a0bd-188">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8a0bd-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a0bd-189">Request</span></span>

<span data-ttu-id="8a0bd-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-190">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a0bd-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a0bd-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="8a0bd-192">C#</span><span class="sxs-lookup"><span data-stu-id="8a0bd-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a0bd-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a0bd-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a0bd-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a0bd-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a0bd-195">Java</span><span class="sxs-lookup"><span data-stu-id="8a0bd-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a0bd-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a0bd-196">Response</span></span>

<span data-ttu-id="8a0bd-197">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-197">The following is an example of the response.</span></span>
><span data-ttu-id="8a0bd-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a0bd-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


