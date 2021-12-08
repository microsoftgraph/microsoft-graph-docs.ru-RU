---
title: Создание userExperienceAnalyticsBatteryHealthDevicePerformance
description: Создание нового объекта userExperienceAnalyticsBatteryHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ae7ad86c4beb0dc221daef729cb6314944d56f0
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343261"
---
# <a name="create-userexperienceanalyticsbatteryhealthdeviceperformance"></a>Создание userExperienceAnalyticsBatteryHealthDevicePerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsBatteryHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)

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
POST /deviceManagement/userExperienceAnalyticsBatteryHealthDevicePerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsBatteryHealthDevicePerformance.

В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsBatteryHealthDevicePerformance.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности устройства работоспособности устройства для аналитики пользовательского интерфейса.|
|deviceId|String|Уникальный идентификатор устройства Intune DeviceID.|
|deviceName|String|Удобное имя устройства.|
|model|String|Имя модели устройства.|
|maxCapacityPercentage|Int32|Отношение текущей емкости и проектной емкости батареи с наименьшей емкостью. Единица в процентах и значениях варьируется от 0 до 100. Допустимые значения 2147483648 2147483647|
|estimatedRuntimeInMinutes|Int32|Предполагаемое время работы устройства при полной зарядке батареи. Единица в минутах. Допустимые значения 2147483648 2147483647|
|batteryAgeInDays|Int32|Предполагаемое время автономной работы. Единица в днях. Допустимые значения 2147483648 2147483647|
|deviceBatteryHealthScore|Int32|Средневзвешенное значение максимального балла мощности устройства и оценки времени работы. Значения варьируются от 0 до 100. Допустимые значения 2147483648 2147483647|
|healthStatus|String|Общее состояние состояния заряда батареи устройства.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthDevicePerformance
Content-type: application/json
Content-length: 362

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "maxCapacityPercentage": 5,
  "estimatedRuntimeInMinutes": 9,
  "batteryAgeInDays": 0,
  "deviceBatteryHealthScore": 8,
  "healthStatus": "Health Status value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 411

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "id": "c8b9e0fd-e0fd-c8b9-fde0-b9c8fde0b9c8",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "maxCapacityPercentage": 5,
  "estimatedRuntimeInMinutes": 9,
  "batteryAgeInDays": 0,
  "deviceBatteryHealthScore": 8,
  "healthStatus": "Health Status value"
}
```




