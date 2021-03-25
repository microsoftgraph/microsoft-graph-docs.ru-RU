---
title: Get deviceCompliancePolicyAssignment
description: Чтение свойств и связей объекта deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f315fd7a5677b247b74cae796247246dc7f0db2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155479"
---
# <a name="get-devicecompliancepolicyassignment"></a><span data-ttu-id="767d3-103">Get deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="767d3-103">Get deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="767d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="767d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="767d3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="767d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="767d3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="767d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="767d3-107">Чтение свойств и связей объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="767d3-107">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="767d3-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="767d3-108">Prerequisites</span></span>
<span data-ttu-id="767d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="767d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="767d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="767d3-111">Permission type</span></span>|<span data-ttu-id="767d3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="767d3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="767d3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="767d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="767d3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="767d3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="767d3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="767d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="767d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="767d3-116">Not supported.</span></span>|
|<span data-ttu-id="767d3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="767d3-117">Application</span></span>|<span data-ttu-id="767d3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="767d3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="767d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="767d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="767d3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="767d3-120">Optional query parameters</span></span>
<span data-ttu-id="767d3-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="767d3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="767d3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="767d3-122">Request headers</span></span>
|<span data-ttu-id="767d3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="767d3-123">Header</span></span>|<span data-ttu-id="767d3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="767d3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="767d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="767d3-125">Authorization</span></span>|<span data-ttu-id="767d3-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="767d3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="767d3-127">Accept</span><span class="sxs-lookup"><span data-stu-id="767d3-127">Accept</span></span>|<span data-ttu-id="767d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="767d3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="767d3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="767d3-129">Request body</span></span>
<span data-ttu-id="767d3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="767d3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="767d3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="767d3-131">Response</span></span>
<span data-ttu-id="767d3-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="767d3-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="767d3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="767d3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="767d3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="767d3-134">Request</span></span>
<span data-ttu-id="767d3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="767d3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="767d3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="767d3-136">Response</span></span>
<span data-ttu-id="767d3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="767d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 540

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
    "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
    "target": {
      "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include",
      "collectionId": "Collection Id value"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```




