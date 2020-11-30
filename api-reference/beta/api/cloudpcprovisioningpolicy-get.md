---
title: Получение Клаудпкпровисионингполици
description: Чтение свойств и связей объекта Клаудпкпровисионингполици.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: fa46603bddde0e12e34ad1abccf5afaa74861971
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378548"
---
# <a name="get-cloudpcprovisioningpolicy"></a><span data-ttu-id="1277d-103">Получение Клаудпкпровисионингполици</span><span class="sxs-lookup"><span data-stu-id="1277d-103">Get cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="1277d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1277d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1277d-105">Чтение свойств и связей объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1277d-105">Read the properties and relationships of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1277d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1277d-106">Permissions</span></span>

<span data-ttu-id="1277d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1277d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1277d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1277d-109">Permission type</span></span>|<span data-ttu-id="1277d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1277d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1277d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1277d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1277d-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="1277d-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="1277d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1277d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1277d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1277d-114">Not supported.</span></span>|
|<span data-ttu-id="1277d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1277d-115">Application</span></span>|<span data-ttu-id="1277d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1277d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1277d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1277d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1277d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1277d-118">Optional query parameters</span></span>

<span data-ttu-id="1277d-119">Этот метод поддерживает `$select` и `$expand` параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1277d-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="1277d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1277d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1277d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1277d-121">Request headers</span></span>

| <span data-ttu-id="1277d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1277d-122">Name</span></span>          | <span data-ttu-id="1277d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1277d-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1277d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1277d-124">Authorization</span></span> | <span data-ttu-id="1277d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1277d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1277d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1277d-127">Request body</span></span>

<span data-ttu-id="1277d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1277d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1277d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1277d-129">Response</span></span>

<span data-ttu-id="1277d-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1277d-130">If successful, this method returns a `200 OK` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1277d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1277d-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-provisioning-policy"></a><span data-ttu-id="1277d-132">Пример 1: получение свойств указанной политики подготовки</span><span class="sxs-lookup"><span data-stu-id="1277d-132">Example 1: Get the properties of the specified provisioning policy</span></span>

#### <a name="request"></a><span data-ttu-id="1277d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1277d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

#### <a name="response"></a><span data-ttu-id="1277d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1277d-134">Response</span></span>

<span data-ttu-id="1277d-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1277d-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-properties-of-the-specified-provisioning-policy-and-expand-on-the-assignments"></a><span data-ttu-id="1277d-136">Пример 2: получение свойств указанной политики подготовки и развертывание в назначениях</span><span class="sxs-lookup"><span data-stu-id="1277d-136">Example 2: Get the properties of the specified provisioning policy and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="1277d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1277d-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcprovisioningpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}?$expand=assignments
```

#### <a name="response"></a><span data-ttu-id="1277d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1277d-138">Response</span></span>

<span data-ttu-id="1277d-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1277d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
