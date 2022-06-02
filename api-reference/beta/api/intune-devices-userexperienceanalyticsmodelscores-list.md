---
title: Перечисление объектов userExperienceAnalyticsModelScores
description: Список свойств и связей объектов userExperienceAnalyticsModelScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc33e646e76090dc07ceeabb18e961d7c460a15a
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857759"
---
# <a name="list-userexperienceanalyticsmodelscoreses"></a>Перечисление объектов userExperienceAnalyticsModelScores

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsModelScores
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения `200 OK` этот метод возвращает код отклика и коллекцию объектов [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsModelScores
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 540

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
      "id": "f2c0f69c-f69c-f2c0-9cf6-c0f29cf6c0f2",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "modelDeviceCount": 0,
      "endpointAnalyticsScore": 7.333333333333333,
      "startupPerformanceScore": 7.666666666666667,
      "appReliabilityScore": 6.333333333333333,
      "workFromAnywhereScore": 7.0,
      "batteryHealthScore": 6.0,
      "healthStatus": "insufficientData"
    }
  ]
}
```




