---
title: Get cloudPcProvisioningPolicy
description: Чтение свойств и связей объекта cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 99a94314e9c7314ee4b3e242ca5382b6acf19c58
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872725"
---
# <a name="get-cloudpcprovisioningpolicy"></a><span data-ttu-id="f518d-103">Get cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="f518d-103">Get cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="f518d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f518d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f518d-105">Чтение свойств и связей объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f518d-105">Read the properties and relationships of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="f518d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f518d-106">Permissions</span></span>

<span data-ttu-id="f518d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f518d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f518d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f518d-109">Permission type</span></span>|<span data-ttu-id="f518d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f518d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f518d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f518d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f518d-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f518d-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f518d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f518d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f518d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f518d-114">Not supported.</span></span>|
|<span data-ttu-id="f518d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f518d-115">Application</span></span>|<span data-ttu-id="f518d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f518d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f518d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f518d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f518d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f518d-118">Optional query parameters</span></span>

<span data-ttu-id="f518d-119">Этот метод поддерживает и `$select` `$expand` параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f518d-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f518d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f518d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f518d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f518d-121">Request headers</span></span>

| <span data-ttu-id="f518d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f518d-122">Name</span></span>          | <span data-ttu-id="f518d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f518d-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f518d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f518d-124">Authorization</span></span> | <span data-ttu-id="f518d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f518d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f518d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f518d-127">Request body</span></span>

<span data-ttu-id="f518d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f518d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f518d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f518d-129">Response</span></span>

<span data-ttu-id="f518d-130">В случае успеха этот метод возвращает код отклика и объект `200 OK` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f518d-130">If successful, this method returns a `200 OK` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f518d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f518d-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-provisioning-policy"></a><span data-ttu-id="f518d-132">Пример 1. Получите свойства указанной политики предоставления</span><span class="sxs-lookup"><span data-stu-id="f518d-132">Example 1: Get the properties of the specified provisioning policy</span></span>

#### <a name="request"></a><span data-ttu-id="f518d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f518d-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f518d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f518d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="f518d-135">C#</span><span class="sxs-lookup"><span data-stu-id="f518d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f518d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f518d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f518d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f518d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f518d-138">Java</span><span class="sxs-lookup"><span data-stu-id="f518d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f518d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f518d-139">Response</span></span>

<span data-ttu-id="f518d-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f518d-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "description": "Description value",
    "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
    "imageId": "Image ID value",
    "imageDisplayName": "Image Display Name value",
    "imageType": "custom"
  }
}
```

### <a name="example-2-get-the-properties-of-the-specified-provisioning-policy-and-expand-on-the-assignments"></a><span data-ttu-id="f518d-141">Пример 2. Получить свойства указанной политики и развернуть назначения</span><span class="sxs-lookup"><span data-stu-id="f518d-141">Example 2: Get the properties of the specified provisioning policy and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="f518d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f518d-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f518d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f518d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}?$expand=assignments
```
# <a name="c"></a>[<span data-ttu-id="f518d-144">C#</span><span class="sxs-lookup"><span data-stu-id="f518d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f518d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f518d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f518d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f518d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f518d-147">Java</span><span class="sxs-lookup"><span data-stu-id="f518d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f518d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f518d-148">Response</span></span>

<span data-ttu-id="f518d-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f518d-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "description": "Description value",
    "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
    "imageId": "Image ID value",
    "imageDisplayName": "Image Display Name value",
    "imageType": "custom",
    "assignments": [
      {
        "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
        "target": {
          "@odata.type":"microsoft.graph.cloudPCManagementGroupAssignmentTarget",
          "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26bfd9"
          }
      }
    ]
  }
}
```
