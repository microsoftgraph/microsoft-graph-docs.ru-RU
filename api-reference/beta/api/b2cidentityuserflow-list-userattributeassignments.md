---
title: Список userAttributeAssignments
description: Получите ресурсы identityUserFlowAttributeAssignment из свойства навигации userAttributeAssignments в b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 46a3f1d7c33440976a71b142b1ec5fc4616c26cf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944743"
---
# <a name="list-userattributeassignments"></a><span data-ttu-id="71e30-103">Список userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="71e30-103">List userAttributeAssignments</span></span>

<span data-ttu-id="71e30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71e30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71e30-105">Получите ресурсы identityUserFlowAttributeAssignment из свойства навигации userAttributeAssignments в [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="71e30-105">Get the identityUserFlowAttributeAssignment resources from the userAttributeAssignments navigation property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71e30-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71e30-106">Permissions</span></span>

<span data-ttu-id="71e30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71e30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71e30-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71e30-109">Permission type</span></span>|<span data-ttu-id="71e30-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71e30-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71e30-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71e30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71e30-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71e30-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="71e30-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71e30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71e30-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="71e30-114">Not supported</span></span>|
|<span data-ttu-id="71e30-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="71e30-115">Application</span></span>|<span data-ttu-id="71e30-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71e30-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71e30-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71e30-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71e30-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71e30-118">Optional query parameters</span></span>

<span data-ttu-id="71e30-119">Этот метод поддерживает параметры и сведения о атрибуте `$select` `$expand` потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="71e30-119">This method supports the `$select` and `$expand` parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="71e30-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="71e30-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="71e30-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71e30-121">Request headers</span></span>

|<span data-ttu-id="71e30-122">Имя</span><span class="sxs-lookup"><span data-stu-id="71e30-122">Name</span></span>|<span data-ttu-id="71e30-123">Описание</span><span class="sxs-lookup"><span data-stu-id="71e30-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="71e30-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71e30-124">Authorization</span></span>|<span data-ttu-id="71e30-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71e30-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71e30-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71e30-127">Request body</span></span>

<span data-ttu-id="71e30-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71e30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71e30-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e30-129">Response</span></span>

<span data-ttu-id="71e30-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71e30-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71e30-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="71e30-131">Examples</span></span>

### <a name="example-1-list-userattributeassignments-in-a-b2cidentityuserflow"></a><span data-ttu-id="71e30-132">Пример 1. Список userAttributeAssignments в b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="71e30-132">Example 1: List userAttributeAssignments in a b2cIdentityUserFlow</span></span>

#### <a name="request"></a><span data-ttu-id="71e30-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="71e30-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="71e30-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="71e30-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?
```
# <a name="c"></a>[<span data-ttu-id="71e30-135">C#</span><span class="sxs-lookup"><span data-stu-id="71e30-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71e30-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71e30-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71e30-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71e30-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71e30-138">Java</span><span class="sxs-lookup"><span data-stu-id="71e30-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71e30-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e30-139">Response</span></span>

<span data-ttu-id="71e30-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71e30-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ]
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": []
        }
    ]
}
```

### <a name="example-2-list-userattributeassignments-in-a-b2cidentityuserflow-and-expand-userattribute"></a><span data-ttu-id="71e30-141">Пример 2. Список userAttributeAssignments в b2cIdentityUserFlow и расширение userAttribute</span><span class="sxs-lookup"><span data-stu-id="71e30-141">Example 2: List userAttributeAssignments in a b2cIdentityUserFlow and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="71e30-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="71e30-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="71e30-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="71e30-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?$expand=userAttribute
```
# <a name="c"></a>[<span data-ttu-id="71e30-144">C#</span><span class="sxs-lookup"><span data-stu-id="71e30-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-expand-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71e30-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71e30-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-expand-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71e30-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71e30-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-expand-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71e30-147">Java</span><span class="sxs-lookup"><span data-stu-id="71e30-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-expand-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="71e30-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e30-148">Response</span></span>

<span data-ttu-id="71e30-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71e30-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.BuiltInUserFlowAttribute",
                "id": "City",
                "displayName": "City",
                "description": "your city",
                "userFlowAttributeType": "builtIn",
                "dataType": "string"
            }
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": [],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.CustomUserFlowAttribute",
                "id": "extension_guid_shoeSize",
                "displayName": "Shoe size",
                "description": "Your shoe size",
                "userFlowAttributeType": "custom",
                "dataType": "string"
            }
        }
    ]
}
```
