---
title: тип ресурса userExperienceAnalyticsBatteryHealthDevicePerformance
description: Объект для аналитики работоспособности устройства для работоспособности устройств с пользовательским опытом содержит сведения об уровне батареи устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 214d47ddfc71972cb6be76e3db46e1499c562486
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62289904"
---
# <a name="userexperienceanalyticsbatteryhealthdeviceperformance-resource-type"></a>тип ресурса userExperienceAnalyticsBatteryHealthDevicePerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект для аналитики работоспособности устройства для работоспособности устройств с пользовательским опытом содержит сведения об уровне батареи устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейExperienceAnalyticsBatteryHealthDevicePerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-list.md)|[коллекция userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) .|
|[Get userExperienceAnalyticsBatteryHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-get.md)|[userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) .|
|[Создание userExperienceAnalyticsBatteryHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-create.md)|[userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)|Создание нового [объекта userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) .|
|[Удаление userExperienceAnalyticsBatteryHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md).|
|[Обновление userExperienceAnalyticsBatteryHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-update.md)|[userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) .|

## <a name="properties"></a>Свойства
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

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "maxCapacityPercentage": 1024,
  "estimatedRuntimeInMinutes": 1024,
  "batteryAgeInDays": 1024,
  "deviceBatteryHealthScore": 1024,
  "healthStatus": "String"
}
```




