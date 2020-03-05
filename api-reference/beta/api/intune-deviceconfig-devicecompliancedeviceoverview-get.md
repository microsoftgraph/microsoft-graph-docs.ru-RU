---
title: Get deviceComplianceDeviceOverview
description: Чтение свойств и связей объекта deviceComplianceDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 71b2a7b7a9d9732c290605fbdd875989e19282ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449343"
---
# <a name="get-devicecompliancedeviceoverview"></a><span data-ttu-id="5a6f4-103">Get deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5a6f4-103">Get deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="5a6f4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5a6f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a6f4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a6f4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a6f4-107">Чтение свойств и связей объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="5a6f4-107">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a6f4-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5a6f4-108">Prerequisites</span></span>
<span data-ttu-id="5a6f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a6f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a6f4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a6f4-111">Permission type</span></span>|<span data-ttu-id="5a6f4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a6f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a6f4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a6f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a6f4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a6f4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a6f4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a6f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a6f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-116">Not supported.</span></span>|
|<span data-ttu-id="5a6f4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a6f4-117">Application</span></span>|<span data-ttu-id="5a6f4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a6f4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a6f4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a6f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a6f4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5a6f4-120">Optional query parameters</span></span>
<span data-ttu-id="5a6f4-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a6f4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a6f4-122">Request headers</span></span>
|<span data-ttu-id="5a6f4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a6f4-123">Header</span></span>|<span data-ttu-id="5a6f4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5a6f4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a6f4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a6f4-125">Authorization</span></span>|<span data-ttu-id="5a6f4-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a6f4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5a6f4-127">Accept</span></span>|<span data-ttu-id="5a6f4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5a6f4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a6f4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a6f4-129">Request body</span></span>
<span data-ttu-id="5a6f4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a6f4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a6f4-131">Response</span></span>
<span data-ttu-id="5a6f4-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a6f4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5a6f4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a6f4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a6f4-134">Request</span></span>
<span data-ttu-id="5a6f4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="5a6f4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a6f4-136">Response</span></span>
<span data-ttu-id="5a6f4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a6f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 432

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
    "id": "886f167b-167b-886f-7b16-6f887b166f88",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





