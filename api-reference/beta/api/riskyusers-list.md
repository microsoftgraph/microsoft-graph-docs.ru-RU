---
title: Список riskyUsers
description: Получение свойств и связей коллекции объектов **рискюсер** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3b7f0e41525d1847ba3217f6e35ffc72028e888
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979184"
---
# <a name="list-riskyusers"></a><span data-ttu-id="356df-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="356df-103">List riskyUsers</span></span>

<span data-ttu-id="356df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="356df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="356df-105">Получение свойств и связей коллекции объектов **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="356df-105">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="356df-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="356df-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="356df-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="356df-107">Permissions</span></span>
<span data-ttu-id="356df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="356df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="356df-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="356df-110">Permission type</span></span>      | <span data-ttu-id="356df-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="356df-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="356df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="356df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="356df-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="356df-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="356df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="356df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="356df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="356df-115">Not supported.</span></span>    |
|<span data-ttu-id="356df-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="356df-116">Application</span></span> | <span data-ttu-id="356df-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="356df-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="356df-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="356df-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
GET /identityProtection/riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="356df-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="356df-119">Optional query parameters</span></span>
<span data-ttu-id="356df-120">Этот метод поддерживает `$filter` настройку ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="356df-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="356df-121">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="356df-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="356df-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="356df-122">Request headers</span></span>
| <span data-ttu-id="356df-123">Имя</span><span class="sxs-lookup"><span data-stu-id="356df-123">Name</span></span>      |<span data-ttu-id="356df-124">Описание</span><span class="sxs-lookup"><span data-stu-id="356df-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="356df-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="356df-125">Authorization</span></span>  | <span data-ttu-id="356df-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="356df-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="356df-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="356df-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="356df-129">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="356df-129">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="356df-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="356df-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="356df-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="356df-131">Request body</span></span>
<span data-ttu-id="356df-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="356df-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="356df-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="356df-133">Response</span></span>
<span data-ttu-id="356df-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="356df-134">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="356df-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="356df-135">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="356df-136">Пример 1: список рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="356df-136">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="356df-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="356df-137">Request</span></span>
<span data-ttu-id="356df-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="356df-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="356df-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="356df-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="356df-140">C#</span><span class="sxs-lookup"><span data-stu-id="356df-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="356df-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="356df-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="356df-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="356df-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="356df-143">Java</span><span class="sxs-lookup"><span data-stu-id="356df-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="356df-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="356df-144">Response</span></span>
<span data-ttu-id="356df-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="356df-145">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="356df-146">Пример 2: список рискованных пользователей и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="356df-146">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="356df-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="356df-147">Request</span></span>
<span data-ttu-id="356df-148">В приведенном ниже примере показано, как `$filter` получить коллекцию рискюсер с уровнем агрегированного риска среднего размера.</span><span class="sxs-lookup"><span data-stu-id="356df-148">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>


# <a name="http"></a>[<span data-ttu-id="356df-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="356df-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="c"></a>[<span data-ttu-id="356df-150">C#</span><span class="sxs-lookup"><span data-stu-id="356df-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="356df-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="356df-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="356df-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="356df-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="356df-153">Java</span><span class="sxs-lookup"><span data-stu-id="356df-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskyusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="356df-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="356df-154">Response</span></span>
<span data-ttu-id="356df-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="356df-155">Here is an example of the response.</span></span>
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


