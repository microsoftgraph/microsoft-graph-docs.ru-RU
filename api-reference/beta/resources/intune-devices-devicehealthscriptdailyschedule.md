---
title: тип ресурса deviceHealthScriptDailySchedule
description: Ежедневное расписание скриптов для скриптов для устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92c65e8434a709fc5270cb1f5193d9341efca1e1e32131d76d339a80f4e52e28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244745"
---
# <a name="devicehealthscriptdailyschedule-resource-type"></a>тип ресурса deviceHealthScriptDailySchedule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ежедневное расписание скриптов для скриптов для устройств.


Наследует [от deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|X значение каждые х часов для почасового расписания, каждые х дней для ежедневного расписания, каждые х недель для еженедельного расписания, каждые х месяцев для ежемесячного расписания. Допустимые значения от 1 до 23, унаследованные от [устройстваHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|useUtc|Логический|Указать, является ли время Utc или клиент локальным. Унаследованный от [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|time|TimeOfDay|В какое время планируется запустить сценарий. Эта коллекция может содержать не более 20 элементов. Унаследованный от [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|

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




