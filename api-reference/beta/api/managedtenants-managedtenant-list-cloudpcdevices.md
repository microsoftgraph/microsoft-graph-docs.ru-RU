---
title: Список cloudPcDevices
description: Получите список объектов cloudPcDevice и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 65da1a66a6a423d3df8859d1cf74d16d03f6ded6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441526"
---
# <a name="list-cloudpcdevices"></a><span data-ttu-id="c4540-103">Список cloudPcDevices</span><span class="sxs-lookup"><span data-stu-id="c4540-103">List cloudPcDevices</span></span>
<span data-ttu-id="c4540-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c4540-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4540-105">Получите список объектов [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="c4540-105">Get a list of the [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4540-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4540-106">Permissions</span></span>
<span data-ttu-id="c4540-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4540-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4540-109">Permission type</span></span>|<span data-ttu-id="c4540-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4540-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4540-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4540-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4540-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4540-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c4540-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4540-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4540-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4540-114">Not supported.</span></span>|
|<span data-ttu-id="c4540-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4540-115">Application</span></span>|<span data-ttu-id="c4540-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4540-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4540-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4540-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4540-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4540-118">Optional query parameters</span></span>
<span data-ttu-id="c4540-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="c4540-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4540-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4540-120">Request headers</span></span>
|<span data-ttu-id="c4540-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c4540-121">Name</span></span>|<span data-ttu-id="c4540-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c4540-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4540-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4540-123">Authorization</span></span>|<span data-ttu-id="c4540-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4540-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4540-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4540-126">Request body</span></span>
<span data-ttu-id="c4540-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4540-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4540-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4540-128">Response</span></span>

<span data-ttu-id="c4540-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4540-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4540-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4540-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4540-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4540-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4540-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4540-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices
```
# <a name="c"></a>[<span data-ttu-id="c4540-133">C#</span><span class="sxs-lookup"><span data-stu-id="c4540-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcdevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4540-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4540-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcdevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4540-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4540-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcdevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4540-136">Java</span><span class="sxs-lookup"><span data-stu-id="c4540-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcdevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c4540-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4540-137">Response</span></span>
><span data-ttu-id="c4540-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c4540-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcDevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "00089754-92d2-483c-a073-420723aac8bc_6b97ad6a-be15-4cbe-afbb-4eb74ecb0243",
      "lastUpdated": "2021-07-10T23:05:03.2565097Z",
      "policyId": "2b142388-f36c-40ee-a5cb-7e8871a658a0",
      "displayName": "ImageProd - ImageRunner4PROD",
      "managedDeviceId": "f3a8e53b-0a9f-42f1-be73-4fd30d801f62",
      "managedDeviceName": "A0000060000",
      "userPrincipalName": "ImageRunner4PROD@fourthcoffee001.onmicrosoft.com",
      "servicePlanName": "CloudPC_Lite",
      "status": "Provisioned",
      "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
      "tenantDisplayName": "Fourth Coffee Publishing",
      "lastRefreshedDateTime": "2021-07-10T23:05:03.2565097Z",
      "provisioningPolicyId": "2b142388-f36c-40ee-a5cb-7e8871a658a0",
      "cloudPcStatus": "Provisioned"
    }
  ]
}
```
