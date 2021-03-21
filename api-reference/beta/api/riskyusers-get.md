---
title: Get riskyUser
description: Извлечение свойств и связей объекта **riskyUser.**
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9582066edadf5fb431bec0f7b3c9701fe71ead8c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960797"
---
# <a name="get-riskyuser"></a><span data-ttu-id="5755b-103">Get riskyUser</span><span class="sxs-lookup"><span data-stu-id="5755b-103">Get riskyUser</span></span>

<span data-ttu-id="5755b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5755b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5755b-105">Извлечение свойств и связей объекта **riskyUser.**</span><span class="sxs-lookup"><span data-stu-id="5755b-105">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="5755b-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="5755b-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="5755b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5755b-107">Permissions</span></span>
<span data-ttu-id="5755b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5755b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5755b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5755b-110">Permission type</span></span>      | <span data-ttu-id="5755b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5755b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5755b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5755b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5755b-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5755b-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="5755b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5755b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5755b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5755b-115">Not supported.</span></span>    |
|<span data-ttu-id="5755b-116">Application</span><span class="sxs-lookup"><span data-stu-id="5755b-116">Application</span></span> | <span data-ttu-id="5755b-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="5755b-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5755b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5755b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
GET /identityProtection/riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="5755b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5755b-119">Request headers</span></span>
| <span data-ttu-id="5755b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5755b-120">Name</span></span>      |<span data-ttu-id="5755b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5755b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5755b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5755b-122">Authorization</span></span>  | <span data-ttu-id="5755b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5755b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5755b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5755b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5755b-126">ID сеанса книги, определяя, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="5755b-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="5755b-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5755b-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5755b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5755b-128">Request body</span></span>
<span data-ttu-id="5755b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5755b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5755b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5755b-130">Response</span></span>

<span data-ttu-id="5755b-131">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [riskyUser](../resources/riskyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5755b-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="5755b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="5755b-132">Examples</span></span>
### <a name="example-1-get-a-risky-user"></a><span data-ttu-id="5755b-133">Пример 1. Получить рискованного пользователя</span><span class="sxs-lookup"><span data-stu-id="5755b-133">Example 1: Get a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="5755b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5755b-134">Request</span></span>
<span data-ttu-id="5755b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5755b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5755b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5755b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_1",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="5755b-137">C#</span><span class="sxs-lookup"><span data-stu-id="5755b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5755b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5755b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5755b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5755b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5755b-140">Java</span><span class="sxs-lookup"><span data-stu-id="5755b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5755b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5755b-141">Response</span></span>
<span data-ttu-id="5755b-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5755b-142">Here is an example of the response.</span></span>
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
### <a name="example-2-get-risky-users"></a><span data-ttu-id="5755b-143">Пример 2. Получить рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="5755b-143">Example 2: Get risky users</span></span>
#### <a name="request"></a><span data-ttu-id="5755b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="5755b-144">Request</span></span>
<span data-ttu-id="5755b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5755b-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5755b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5755b-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_2",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers
```
# <a name="c"></a>[<span data-ttu-id="5755b-147">C#</span><span class="sxs-lookup"><span data-stu-id="5755b-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5755b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5755b-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5755b-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5755b-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5755b-150">Java</span><span class="sxs-lookup"><span data-stu-id="5755b-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5755b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="5755b-151">Response</span></span>
<span data-ttu-id="5755b-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5755b-152">Here is an example of the response.</span></span>
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



