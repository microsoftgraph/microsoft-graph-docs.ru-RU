---
title: тип ресурса userExperienceAnalyticsBatteryHealthModelPerformance
description: Объект производительности модели работоспособности модели работоспособности пользовательского интерфейса содержит сведения, связанные с батареей для всех уникальных моделей устройств в их организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02f3b336b3edce12d5f290d496fef440d959230e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343149"
---
# <a name="userexperienceanalyticsbatteryhealthmodelperformance-resource-type"></a>тип ресурса userExperienceAnalyticsBatteryHealthModelPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности модели работоспособности модели работоспособности пользовательского интерфейса содержит сведения, связанные с батареей для всех уникальных моделей устройств в их организации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейExperienceAnalyticsBatteryHealthModelPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-list.md)|[коллекция userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|
|[Get userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-get.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|
|[Создание userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-create.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Создайте новый [объект userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|
|[Удаление userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md).|
|[Обновление userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-update.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности модели работоспособности модели работоспособности пользовательской аналитики.|
|activeDevices|Int32|Количество активных устройств для этой модели. Допустимые значения 2147483648 2147483647|
|model|String|Имя модели устройства.|
|manufacturer|String|Имя производителя устройств.|
|averageMaxCapacityPercentage|Int32|Значение максимальной емкости для всех устройств данной модели. Максимальная емкость измеряет полную мощность заряда по сравнению с проектной мощностью для аккумуляторов устройства.. Допустимые значения 2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|Для всех устройств данной модели имеется в виду предполагаемое время запуска на полную плату. Единица в минутах. Допустимые значения 2147483648 2147483647|
|averageBatteryAgeInDays|Int32|Время работы от батареи для всех устройств данной модели в клиенте. Единица в днях. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
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
  "averageBatteryAgeInDays": 1024
}
```




