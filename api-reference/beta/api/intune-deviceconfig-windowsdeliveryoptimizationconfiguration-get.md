---
title: Получить windowsDeliveryOptimizationConfiguration
description: Чтение свойств и связей объекта WindowsDeliveryOptimizationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7200cfd8ab5f55db9e05c712ac9be4dbd29718f1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132403"
---
# <a name="get-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="0b78e-103">Получить windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b78e-103">Get windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="0b78e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b78e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b78e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b78e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b78e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b78e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b78e-107">Чтение свойств и связей [объекта WindowsDeliveryOptimizationConfiguration.](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b78e-107">Read properties and relationships of the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b78e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0b78e-108">Prerequisites</span></span>
<span data-ttu-id="0b78e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b78e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b78e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b78e-111">Permission type</span></span>|<span data-ttu-id="0b78e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b78e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b78e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b78e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b78e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b78e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b78e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b78e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b78e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b78e-116">Not supported.</span></span>|
|<span data-ttu-id="0b78e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0b78e-117">Application</span></span>|<span data-ttu-id="0b78e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b78e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b78e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b78e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b78e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b78e-120">Optional query parameters</span></span>
<span data-ttu-id="0b78e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0b78e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b78e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b78e-122">Request headers</span></span>
|<span data-ttu-id="0b78e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b78e-123">Header</span></span>|<span data-ttu-id="0b78e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0b78e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b78e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b78e-125">Authorization</span></span>|<span data-ttu-id="0b78e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b78e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b78e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0b78e-127">Accept</span></span>|<span data-ttu-id="0b78e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0b78e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b78e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b78e-129">Request body</span></span>
<span data-ttu-id="0b78e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b78e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b78e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b78e-131">Response</span></span>
<span data-ttu-id="0b78e-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b78e-132">If successful, this method returns a `200 OK` response code and [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b78e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0b78e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b78e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b78e-134">Request</span></span>
<span data-ttu-id="0b78e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b78e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0b78e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b78e-136">Response</span></span>
<span data-ttu-id="0b78e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b78e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2344

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
    "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "deliveryOptimizationMode": "httpOnly",
    "restrictPeerSelectionBy": "subnetMask",
    "groupIdSource": {
      "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
    },
    "bandwidthMode": {
      "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
    },
    "backgroundDownloadFromHttpDelayInSeconds": 8,
    "foregroundDownloadFromHttpDelayInSeconds": 8,
    "minimumRamAllowedToPeerInGigabytes": 2,
    "minimumDiskSizeAllowedToPeerInGigabytes": 7,
    "minimumFileSizeToCacheInMegabytes": 1,
    "minimumBatteryPercentageAllowedToUpload": 7,
    "modifyCacheLocation": "Modify Cache Location value",
    "maximumCacheAgeInDays": 5,
    "maximumCacheSize": {
      "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
    },
    "vpnPeerCaching": "enabled",
    "cacheServerHostNames": [
      "Cache Server Host Names value"
    ],
    "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
    "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
  }
}
```




