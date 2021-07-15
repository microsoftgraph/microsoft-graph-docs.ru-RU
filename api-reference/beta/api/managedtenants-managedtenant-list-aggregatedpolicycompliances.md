---
title: Список агрегированныхPolicyCompliances
description: Получите список объектов aggregatedPolicyCompliance и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 160292f38035390d7b5ed769bbea42847bba71b2
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441555"
---
# <a name="list-aggregatedpolicycompliances"></a><span data-ttu-id="db83b-103">Список агрегированныхPolicyCompliances</span><span class="sxs-lookup"><span data-stu-id="db83b-103">List aggregatedPolicyCompliances</span></span>
<span data-ttu-id="db83b-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="db83b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db83b-105">Получите список объектов [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="db83b-105">Get a list of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="db83b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db83b-106">Permissions</span></span>
<span data-ttu-id="db83b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db83b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db83b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db83b-109">Permission type</span></span>|<span data-ttu-id="db83b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db83b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db83b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db83b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="db83b-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db83b-112">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db83b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db83b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db83b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db83b-114">Not supported.</span></span>|
|<span data-ttu-id="db83b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db83b-115">Application</span></span>|<span data-ttu-id="db83b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db83b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db83b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db83b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/aggregatedPolicyCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db83b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db83b-118">Optional query parameters</span></span>
<span data-ttu-id="db83b-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="db83b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db83b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db83b-120">Request headers</span></span>
|<span data-ttu-id="db83b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="db83b-121">Name</span></span>|<span data-ttu-id="db83b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="db83b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="db83b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db83b-123">Authorization</span></span>|<span data-ttu-id="db83b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db83b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db83b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db83b-126">Request body</span></span>
<span data-ttu-id="db83b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db83b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db83b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="db83b-128">Response</span></span>

<span data-ttu-id="db83b-129">В случае успешного использования этот метод возвращает код ответа и коллекцию объектов `200 OK` [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="db83b-129">If successful, this method returns a `200 OK` response code and a collection of [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db83b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="db83b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db83b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="db83b-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="db83b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="db83b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_aggregatedpolicycompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/aggregatedPolicyCompliances
```
# <a name="c"></a>[<span data-ttu-id="db83b-133">C#</span><span class="sxs-lookup"><span data-stu-id="db83b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-aggregatedpolicycompliance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db83b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db83b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-aggregatedpolicycompliance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db83b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db83b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-aggregatedpolicycompliance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db83b-136">Java</span><span class="sxs-lookup"><span data-stu-id="db83b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-aggregatedpolicycompliance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="db83b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="db83b-137">Response</span></span>
><span data-ttu-id="db83b-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="db83b-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
