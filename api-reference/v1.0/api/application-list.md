---
title: Список приложений
description: Получение списка приложений в организации.
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 28eca7aee974f8fc60f4c6bd5db211429e3cde61
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430245"
---
# <a name="list-applications"></a><span data-ttu-id="8dec7-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="8dec7-103">List applications</span></span>

<span data-ttu-id="8dec7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dec7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8dec7-105">Получение списка [приложений](../resources/application.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="8dec7-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

> [!NOTE]
> <span data-ttu-id="8dec7-106">При вызове этого API с использованием маркеров, выпущенных для личной учетной записи Майкрософт, возвращаются приложения, принадлежащие личной учетной записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8dec7-106">When calling this API using tokens issued for a personal Microsoft account, it will return the apps owned by the personal Microsoft account.</span></span> <span data-ttu-id="8dec7-107">Для личных учетных записей Майкрософт не существует понятия организаций.</span><span class="sxs-lookup"><span data-stu-id="8dec7-107">The notion of organizations doesn't exist for personal Microsoft accounts.</span></span> <span data-ttu-id="8dec7-108">Чтобы составить список приложений, принадлежащих определенным личным учетным записям Майкрософт, для этого API помимо Application.Read.All или Application.ReadWrite.All требуется разрешение User.Read.</span><span class="sxs-lookup"><span data-stu-id="8dec7-108">In order to list applications owned by specific personal Microsoft accounts, this API requires User.Read permission in addition to Application.Read.All or Application.ReadWrite.All.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dec7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8dec7-109">Permissions</span></span>
<span data-ttu-id="8dec7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dec7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8dec7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dec7-112">Permission type</span></span>      | <span data-ttu-id="8dec7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dec7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dec7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dec7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8dec7-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8dec7-115">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8dec7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dec7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dec7-117">Application.Read.All и User.Read, Application.ReadWrite.All и User.Read</span><span class="sxs-lookup"><span data-stu-id="8dec7-117">Application.Read.All and User.Read, Application.ReadWrite.All and User.Read</span></span> |
|<span data-ttu-id="8dec7-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="8dec7-118">Application</span></span> | <span data-ttu-id="8dec7-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dec7-119">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dec7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dec7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8dec7-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8dec7-121">Optional query parameters</span></span>

<span data-ttu-id="8dec7-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select` и `$top` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8dec7-122">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="8dec7-123">Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`.</span><span class="sxs-lookup"><span data-stu-id="8dec7-123">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="8dec7-124">Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8dec7-124">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8dec7-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dec7-125">Request headers</span></span>

| <span data-ttu-id="8dec7-126">Имя</span><span class="sxs-lookup"><span data-stu-id="8dec7-126">Name</span></span>           | <span data-ttu-id="8dec7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8dec7-127">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="8dec7-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dec7-128">Authorization</span></span>  | <span data-ttu-id="8dec7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dec7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8dec7-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="8dec7-131">ConsistencyLevel</span></span> | <span data-ttu-id="8dec7-132">необязательный.</span><span class="sxs-lookup"><span data-stu-id="8dec7-132">eventual.</span></span> <span data-ttu-id="8dec7-133">Этот заголовок и `$count` требуются при использовании `$search` или определенном использовании `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8dec7-133">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="8dec7-134">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8dec7-134">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dec7-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dec7-135">Request body</span></span>
<span data-ttu-id="8dec7-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8dec7-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dec7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dec7-137">Response</span></span>

<span data-ttu-id="8dec7-138">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8dec7-138">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8dec7-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="8dec7-139">Examples</span></span>

### <a name="example-1-get-the-list-of-applications"></a><span data-ttu-id="8dec7-140">Пример 1: получение списка приложений</span><span class="sxs-lookup"><span data-stu-id="8dec7-140">Example 1: Get the list of applications</span></span>

#### <a name="request"></a><span data-ttu-id="8dec7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dec7-141">Request</span></span>

<span data-ttu-id="8dec7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dec7-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8dec7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dec7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications
```
# <a name="c"></a>[<span data-ttu-id="8dec7-144">C#</span><span class="sxs-lookup"><span data-stu-id="8dec7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8dec7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dec7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8dec7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dec7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8dec7-147">Java</span><span class="sxs-lookup"><span data-stu-id="8dec7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8dec7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dec7-148">Response</span></span>

<span data-ttu-id="8dec7-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8dec7-149">Here is an example of the response.</span></span>

> <span data-ttu-id="8dec7-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8dec7-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications",
  "value": [
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName": "My app",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-applications"></a><span data-ttu-id="8dec7-151">Пример 2: получение только количества приложений</span><span class="sxs-lookup"><span data-stu-id="8dec7-151">Example 2: Get only a count of applications</span></span>

#### <a name="request"></a><span data-ttu-id="8dec7-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dec7-152">Request</span></span>

<span data-ttu-id="8dec7-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dec7-153">The following is an example of the request.</span></span> <span data-ttu-id="8dec7-154">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$count`.</span><span class="sxs-lookup"><span data-stu-id="8dec7-154">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="8dec7-155">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8dec7-155">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8dec7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dec7-156">Response</span></span>

<span data-ttu-id="8dec7-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8dec7-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-3-use-filter-and-top-to-get-one-application-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="8dec7-158">Пример 3: использование параметров $filter и $top для получения одного приложения с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="8dec7-158">Example 3: Use $filter and $top to get one application with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8dec7-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dec7-159">Request</span></span>

<span data-ttu-id="8dec7-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dec7-160">The following is an example of the request.</span></span> <span data-ttu-id="8dec7-161">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8dec7-161">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="8dec7-162">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8dec7-162">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8dec7-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dec7-163">Response</span></span>

<span data-ttu-id="8dec7-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8dec7-164">The following is an example of the response.</span></span>

><span data-ttu-id="8dec7-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8dec7-165">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.count":1,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"a",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-applications-with-display-names-that-contain-the-letters-web-including-a-count-of-returned-objects"></a><span data-ttu-id="8dec7-166">Пример 4: использование параметра $search для получения приложений с отображаемыми именами, содержащими буквы "Web", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="8dec7-166">Example 4: Use $search to get applications with display names that contain the letters 'Web' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8dec7-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dec7-167">Request</span></span>

<span data-ttu-id="8dec7-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dec7-168">The following is an example of the request.</span></span> <span data-ttu-id="8dec7-169">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$search` и строка запроса `$count=true`.</span><span class="sxs-lookup"><span data-stu-id="8dec7-169">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="8dec7-170">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8dec7-170">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_web_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications?$search="displayName:Web"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8dec7-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dec7-171">Response</span></span>

<span data-ttu-id="8dec7-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8dec7-172">The following is an example of the response.</span></span>

><span data-ttu-id="8dec7-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8dec7-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#applications",
  "@odata.count":1396,
  "value":[
    {
      "appId": "00000000-0000-0000-0000-000000000000",
      "identifierUris": [ "http://contoso/" ],
      "displayName":"'DotNetWeb-App' ",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
