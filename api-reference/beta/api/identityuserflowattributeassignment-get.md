---
title: Get userAttributeAssignments
description: Ознакомьтесь с свойствами и отношениями объекта identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3ed6fad28761a06c3289eaa2e661f7e53a8693da
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963317"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="c60de-103">Get identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="c60de-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="c60de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c60de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c60de-105">Ознакомьтесь с свойствами и отношениями объекта [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c60de-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c60de-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c60de-106">Permissions</span></span>

<span data-ttu-id="c60de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c60de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c60de-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c60de-109">Permission type</span></span>|<span data-ttu-id="c60de-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c60de-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c60de-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c60de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c60de-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c60de-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c60de-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c60de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c60de-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c60de-114">Not supported</span></span>|
|<span data-ttu-id="c60de-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c60de-115">Application</span></span>|<span data-ttu-id="c60de-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c60de-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c60de-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c60de-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c60de-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c60de-118">Optional query parameters</span></span>

<span data-ttu-id="c60de-119">Этот метод поддерживает параметры запроса и получения сведений `$select` `$expand` о атрибуте потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="c60de-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="c60de-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c60de-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c60de-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c60de-121">Request headers</span></span>

|<span data-ttu-id="c60de-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c60de-122">Name</span></span>|<span data-ttu-id="c60de-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c60de-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c60de-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c60de-124">Authorization</span></span>|<span data-ttu-id="c60de-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c60de-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c60de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c60de-127">Request body</span></span>

<span data-ttu-id="c60de-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c60de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c60de-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c60de-129">Response</span></span>

<span data-ttu-id="c60de-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c60de-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c60de-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c60de-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="c60de-132">Пример 1. Сведения о удостоверенииUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="c60de-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="c60de-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c60de-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c60de-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c60de-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="c60de-135">C#</span><span class="sxs-lookup"><span data-stu-id="c60de-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c60de-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c60de-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c60de-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c60de-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c60de-138">Java</span><span class="sxs-lookup"><span data-stu-id="c60de-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c60de-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c60de-139">Response</span></span>

<span data-ttu-id="c60de-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c60de-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('userFlowId')/userAttributeAssignments/$entity",
    "id": "City",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "City",
    "userAttributeValues": [
        {
            "name": "S",
            "value": "1",
            "isDefault": true
        }
    ]
}
```

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="c60de-141">Пример 2. Получить сведения о identityUserFlowAttributeAssignment и расширить userAttribute</span><span class="sxs-lookup"><span data-stu-id="c60de-141">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="c60de-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c60de-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c60de-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c60de-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```
# <a name="c"></a>[<span data-ttu-id="c60de-144">C#</span><span class="sxs-lookup"><span data-stu-id="c60de-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-expand-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c60de-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c60de-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-expand-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c60de-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c60de-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-expand-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c60de-147">Java</span><span class="sxs-lookup"><span data-stu-id="c60de-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-expand-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c60de-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c60de-148">Response</span></span>

<span data-ttu-id="c60de-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c60de-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('userFlowId')/userAttributeAssignments/$entity",
    "id": "City",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "City",
    "userAttributeValues": [
        {
            "name": "S",
            "value": "1",
            "isDefault": true
        }
    ],
    "userAttribute": {
        "id": "City",
        "displayName": "City",
        "description": "Your city",
        "userFlowAttributeType": "builtIn",
        "dataType": "string"
  }
}
```
