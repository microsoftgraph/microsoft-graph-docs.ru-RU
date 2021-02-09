---
title: Тип ресурса userExperienceAnalyticsResourcePerformance
description: Сущность производительности ресурсов аналитики пользовательского интерфейса.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7666c09cd2b27e6c657a71c97693f025cfcc9360
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160969"
---
# <a name="userexperienceanalyticsresourceperformance-resource-type"></a>Тип ресурса userExperienceAnalyticsResourcePerformance

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность производительности ресурсов аналитики пользовательского интерфейса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsResourcePerformances](../api/intune-devices-userexperienceanalyticsresourceperformance-list.md)|[Коллекция userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Get userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-get.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Чтение свойств и связей объекта [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Создание userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-create.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Создание объекта [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Удаление userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Обновление userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-update.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Обновление свойств объекта [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[функция summarizeDeviceResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-summarizedeviceresourceperformance.md)|[Коллекция userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор сущности производительности ресурсов аналитики пользовательского интерфейса.|
|deviceId|String|ИД устройства.|
|deviceName|String|Имя устройства.|
|model|String|Модель устройства аналитики пользовательского интерфейса.|
|deviceCount|Int64|Аналитика пользовательского интерфейса суммирует количество устройств.|
|manufacturer|String|Изготовитель устройства аналитики пользовательского интерфейса.|
|cpuSpikeTimePercentage|Двойное с плавающей точкой|Время пика ЦП в процентах. Допустимые значения: от 0 до 100|
|ramSpikeTimePercentage|Двойное с плавающей точкой|Время пика ОЗУ в процентах. Допустимые значения: от 0 до 100|
|cpuSpikeTimeScore|Int32|Оценка времени пика пика ЦП устройства аналитики пользовательского интерфейса. Допустимые значения: от 0 до 100|
|cpuSpikeTimePercentageThreshold|Двойное с плавающей точкой|Пороговое значение cpuSpikeTimeScore. Допустимые значения: от 0 до 100|
|ramSpikeTimeScore|Int32|Показатель времени пика пика ОЗУ устройства аналитики пользовательского интерфейса. Допустимые значения: от 0 до 100|
|ramSpikeTimePercentageThreshold|Двойное с плавающей точкой|Пороговое значение ramSpikeTimeScore. Допустимые значения: от 0 до 100|
|deviceResourcePerformanceScore|Int32|Оценка производительности ресурсов для конкретного устройства. Допустимые значения: от 0 до 100.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsResourcePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "model": "String",
  "deviceCount": 1024,
  "manufacturer": "String",
  "cpuSpikeTimePercentage": "4.2",
  "ramSpikeTimePercentage": "4.2",
  "cpuSpikeTimeScore": 1024,
  "cpuSpikeTimePercentageThreshold": "4.2",
  "ramSpikeTimeScore": 1024,
  "ramSpikeTimePercentageThreshold": "4.2",
  "deviceResourcePerformanceScore": 1024
}
```




