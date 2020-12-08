---
title: Получение Усераттрибутеассигнментс
description: Чтение свойств и связей объекта Идентитюсерфловаттрибутеассигнмент.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c134e5e101080c007a0927fd18887262b8e10539
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581432"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="da88b-103">Получение Идентитюсерфловаттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="da88b-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="da88b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da88b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da88b-105">Чтение свойств и связей объекта [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="da88b-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="da88b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da88b-106">Permissions</span></span>

<span data-ttu-id="da88b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da88b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da88b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da88b-109">Permission type</span></span>|<span data-ttu-id="da88b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da88b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da88b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da88b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da88b-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="da88b-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="da88b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da88b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da88b-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="da88b-114">Not supported</span></span>|
|<span data-ttu-id="da88b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="da88b-115">Application</span></span>|<span data-ttu-id="da88b-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="da88b-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da88b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da88b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da88b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da88b-118">Optional query parameters</span></span>

<span data-ttu-id="da88b-119">Этот метод поддерживает `$select` `$expand` параметры запросов и для получения сведений об атрибуте пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="da88b-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="da88b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="da88b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="da88b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da88b-121">Request headers</span></span>

|<span data-ttu-id="da88b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="da88b-122">Name</span></span>|<span data-ttu-id="da88b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="da88b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da88b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da88b-124">Authorization</span></span>|<span data-ttu-id="da88b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da88b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da88b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da88b-127">Request body</span></span>

<span data-ttu-id="da88b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da88b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da88b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="da88b-129">Response</span></span>

<span data-ttu-id="da88b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da88b-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da88b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="da88b-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="da88b-132">Пример 1: получение сведений о Идентитюсерфловаттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="da88b-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="da88b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="da88b-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```

#### <a name="response"></a><span data-ttu-id="da88b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="da88b-134">Response</span></span>

<span data-ttu-id="da88b-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="da88b-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="da88b-136">Пример 2: получение сведений о Идентитюсерфловаттрибутеассигнмент и развертывание Усераттрибуте</span><span class="sxs-lookup"><span data-stu-id="da88b-136">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="da88b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="da88b-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```

#### <a name="response"></a><span data-ttu-id="da88b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="da88b-138">Response</span></span>

<span data-ttu-id="da88b-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="da88b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
