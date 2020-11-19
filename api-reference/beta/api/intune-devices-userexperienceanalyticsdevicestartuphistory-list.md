---
title: Список Усерекспериенцеаналитиксдевицестартуфисториес
description: Список свойств и связей объектов Усерекспериенцеаналитиксдевицестартуфистори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40401d8412539de4c4fe59d1b385436cc52d66f4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234309"
---
# <a name="list-userexperienceanalyticsdevicestartuphistories"></a>Список Усерекспериенцеаналитиксдевицестартуфисториес

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
      "id": "13357123-7123-1335-2371-351323713513",
      "deviceId": "Device Id value",
      "startTime": "2017-01-01T00:03:29.2730865-08:00",
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "featureUpdateBootTimeInMs": 9,
      "totalBootTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "coreLoginTimeInMs": 1,
      "responsiveDesktopTimeInMs": 9,
      "totalLoginTimeInMs": 2,
      "isFirstLogin": true,
      "isFeatureUpdate": true,
      "operatingSystemVersion": "Operating System Version value",
      "restartCategory": "restartWithUpdate",
      "restartStopCode": "Restart Stop Code value",
      "restartFaultBucket": "Restart Fault Bucket value"
    }
  ]
}
```




