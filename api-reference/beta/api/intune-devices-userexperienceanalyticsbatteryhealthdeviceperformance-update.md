---
title: Обновление userExperienceAnalyticsBatteryHealthDevicePerformance
description: Обновление свойств объекта userExperienceAnalyticsBatteryHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32a22971366bf0bd977e0cad9800e89b3495361b
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291929"
---
# <a name="update-userexperienceanalyticsbatteryhealthdeviceperformance"></a>Обновление userExperienceAnalyticsBatteryHealthDevicePerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthDevicePerformance/{userExperienceAnalyticsBatteryHealthDevicePerformanceId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) .

В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности устройства работоспособности устройства для аналитики пользовательского интерфейса.|
|deviceId|String|Уникальный идентификатор устройства Intune DeviceID.|
|deviceName|String|Удобное имя устройства.|
|model|String|Имя модели устройства.|
|manufacturer|String|Имя производителя устройства.|
|maxCapacityPercentage|Int32|Отношение текущей емкости и проектной емкости батареи с наименьшей емкостью. Единица в процентах и значениях варьируется от 0 до 100. Допустимые значения 2147483648 2147483647|
|estimatedRuntimeInMinutes|Int32|Предполагаемое время работы устройства при полной зарядке батареи. Единица в минутах. Допустимые значения 2147483648 2147483647|
|batteryAgeInDays|Int32|Предполагаемое время автономной работы. Единица в днях. Допустимые значения 2147483648 2147483647|
|deviceBatteryHealthScore|Int32|Средневзвешенное значение максимального балла мощности устройства и оценки времени работы. Значения варьируются от 0 до 100. Допустимые значения 2147483648 2147483647|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Общее состояние состояния заряда батареи устройства. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае `200 OK` успеха этот метод возвращает код отклика и обновленный объект [userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthDevicePerformance/{userExperienceAnalyticsBatteryHealthDevicePerformanceId}
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "maxCapacityPercentage": 5,
  "estimatedRuntimeInMinutes": 9,
  "batteryAgeInDays": 0,
  "deviceBatteryHealthScore": 8,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 449

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "id": "c8b9e0fd-e0fd-c8b9-fde0-b9c8fde0b9c8",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "maxCapacityPercentage": 5,
  "estimatedRuntimeInMinutes": 9,
  "batteryAgeInDays": 0,
  "deviceBatteryHealthScore": 8,
  "healthStatus": "insufficientData"
}
```




