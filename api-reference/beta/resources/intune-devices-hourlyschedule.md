---
title: Тип ресурса Хаурлисчедуле
description: ПоЧасовое расписание выполнения сценария управления повторяющимся устройством.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb3eacf4e17ed1137ce78d21112c394a45423c6b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173418"
---
# <a name="hourlyschedule-resource-type"></a>Тип ресурса Хаурлисчедуле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ПоЧасовое расписание выполнения сценария управления повторяющимся устройством.


НаСледуется от [рунсчедуле](../resources/intune-devices-runschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|Интервал (в часах)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```




