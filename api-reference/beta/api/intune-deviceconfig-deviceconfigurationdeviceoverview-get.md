---
title: Get deviceConfigurationDeviceOverview
description: Чтение свойств и связей объекта deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd140947668dfd077f786e6389b2ad4d23a8d664
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131682"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="8fe2d-103">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8fe2d-103">Get deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="8fe2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fe2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fe2d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fe2d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fe2d-107">Чтение свойств и связей объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8fe2d-107">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fe2d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8fe2d-108">Prerequisites</span></span>
<span data-ttu-id="8fe2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fe2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fe2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fe2d-111">Permission type</span></span>|<span data-ttu-id="8fe2d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fe2d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fe2d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fe2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fe2d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fe2d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fe2d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fe2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fe2d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-116">Not supported.</span></span>|
|<span data-ttu-id="8fe2d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8fe2d-117">Application</span></span>|<span data-ttu-id="8fe2d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fe2d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fe2d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fe2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8fe2d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8fe2d-120">Optional query parameters</span></span>
<span data-ttu-id="8fe2d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fe2d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fe2d-122">Request headers</span></span>
|<span data-ttu-id="8fe2d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fe2d-123">Header</span></span>|<span data-ttu-id="8fe2d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8fe2d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fe2d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fe2d-125">Authorization</span></span>|<span data-ttu-id="8fe2d-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fe2d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8fe2d-127">Accept</span></span>|<span data-ttu-id="8fe2d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8fe2d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fe2d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fe2d-129">Request body</span></span>
<span data-ttu-id="8fe2d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fe2d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fe2d-131">Response</span></span>
<span data-ttu-id="8fe2d-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fe2d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8fe2d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fe2d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fe2d-134">Request</span></span>
<span data-ttu-id="8fe2d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="8fe2d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fe2d-136">Response</span></span>
<span data-ttu-id="8fe2d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fe2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
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




