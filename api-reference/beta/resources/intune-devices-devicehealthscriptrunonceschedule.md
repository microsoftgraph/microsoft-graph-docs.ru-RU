---
title: тип ресурса deviceHealthScriptRunOnceSchedule
description: Сценарий состояния устройства запустится один раз.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c51150e9299a44495c517e8f78a4e67de3ce47c1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802476"
---
# <a name="devicehealthscriptrunonceschedule-resource-type"></a>тип ресурса deviceHealthScriptRunOnceSchedule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сценарий состояния устройства запустится один раз.


Наследует [от deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|X значение каждые х часов для почасового расписания, каждые х дней для ежедневного расписания, каждые х недель для еженедельного расписания, каждые х месяцев для ежемесячного расписания. Допустимые значения от 1 до 23, унаследованные от [устройстваHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|useUtc|Логический|Указать, является ли время Utc или клиент локальным. Унаследованный от [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|time|TimeOfDay|В какое время планируется запустить сценарий. Эта коллекция может содержать не более 20 элементов. Унаследованный от [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)|
|date|Date|Дата запуска сценария. Эта коллекция может содержать не более 20 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunOnceSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunOnceSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)",
  "date": "String (Date)"
}
```



