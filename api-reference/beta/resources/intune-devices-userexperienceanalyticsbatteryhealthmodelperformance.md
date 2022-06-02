---
title: Тип ресурса userExperienceAnalyticsBatteryHealthModelPerformance
description: Сущность производительности модели работоспособности аккумулятора аналитики пользовательского интерфейса содержит сведения, связанные с аккумулятором, для всех уникальных моделей устройств в организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 010b4498a8b725519636a727e0fada648c3a2b69
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857430"
---
# <a name="userexperienceanalyticsbatteryhealthmodelperformance-resource-type"></a>Тип ресурса userExperienceAnalyticsBatteryHealthModelPerformance

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность производительности модели работоспособности аккумулятора аналитики пользовательского интерфейса содержит сведения, связанные с аккумулятором, для всех уникальных моделей устройств в организации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов userExperienceAnalyticsBatteryHealthModelPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-list.md)|[Коллекция userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Список свойств и связей объектов [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .|
|[Получение userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-get.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Чтение свойств и связей объекта [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .|
|[Создание объекта userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-create.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Создайте объект [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .|
|[Удаление userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-delete.md)|Нет|Удаляет [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md).|
|[Обновление userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-update.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности модели работоспособности батареи аналитики пользовательского интерфейса.|
|activeDevices|Int32|Количество активных устройств для этой модели. Допустимые значения — 2147483648 2147483647|
|model|String|Имя модели устройства.|
|manufacturer|String|Имя производителя устройства.|
|averageMaxCapacityPercentage|Int32|Среднее значение максимальной емкости для всех устройств данной модели. Максимальная емкость измеряет полную стоимость и емкость конструктора для аккумуляторов устройства. Допустимые значения — 2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|Среднее значение предполагаемых сред выполнения при полной оплате для всех устройств данной модели. Единица в минутах. Допустимые значения — 2147483648 2147483647|
|averageBatteryAgeInDays|Int32|Среднее время заряда батареи для всех устройств данной модели в клиенте. Единица в днях. Допустимые значения — 2147483648 2147483647|
|modelBatteryHealthScore|Int32|Взвешенного среднего значения максимальной оценки емкости модели и оценки времени выполнения. Значения в диапазоне от 0 до 100. Допустимые значения — 2147483648 2147483647|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "model": "String",
  "manufacturer": "String",
  "averageMaxCapacityPercentage": 1024,
  "averageEstimatedRuntimeInMinutes": 1024,
  "averageBatteryAgeInDays": 1024,
  "modelBatteryHealthScore": 1024
}
```




