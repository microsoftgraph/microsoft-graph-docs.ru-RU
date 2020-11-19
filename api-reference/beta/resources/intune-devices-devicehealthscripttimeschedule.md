---
title: Тип ресурса Девицехеалсскрипттимесчедуле
description: Базовый тип расписания работоспособности устройства для сценария работоспособности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 362bc9d449c3854fa98272758546a871333162a8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299340"
---
# <a name="devicehealthscripttimeschedule-resource-type"></a>Тип ресурса Девицехеалсскрипттимесчедуле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый тип расписания работоспособности устройства для сценария работоспособности.


Наследуется от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания. Допустимые значения — от 1 до 23, наследуемые от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|усеутк|Boolean|Укажите время в формате UTC или местное время клиента.|
|time|TimeOfDay|При планировании запуска сценария. Эта коллекция может содержать не более 20 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptTimeSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptTimeSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```




