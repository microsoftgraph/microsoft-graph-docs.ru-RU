---
title: Тип ресурса Девицехеалсскриптдаилисчедуле
description: Ежедневное расписание сценариев работоспособности устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32206322473a4dd3986500865d01c071637f0669
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728111"
---
# <a name="devicehealthscriptdailyschedule-resource-type"></a>Тип ресурса Девицехеалсскриптдаилисчедуле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ежедневное расписание сценариев работоспособности устройств.


Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания. Допустимые значения — от 1 до 23, наследуемые от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|усеутк|Логический|Укажите время в формате UTC или местное время клиента. Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|time|TimeOfDay|При планировании запуска сценария. Эта коллекция может содержать не более 20 элементов. Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDailySchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```





