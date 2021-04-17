---
title: Get userAttributeAssignments
description: Ознакомьтесь с свойствами и отношениями объекта identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fa51cbdc0d58c9a80863eeb3743ca56ec9d2e890
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883068"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="6b043-103">Get identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="6b043-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="6b043-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b043-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b043-105">Ознакомьтесь с свойствами и отношениями объекта [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6b043-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b043-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b043-106">Permissions</span></span>

<span data-ttu-id="6b043-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b043-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b043-109">Permission type</span></span>|<span data-ttu-id="6b043-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b043-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b043-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b043-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b043-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b043-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="6b043-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b043-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b043-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6b043-114">Not supported</span></span>|
|<span data-ttu-id="6b043-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b043-115">Application</span></span>|<span data-ttu-id="6b043-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b043-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b043-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b043-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b043-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6b043-118">Optional query parameters</span></span>

<span data-ttu-id="6b043-119">Этот метод поддерживает параметры запроса и получения сведений `$select` `$expand` о атрибуте потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6b043-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="6b043-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6b043-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b043-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b043-121">Request headers</span></span>

|<span data-ttu-id="6b043-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6b043-122">Name</span></span>|<span data-ttu-id="6b043-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6b043-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6b043-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b043-124">Authorization</span></span>|<span data-ttu-id="6b043-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b043-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b043-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b043-127">Request body</span></span>

<span data-ttu-id="6b043-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b043-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b043-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b043-129">Response</span></span>

<span data-ttu-id="6b043-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6b043-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b043-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b043-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="6b043-132">Пример 1. Сведения о удостоверенииUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="6b043-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="6b043-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b043-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City
```

#### <a name="response"></a><span data-ttu-id="6b043-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b043-134">Response</span></span>

<span data-ttu-id="6b043-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b043-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('userFlowId')/userAttributeAssignments/$entity",
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

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="6b043-136">Пример 2. Получить сведения о identityUserFlowAttributeAssignment и расширить userAttribute</span><span class="sxs-lookup"><span data-stu-id="6b043-136">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="6b043-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b043-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```

#### <a name="response"></a><span data-ttu-id="6b043-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b043-138">Response</span></span>

<span data-ttu-id="6b043-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b043-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('userFlowId')/userAttributeAssignments/$entity",
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
