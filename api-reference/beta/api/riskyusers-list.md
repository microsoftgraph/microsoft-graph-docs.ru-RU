---
title: Список riskyUsers
description: Получение свойств и связей коллекции объектов **рискюсер** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3bda35a6855dfbcb6da086cfa67c4e51def40a5d
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863504"
---
# <a name="list-riskyusers"></a><span data-ttu-id="023f0-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="023f0-103">List riskyUsers</span></span>

<span data-ttu-id="023f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="023f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="023f0-105">Получение свойств и связей коллекции объектов **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="023f0-105">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="023f0-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="023f0-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="023f0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="023f0-107">Permissions</span></span>
<span data-ttu-id="023f0-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="023f0-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="023f0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="023f0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="023f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="023f0-110">Permission type</span></span>      | <span data-ttu-id="023f0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="023f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="023f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="023f0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="023f0-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="023f0-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="023f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="023f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="023f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="023f0-115">Not supported.</span></span>    |
|<span data-ttu-id="023f0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="023f0-116">Application</span></span> | <span data-ttu-id="023f0-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="023f0-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="023f0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="023f0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
GET /identityProtection/riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="023f0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="023f0-119">Optional query parameters</span></span>
<span data-ttu-id="023f0-120">Этот метод поддерживает `$filter` настройку ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="023f0-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="023f0-121">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="023f0-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="023f0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="023f0-122">Request headers</span></span>
| <span data-ttu-id="023f0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="023f0-123">Name</span></span>      |<span data-ttu-id="023f0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="023f0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="023f0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="023f0-125">Authorization</span></span>  | <span data-ttu-id="023f0-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="023f0-126">Bearer {token}.</span></span> <span data-ttu-id="023f0-127">Required.</span><span class="sxs-lookup"><span data-stu-id="023f0-127">Required.</span></span> |
| <span data-ttu-id="023f0-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="023f0-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="023f0-129">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="023f0-129">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="023f0-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="023f0-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="023f0-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="023f0-131">Request body</span></span>
<span data-ttu-id="023f0-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="023f0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="023f0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="023f0-133">Response</span></span>
<span data-ttu-id="023f0-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="023f0-134">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="023f0-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="023f0-135">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="023f0-136">Пример 1: список рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="023f0-136">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="023f0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="023f0-137">Request</span></span>
<span data-ttu-id="023f0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="023f0-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="023f0-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="023f0-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="023f0-140">C#</span><span class="sxs-lookup"><span data-stu-id="023f0-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="023f0-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="023f0-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="023f0-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="023f0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="023f0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="023f0-143">Response</span></span>
<span data-ttu-id="023f0-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="023f0-144">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="023f0-145">Пример 2: список рискованных пользователей и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="023f0-145">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="023f0-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="023f0-146">Request</span></span>
<span data-ttu-id="023f0-147">В приведенном ниже примере показано, как `$filter` получить коллекцию рискюсер с уровнем агрегированного риска среднего размера.</span><span class="sxs-lookup"><span data-stu-id="023f0-147">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="http"></a>[<span data-ttu-id="023f0-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="023f0-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="c"></a>[<span data-ttu-id="023f0-149">C#</span><span class="sxs-lookup"><span data-stu-id="023f0-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="023f0-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="023f0-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="023f0-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="023f0-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="023f0-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="023f0-152">Response</span></span>
<span data-ttu-id="023f0-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="023f0-153">Here is an example of the response.</span></span>
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
