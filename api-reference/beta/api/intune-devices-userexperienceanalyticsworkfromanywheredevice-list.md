---
title: Список userExperienceAnalyticsWorkFromAnywhereDevices
description: Список свойств и связей объектов userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 730a6a3209e82f20e8acf0933b1b8e927c92a6e1
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339334"
---
# <a name="list-userexperienceanalyticsworkfromanywheredevices"></a>Список userExperienceAnalyticsWorkFromAnywhereDevices

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей [объектов userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1549

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
      "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "ownership": "Ownership value",
      "managedBy": "Managed By value",
      "autoPilotRegistered": true,
      "autoPilotProfileAssigned": true,
      "azureAdRegistered": true,
      "azureAdDeviceId": "Azure Ad Device Id value",
      "azureAdJoinType": "Azure Ad Join Type value",
      "osDescription": "Os Description value",
      "osVersion": "Os Version value",
      "tenantAttached": true,
      "compliancePolicySetToIntune": true,
      "otherWorkloadsSetToIntune": true,
      "isCloudManagedGatewayEnabled": true,
      "upgradeEligibility": "unknown",
      "ramCheckFailed": true,
      "storageCheckFailed": true,
      "processorCoreCountCheckFailed": true,
      "processorSpeedCheckFailed": true,
      "tpmCheckFailed": true,
      "secureBootCheckFailed": true,
      "processorFamilyCheckFailed": true,
      "processor64BitCheckFailed": true,
      "osCheckFailed": true,
      "workFromAnywhereScore": 7.0,
      "windowsScore": 4.0,
      "cloudManagementScore": 6.666666666666667,
      "cloudIdentityScore": 6.0,
      "cloudProvisioningScore": 7.333333333333333,
      "healthStatus": "insufficientData"
    }
  ]
}
```




