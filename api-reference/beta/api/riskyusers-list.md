---
title: Список riskyUsers
description: Извлечение свойств и связей коллекции объектов **riskyUser.**
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: d0ab9e55f6274f048d6fe25dd9f731c91dd182ad
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440781"
---
# <a name="list-riskyusers"></a><span data-ttu-id="dd0bc-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="dd0bc-103">List riskyUsers</span></span>

<span data-ttu-id="dd0bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd0bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd0bc-105">Извлечение свойств и связей коллекции объектов **riskyUser.**</span><span class="sxs-lookup"><span data-stu-id="dd0bc-105">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="dd0bc-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd0bc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd0bc-107">Permissions</span></span>
<span data-ttu-id="dd0bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd0bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd0bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd0bc-110">Permission type</span></span>      | <span data-ttu-id="dd0bc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd0bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd0bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd0bc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dd0bc-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0bc-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="dd0bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd0bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd0bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-115">Not supported.</span></span>    |
|<span data-ttu-id="dd0bc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd0bc-116">Application</span></span> | <span data-ttu-id="dd0bc-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0bc-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd0bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd0bc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
GET /identityProtection/riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd0bc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd0bc-119">Optional query parameters</span></span>
<span data-ttu-id="dd0bc-120">Этот метод поддерживает `$filter` настройку ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="dd0bc-121">Пример см. в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="dd0bc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd0bc-122">Request headers</span></span>
| <span data-ttu-id="dd0bc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dd0bc-123">Name</span></span>      |<span data-ttu-id="dd0bc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dd0bc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd0bc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd0bc-125">Authorization</span></span>  | <span data-ttu-id="dd0bc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd0bc-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dd0bc-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="dd0bc-129">ID сеанса книги, определяя, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-129">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="dd0bc-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd0bc-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd0bc-131">Request body</span></span>
<span data-ttu-id="dd0bc-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd0bc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0bc-133">Response</span></span>
<span data-ttu-id="dd0bc-134">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [riskyUser](../resources/riskyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-134">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd0bc-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd0bc-135">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="dd0bc-136">Пример 1. Список рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="dd0bc-136">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="dd0bc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd0bc-137">Request</span></span>
<span data-ttu-id="dd0bc-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd0bc-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd0bc-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="dd0bc-140">C#</span><span class="sxs-lookup"><span data-stu-id="dd0bc-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd0bc-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd0bc-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd0bc-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd0bc-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd0bc-143">Java</span><span class="sxs-lookup"><span data-stu-id="dd0bc-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="dd0bc-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0bc-144">Response</span></span>
<span data-ttu-id="dd0bc-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
            "isProcessing": true,
            "isDeleted": true,
            "riskDetail": "adminConfirmedSigninCompromised",
            "riskLevel": "high",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com"
        }
    ]
}
```

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="dd0bc-146">Пример 2. Список рискованных пользователей и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="dd0bc-146">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="dd0bc-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd0bc-147">Request</span></span>
<span data-ttu-id="dd0bc-148">В следующем примере показано, как использовать для получения коллекции riskyUser, совокупный уровень риска которого `$filter` средний.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-148">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="http"></a>[<span data-ttu-id="dd0bc-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd0bc-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="c"></a>[<span data-ttu-id="dd0bc-150">C#</span><span class="sxs-lookup"><span data-stu-id="dd0bc-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd0bc-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd0bc-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd0bc-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd0bc-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd0bc-153">Java</span><span class="sxs-lookup"><span data-stu-id="dd0bc-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dd0bc-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0bc-154">Response</span></span>
<span data-ttu-id="dd0bc-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd0bc-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
            "isProcessing": true,
            "isDeleted": false,
            "riskDetail": "none",
            "riskLevel": "medium",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


