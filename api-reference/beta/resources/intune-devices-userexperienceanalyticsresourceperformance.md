---
title: тип ресурса userExperienceAnalyticsResourcePerformance
description: Объект производительности ресурсов для аналитики пользовательского интерфейса.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca9f8fa6449871e5ead56976808267bb6cf2bfd9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046983"
---
# <a name="userexperienceanalyticsresourceperformance-resource-type"></a>тип ресурса userExperienceAnalyticsResourcePerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности ресурсов для аналитики пользовательского интерфейса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsResourcePerformances](../api/intune-devices-userexperienceanalyticsresourceperformance-list.md)|[коллекция userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Get userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-get.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Создание userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-create.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Создание нового [объекта userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Удаление userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md).|
|[Обновление userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-update.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Обновление свойств объекта [userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[summarizeDeviceResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-summarizedeviceresourceperformance.md)|[коллекция userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор сущности производительности ресурсов аналитики пользовательских интерфейсов.|
|deviceId|String|ID устройства.|
|deviceName|String|Имя устройства.|
|model|String|Модель устройства аналитики пользовательских интерфейсов.|
|deviceCount|Int64|Аналитика пользовательских интерфейсов суммирует количество устройств.|
|manufacturer|String|Производитель устройств аналитики пользовательских интерфейсов.|
|cpuSpikeTimePercentage|Двойное с плавающей точкой|Время пика ЦП в процентах. Допустимые значения: от 0 до 100|
|ramSpikeTimePercentage|Двойное с плавающей точкой|Время пика оперативной памяти в процентах. Допустимые значения: от 0 до 100|
|cpuSpikeTimeScore|Int32|Оценка времени пика пика ЦП для пользовательского интерфейса. Допустимые значения: от 0 до 100|
|cpuSpikeTimePercentageThreshold|Двойное с плавающей точкой|Порог cpuSpikeTimeScore. Допустимые значения: от 0 до 100|
|ramSpikeTimeScore|Int32|Оценка времени пика пика оперативной памяти устройства аналитики пользовательского интерфейса. Допустимые значения: от 0 до 100|
|ramSpikeTimePercentageThreshold|Двойное с плавающей точкой|Порог ramSpikeTimeScore. Допустимые значения: от 0 до 100|
|deviceResourcePerformanceScore|Int32|Оценка производительности ресурсов определенного устройства. Допустимые значения: от 0 до 100|
|averageSpikeTimeScore|Int32|AverageSpikeTimeScore устройства или типа модели. Допустимые значения: от 0 до 100.|

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
  "deviceResourcePerformanceScore": 1024,
  "averageSpikeTimeScore": 1024
}
```



