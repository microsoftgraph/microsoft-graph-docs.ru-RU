---
title: Список riskyUsers
description: Получение свойств и связей коллекции объектов **рискюсер** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ee16244a6910799fbfdc02ee97a6fcaeeb5d9a5e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410831"
---
# <a name="list-riskyusers"></a><span data-ttu-id="400c3-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="400c3-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="400c3-104">Получение свойств и связей коллекции объектов **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="400c3-104">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="400c3-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="400c3-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="400c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="400c3-106">Permissions</span></span>
<span data-ttu-id="400c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="400c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="400c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="400c3-109">Permission type</span></span>      | <span data-ttu-id="400c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="400c3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="400c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="400c3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="400c3-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="400c3-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="400c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="400c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="400c3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="400c3-114">Not supported.</span></span>    |
|<span data-ttu-id="400c3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="400c3-115">Application</span></span> | <span data-ttu-id="400c3-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="400c3-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="400c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="400c3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="400c3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="400c3-118">Optional query parameters</span></span>
<span data-ttu-id="400c3-119">Этот метод поддерживает `$filter` настройку ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="400c3-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="400c3-120">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="400c3-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="400c3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="400c3-121">Request headers</span></span>
| <span data-ttu-id="400c3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="400c3-122">Name</span></span>      |<span data-ttu-id="400c3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="400c3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="400c3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="400c3-124">Authorization</span></span>  | <span data-ttu-id="400c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="400c3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="400c3-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="400c3-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="400c3-128">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="400c3-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="400c3-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="400c3-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="400c3-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="400c3-130">Request body</span></span>
<span data-ttu-id="400c3-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="400c3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="400c3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="400c3-132">Response</span></span>
<span data-ttu-id="400c3-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="400c3-133">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="400c3-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="400c3-134">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="400c3-135">Пример 1: список рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="400c3-135">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="400c3-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="400c3-136">Request</span></span>
<span data-ttu-id="400c3-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="400c3-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="400c3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="400c3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="400c3-139">C#</span><span class="sxs-lookup"><span data-stu-id="400c3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="400c3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="400c3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="400c3-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="400c3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="400c3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="400c3-142">Response</span></span>
<span data-ttu-id="400c3-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="400c3-143">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="400c3-144">Пример 2: список рискованных пользователей и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="400c3-144">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="400c3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="400c3-145">Request</span></span>
<span data-ttu-id="400c3-146">В приведенном ниже примере показано, `$filter` как получить коллекцию рискюсер с уровнем агрегированного риска среднего размера.</span><span class="sxs-lookup"><span data-stu-id="400c3-146">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="400c3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="400c3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="400c3-148">C#</span><span class="sxs-lookup"><span data-stu-id="400c3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="400c3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="400c3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="400c3-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="400c3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="400c3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="400c3-151">Response</span></span>
<span data-ttu-id="400c3-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="400c3-152">Here is an example of the response.</span></span>
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
