---
title: Получение Рискюсер
description: Получение свойств и связей объекта **рискюсер** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8414de9fe809e26e4895be2fb0ebfddfa1306cc1
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863511"
---
# <a name="get-riskyuser"></a><span data-ttu-id="9c421-103">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="9c421-103">Get riskyUser</span></span>

<span data-ttu-id="9c421-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c421-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c421-105">Получение свойств и связей объекта **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="9c421-105">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="9c421-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="9c421-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c421-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c421-107">Permissions</span></span>
<span data-ttu-id="9c421-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c421-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c421-110">Permission type</span></span>      | <span data-ttu-id="9c421-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c421-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c421-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c421-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c421-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c421-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="9c421-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c421-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c421-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c421-115">Not supported.</span></span>    |
|<span data-ttu-id="9c421-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c421-116">Application</span></span> | <span data-ttu-id="9c421-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c421-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c421-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c421-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
GET /identityProtection/riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="9c421-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c421-119">Request headers</span></span>
| <span data-ttu-id="9c421-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9c421-120">Name</span></span>      |<span data-ttu-id="9c421-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9c421-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c421-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c421-122">Authorization</span></span>  | <span data-ttu-id="9c421-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c421-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c421-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9c421-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9c421-126">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="9c421-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="9c421-127">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="9c421-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c421-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c421-128">Request body</span></span>
<span data-ttu-id="9c421-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c421-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c421-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c421-130">Response</span></span>

<span data-ttu-id="9c421-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c421-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="9c421-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="9c421-132">Examples</span></span>
### <a name="example-1-get-a-risky-user"></a><span data-ttu-id="9c421-133">Пример 1: получение опасного пользователя</span><span class="sxs-lookup"><span data-stu-id="9c421-133">Example 1: Get a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="9c421-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c421-134">Request</span></span>
<span data-ttu-id="9c421-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c421-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c421-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c421-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="9c421-137">C#</span><span class="sxs-lookup"><span data-stu-id="9c421-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c421-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c421-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c421-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c421-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9c421-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c421-140">Response</span></span>
<span data-ttu-id="9c421-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c421-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
### <a name="example-2-get-risky-users"></a><span data-ttu-id="9c421-142">Пример 2: получение рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="9c421-142">Example 2: Get risky users</span></span>
#### <a name="request"></a><span data-ttu-id="9c421-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c421-143">Request</span></span>
<span data-ttu-id="9c421-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c421-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c421-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c421-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="9c421-146">C#</span><span class="sxs-lookup"><span data-stu-id="9c421-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c421-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c421-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c421-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c421-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9c421-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c421-149">Response</span></span>
<span data-ttu-id="9c421-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c421-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

