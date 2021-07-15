---
title: Перечисление servicePrincipals
description: Получение списка объектов servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 595c7e9ee58fc2186fb1f29ccfe5f413cd36b7d5
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430286"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="62524-103">Перечисление servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="62524-103">List servicePrincipals</span></span>

<span data-ttu-id="62524-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62524-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62524-105">Получение списка объектов [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="62524-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="62524-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62524-106">Permissions</span></span>

<span data-ttu-id="62524-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62524-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62524-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62524-109">Permission type</span></span> | <span data-ttu-id="62524-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62524-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="62524-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62524-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62524-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62524-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="62524-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62524-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62524-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62524-114">Not supported.</span></span> |
| <span data-ttu-id="62524-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62524-115">Application</span></span> | <span data-ttu-id="62524-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="62524-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62524-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62524-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62524-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62524-118">Optional query parameters</span></span>

<span data-ttu-id="62524-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select` и `$top` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="62524-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="62524-120">Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`.</span><span class="sxs-lookup"><span data-stu-id="62524-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="62524-121">Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="62524-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="62524-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62524-122">Request headers</span></span>

| <span data-ttu-id="62524-123">Имя</span><span class="sxs-lookup"><span data-stu-id="62524-123">Name</span></span> | <span data-ttu-id="62524-124">Описание</span><span class="sxs-lookup"><span data-stu-id="62524-124">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="62524-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62524-125">Authorization</span></span> | <span data-ttu-id="62524-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62524-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62524-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="62524-128">ConsistencyLevel</span></span> | <span data-ttu-id="62524-129">необязательный.</span><span class="sxs-lookup"><span data-stu-id="62524-129">eventual.</span></span> <span data-ttu-id="62524-130">Этот заголовок и `$count` требуются при использовании `$search` или определенном использовании `$filter`.</span><span class="sxs-lookup"><span data-stu-id="62524-130">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="62524-131">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="62524-131">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="62524-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62524-132">Request body</span></span>

<span data-ttu-id="62524-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62524-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62524-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="62524-134">Response</span></span>

<span data-ttu-id="62524-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62524-135">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62524-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="62524-136">Examples</span></span>

### <a name="example-1-get-a-list-of-service-principals"></a><span data-ttu-id="62524-137">Пример 1. Получение списка субъект-служб</span><span class="sxs-lookup"><span data-stu-id="62524-137">Example 1: Get a list of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="62524-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="62524-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="62524-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="62524-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="62524-140">C#</span><span class="sxs-lookup"><span data-stu-id="62524-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62524-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62524-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62524-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62524-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62524-143">Java</span><span class="sxs-lookup"><span data-stu-id="62524-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62524-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="62524-144">Response</span></span>

<span data-ttu-id="62524-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="62524-145">The following is an example of the response.</span></span>
><span data-ttu-id="62524-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62524-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "displayName":"amasf",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-service-principals"></a><span data-ttu-id="62524-147">Пример 2. Получение только количества субъект-служб</span><span class="sxs-lookup"><span data-stu-id="62524-147">Example 2: Get only a count of service principals</span></span>

#### <a name="request"></a><span data-ttu-id="62524-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="62524-148">Request</span></span>

<span data-ttu-id="62524-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62524-149">The following is an example of the request.</span></span> <span data-ttu-id="62524-150">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$count`.</span><span class="sxs-lookup"><span data-stu-id="62524-150">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="62524-151">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="62524-151">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="62524-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="62524-152">Response</span></span>

<span data-ttu-id="62524-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="62524-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```

### <a name="example-3-use-filter-and-top-to-get-one-service-principal-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="62524-154">Пример 3. Использование параметров $filter и $top для получения субъект-службы с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="62524-154">Example 3: Use $filter and $top to get one service principal with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="62524-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="62524-155">Request</span></span>

<span data-ttu-id="62524-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62524-156">The following is an example of the request.</span></span> <span data-ttu-id="62524-157">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`.</span><span class="sxs-lookup"><span data-stu-id="62524-157">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="62524-158">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="62524-158">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="62524-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="62524-159">Response</span></span>

<span data-ttu-id="62524-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="62524-160">The following is an example of the response.</span></span>
><span data-ttu-id="62524-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62524-161">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrinciples",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"a",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-service-principals-with-display-names-that-contain-the-letters-team-including-a-count-of-returned-objects"></a><span data-ttu-id="62524-162">Пример 4. Использование параметра $search для получения субъект-служб с отображаемыми именами, содержащими буквы "Team", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="62524-162">Example 4: Use $search to get service principals with display names that contain the letters 'Team' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="62524-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="62524-163">Request</span></span>

<span data-ttu-id="62524-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62524-164">The following is an example of the request.</span></span> <span data-ttu-id="62524-165">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$search` и строка запроса `$count=true`.</span><span class="sxs-lookup"><span data-stu-id="62524-165">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="62524-166">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="62524-166">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals?$search="displayName:Team"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="62524-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="62524-167">Response</span></span>

<span data-ttu-id="62524-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="62524-168">The following is an example of the response.</span></span>
><span data-ttu-id="62524-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62524-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "displayName":"myContosoTeam",
      "publisherName":"Contoso",
      "servicePrincipalType":"Application",
      "signInAudience":"AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



