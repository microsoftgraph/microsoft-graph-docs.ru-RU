---
title: Список riskyUsers
description: Получение свойств и связей коллекции объектов **рискюсер** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b91237a5957875256adf3a03d97054e05696894
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264976"
---
# <a name="list-riskyusers"></a><span data-ttu-id="5b066-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="5b066-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b066-104">Получение свойств и связей коллекции объектов **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="5b066-104">Retrieve the properties and relationships of a collection of **riskyUser** objects.</span></span>

><span data-ttu-id="5b066-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="5b066-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b066-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b066-106">Permissions</span></span>
<span data-ttu-id="5b066-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b066-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b066-109">Permission type</span></span>      | <span data-ttu-id="5b066-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b066-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b066-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b066-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b066-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b066-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="5b066-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b066-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b066-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b066-114">Not supported.</span></span>    |
|<span data-ttu-id="5b066-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b066-115">Application</span></span> | <span data-ttu-id="5b066-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b066-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b066-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b066-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b066-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b066-118">Optional query parameters</span></span>
<span data-ttu-id="5b066-119">Этот метод поддерживает `$filter` настройку ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="5b066-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="5b066-120">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="5b066-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="5b066-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b066-121">Request headers</span></span>
| <span data-ttu-id="5b066-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5b066-122">Name</span></span>      |<span data-ttu-id="5b066-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5b066-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b066-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b066-124">Authorization</span></span>  | <span data-ttu-id="5b066-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b066-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b066-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5b066-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="5b066-128">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="5b066-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="5b066-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="5b066-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b066-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b066-130">Request body</span></span>
<span data-ttu-id="5b066-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b066-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b066-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b066-132">Response</span></span>
<span data-ttu-id="5b066-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b066-133">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b066-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b066-134">Examples</span></span>
### <a name="example-1-list-risky-users"></a><span data-ttu-id="5b066-135">Пример 1: список рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="5b066-135">Example 1: List risky users</span></span>
#### <a name="request"></a><span data-ttu-id="5b066-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b066-136">Request</span></span>
<span data-ttu-id="5b066-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b066-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
#### <a name="response"></a><span data-ttu-id="5b066-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b066-138">Response</span></span>
<span data-ttu-id="5b066-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b066-139">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b066-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5b066-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b066-141">C#</span><span class="sxs-lookup"><span data-stu-id="5b066-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_riskyusers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b066-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b066-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_riskyusers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5b066-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5b066-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list_riskyusers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="5b066-144">Пример 2: список рискованных пользователей и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="5b066-144">Example 2: List risky users and filter the results</span></span>
#### <a name="request"></a><span data-ttu-id="5b066-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b066-145">Request</span></span>
<span data-ttu-id="5b066-146">В приведенном ниже примере показано, `$filter` как получить коллекцию рискюсер с уровнем агрегированного риска среднего размера.</span><span class="sxs-lookup"><span data-stu-id="5b066-146">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```

#### <a name="response"></a><span data-ttu-id="5b066-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b066-147">Response</span></span>
<span data-ttu-id="5b066-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b066-148">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5b066-149">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="5b066-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5b066-150">C#</span><span class="sxs-lookup"><span data-stu-id="5b066-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_filter_riskyusers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b066-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b066-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_filter_riskyusers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5b066-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5b066-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list_filter_riskyusers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
