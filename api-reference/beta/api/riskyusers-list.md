---
title: Список riskyUsers
description: Получение свойств и связей коллекции объектов **рискюсер** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb29c5845c8243a046a563351d4b1e486d38c029
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358204"
---
# <a name="list-riskyusers"></a><span data-ttu-id="84cdf-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="84cdf-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84cdf-104">Получение свойств и связей коллекции объектов **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="84cdf-104">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="84cdf-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="84cdf-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="84cdf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84cdf-106">Permissions</span></span>
<span data-ttu-id="84cdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84cdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84cdf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84cdf-109">Permission type</span></span>      | <span data-ttu-id="84cdf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84cdf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84cdf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84cdf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84cdf-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="84cdf-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="84cdf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84cdf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84cdf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84cdf-114">Not supported.</span></span>    |
|<span data-ttu-id="84cdf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84cdf-115">Application</span></span> | <span data-ttu-id="84cdf-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="84cdf-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84cdf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84cdf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84cdf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84cdf-118">Optional query parameters</span></span>
<span data-ttu-id="84cdf-119">Этот метод поддерживает `$filter` настройку ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="84cdf-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="84cdf-120">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="84cdf-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="84cdf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84cdf-121">Request headers</span></span>
| <span data-ttu-id="84cdf-122">Имя</span><span class="sxs-lookup"><span data-stu-id="84cdf-122">Name</span></span>      |<span data-ttu-id="84cdf-123">Описание</span><span class="sxs-lookup"><span data-stu-id="84cdf-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84cdf-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84cdf-124">Authorization</span></span>  | <span data-ttu-id="84cdf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84cdf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84cdf-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="84cdf-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="84cdf-128">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="84cdf-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="84cdf-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="84cdf-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84cdf-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84cdf-130">Request body</span></span>
<span data-ttu-id="84cdf-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84cdf-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84cdf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="84cdf-132">Response</span></span>
<span data-ttu-id="84cdf-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84cdf-133">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84cdf-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="84cdf-134">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="84cdf-135">Пример 1: список рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="84cdf-135">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="84cdf-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="84cdf-136">Request</span></span>
<span data-ttu-id="84cdf-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84cdf-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84cdf-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="84cdf-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84cdf-139">C#</span><span class="sxs-lookup"><span data-stu-id="84cdf-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84cdf-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84cdf-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84cdf-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84cdf-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="84cdf-142">Java</span><span class="sxs-lookup"><span data-stu-id="84cdf-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="84cdf-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="84cdf-143">Response</span></span>
<span data-ttu-id="84cdf-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84cdf-144">Here is an example of the response.</span></span>
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
            "isGuest": true,
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="84cdf-145">Пример 2: список рискованных пользователей и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="84cdf-145">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="84cdf-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="84cdf-146">Request</span></span>
<span data-ttu-id="84cdf-147">В приведенном ниже примере показано, `$filter` как получить коллекцию рискюсер с уровнем агрегированного риска среднего размера.</span><span class="sxs-lookup"><span data-stu-id="84cdf-147">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="84cdf-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="84cdf-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84cdf-149">C#</span><span class="sxs-lookup"><span data-stu-id="84cdf-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84cdf-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84cdf-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84cdf-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84cdf-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="84cdf-152">Java</span><span class="sxs-lookup"><span data-stu-id="84cdf-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84cdf-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="84cdf-153">Response</span></span>
<span data-ttu-id="84cdf-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84cdf-154">Here is an example of the response.</span></span>
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
            "isGuest": false,
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
