---
title: Список userExperienceAnalyticsDevicePerformances
description: Список свойств и связей объектов userExperienceAnalyticsDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f758e01fb2998a53c8a7f57782338b3f2281ab6b
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291922"
---
# <a name="list-userexperienceanalyticsdeviceperformances"></a>Список userExperienceAnalyticsDevicePerformances

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей [объектов userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .

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
GET /deviceManagement/userExperienceAnalyticsDevicePerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной `200 OK` работы этот метод возвращает код ответа и коллекцию объектов [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 909

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
      "id": "852ae826-e826-852a-26e8-2a8526e82a85",
      "deviceName": "Device Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "diskType": "ssd",
      "operatingSystemVersion": "Operating System Version value",
      "bootScore": 9,
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "healthStatus": "insufficientData",
      "loginScore": 10,
      "coreLoginTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "deviceCount": 11,
      "responsiveDesktopTimeInMs": 9,
      "blueScreenCount": 15,
      "restartCount": 12,
      "averageBlueScreens": 6.0,
      "averageRestarts": 5.0,
      "startupPerformanceScore": 7.666666666666667,
      "modelStartupPerformanceScore": 9.3333333333333339
    }
  ]
}
```




