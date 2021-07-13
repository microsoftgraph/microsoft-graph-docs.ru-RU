---
title: Список управляемыхDeviceComplianceTrends
description: Получите список объектов managedDeviceComplianceTrend и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ace0b14145df253d2d8f5c6cab62f3c23f0458c3
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402417"
---
# <a name="list-manageddevicecompliancetrends"></a><span data-ttu-id="a9a88-103">Список управляемыхDeviceComplianceTrends</span><span class="sxs-lookup"><span data-stu-id="a9a88-103">List managedDeviceComplianceTrends</span></span>
<span data-ttu-id="a9a88-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="a9a88-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9a88-105">Получите список объектов [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="a9a88-105">Get a list of the [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9a88-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9a88-106">Permissions</span></span>
<span data-ttu-id="a9a88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9a88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9a88-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9a88-109">Permission type</span></span>|<span data-ttu-id="a9a88-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9a88-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9a88-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9a88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9a88-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9a88-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a9a88-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9a88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9a88-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9a88-114">Not supported.</span></span>|
|<span data-ttu-id="a9a88-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9a88-115">Application</span></span>|<span data-ttu-id="a9a88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9a88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9a88-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9a88-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceComplianceTrends
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9a88-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a9a88-118">Optional query parameters</span></span>
<span data-ttu-id="a9a88-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="a9a88-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9a88-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9a88-120">Request headers</span></span>
|<span data-ttu-id="a9a88-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a9a88-121">Name</span></span>|<span data-ttu-id="a9a88-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a9a88-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a9a88-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9a88-123">Authorization</span></span>|<span data-ttu-id="a9a88-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9a88-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9a88-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9a88-126">Request body</span></span>
<span data-ttu-id="a9a88-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9a88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9a88-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9a88-128">Response</span></span>

<span data-ttu-id="a9a88-129">В случае успешного использования этот метод возвращает код ответа и коллекцию объектов `200 OK` [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a9a88-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9a88-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a9a88-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9a88-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9a88-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_manageddevicecompliancetrend"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/tenantRelationships/managedTenants/managedDeviceComplianceTrends
```


### <a name="response"></a><span data-ttu-id="a9a88-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9a88-132">Response</span></span>
><span data-ttu-id="a9a88-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a9a88-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managedDeviceComplianceTrend)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managedDeviceComplianceTrends",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_2021-06-12",
      "unknownDeviceCount": 0,
      "compliantDeviceCount": 4,
      "noncompliantDeviceCount": 0,
      "errorDeviceCount": 0,
      "inGracePeriodDeviceCount": 0,
      "configManagerDeviceCount": 0,
      "countDateTime": "2021-06-12",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_2021-06-16",
      "unknownDeviceCount": 0,
      "compliantDeviceCount": 1,
      "noncompliantDeviceCount": 4,
      "errorDeviceCount": 0,
      "inGracePeriodDeviceCount": 0,
      "configManagerDeviceCount": 0,
      "countDateTime": "2021-06-16",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
