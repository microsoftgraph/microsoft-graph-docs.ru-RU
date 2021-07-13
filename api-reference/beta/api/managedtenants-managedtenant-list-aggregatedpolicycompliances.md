---
title: Список агрегированныхPolicyCompliances
description: Получите список объектов aggregatedPolicyCompliance и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a9ec9c51db24dc6618eabda1a4d9dda957c23532
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402483"
---
# <a name="list-aggregatedpolicycompliances"></a><span data-ttu-id="f3f0b-103">Список агрегированныхPolicyCompliances</span><span class="sxs-lookup"><span data-stu-id="f3f0b-103">List aggregatedPolicyCompliances</span></span>
<span data-ttu-id="f3f0b-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f3f0b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3f0b-105">Получите список объектов [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="f3f0b-105">Get a list of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3f0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f0b-106">Permissions</span></span>
<span data-ttu-id="f3f0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3f0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3f0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f0b-109">Permission type</span></span>|<span data-ttu-id="f3f0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3f0b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3f0b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3f0b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3f0b-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f0b-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3f0b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3f0b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3f0b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3f0b-114">Not supported.</span></span>|
|<span data-ttu-id="f3f0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3f0b-115">Application</span></span>|<span data-ttu-id="f3f0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3f0b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3f0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3f0b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/aggregatedPolicyCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3f0b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3f0b-118">Optional query parameters</span></span>
<span data-ttu-id="f3f0b-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="f3f0b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3f0b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3f0b-120">Request headers</span></span>
|<span data-ttu-id="f3f0b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f3f0b-121">Name</span></span>|<span data-ttu-id="f3f0b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f3f0b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f3f0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3f0b-123">Authorization</span></span>|<span data-ttu-id="f3f0b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3f0b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3f0b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3f0b-126">Request body</span></span>
<span data-ttu-id="f3f0b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3f0b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3f0b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3f0b-128">Response</span></span>

<span data-ttu-id="f3f0b-129">В случае успешного использования этот метод возвращает код ответа и коллекцию объектов `200 OK` [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f3f0b-129">If successful, this method returns a `200 OK` response code and a collection of [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3f0b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f3f0b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3f0b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3f0b-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_aggregatedpolicycompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/aggregatedPolicyCompliances
```


### <a name="response"></a><span data-ttu-id="f3f0b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3f0b-132">Response</span></span>
><span data-ttu-id="f3f0b-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f3f0b-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.aggregatedPolicyCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#aggregatedPolicyCompliances",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
      "compliancePolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
      "compliancePolicyName": "Baseline - Setup Compliance Policy for Windows devices",
      "compliancePolicyType": "Unknown",
      "compliancePolicyPlatform": "Windows10",
      "numberOfCompliantDevices": 0,
      "numberOfNonCompliantDevices": 0,
      "numberOfErrorDevices": 0,
      "policyModifiedDateTime": "2021-06-22T17:01:46Z",
      "lastRefreshedDateTime": "2021-07-11T01:02:33.4452876Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_3e4b612f-5ce0-42f6-9e21-a172adc5100d",
      "compliancePolicyId": "3e4b612f-5ce0-42f6-9e21-a172adc5100d",
      "compliancePolicyName": "Windows Level 2 Compliance Policy",
      "compliancePolicyType": "Unknown",
      "compliancePolicyPlatform": "Windows10",
      "numberOfCompliantDevices": 4,
      "numberOfNonCompliantDevices": 0,
      "numberOfErrorDevices": 0,
      "policyModifiedDateTime": "2021-04-20T22:27:20Z",
      "lastRefreshedDateTime": "2021-07-11T01:02:33.4452876Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
