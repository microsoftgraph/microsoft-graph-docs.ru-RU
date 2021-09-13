---
title: Список userExperienceAnalyticsWorkFromAnywhereDevices
description: Список свойств и связей объектов userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 599a66a5d38d3133e1979e4e34819565eaa79d45
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59087935"
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
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.Read.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

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
|Authorization|Bearer &lt;token&gt;. Обязательный.|
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
Content-Length: 1429

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
      "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
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
      "windowsScore": 4.0,
      "cloudManagementScore": 6.666666666666667,
      "cloudIdentityScore": 6.0,
      "cloudProvisioningScore": 7.333333333333333,
      "healthStatus": "insufficientData"
    }
  ]
}
```



