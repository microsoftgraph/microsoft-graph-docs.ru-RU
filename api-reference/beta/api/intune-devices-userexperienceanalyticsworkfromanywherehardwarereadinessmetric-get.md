---
title: Get userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
description: Чтение свойств и связей объекта userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e53fa64d3443bc2ab092ea7033d6738740dd216e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348266"
---
# <a name="get-userexperienceanalyticsworkfromanywherehardwarereadinessmetric"></a>Get userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)

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
GET /deviceManagement/userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `200 OK` [объект userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 720

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
    "id": "6df21a06-1a06-6df2-061a-f26d061af26d",
    "totalDeviceCount": 0,
    "upgradeEligibleDeviceCount": 10,
    "ramCheckFailedPercentage": 8.0,
    "storageCheckFailedPercentage": 9.3333333333333339,
    "processorCoreCountCheckFailedPercentage": 13.0,
    "processorSpeedCheckFailedPercentage": 11.666666666666666,
    "tpmCheckFailedPercentage": 8.0,
    "secureBootCheckFailedPercentage": 10.333333333333334,
    "processorFamilyCheckFailedPercentage": 12.0,
    "processor64BitCheckFailedPercentage": 11.666666666666666,
    "osCheckFailedPercentage": 7.666666666666667
  }
}
```




