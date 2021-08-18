---
title: тип ресурса deviceHealthScriptTimeSchedule
description: Базовый тип расписания скрипта для скрипта для здоровья устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9f13ec9c3913cadbfb99b37416e24903bb823e2b551a26b1ba27f9933e609c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54232589"
---
# <a name="devicehealthscripttimeschedule-resource-type"></a>тип ресурса deviceHealthScriptTimeSchedule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый тип расписания скрипта для скрипта для здоровья устройств.


Наследует от [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|X значение каждые х часов для почасового расписания, каждые х дней для ежедневного расписания, каждые х недель для еженедельного расписания, каждые х месяцев для ежемесячного расписания. Допустимые значения от 1 до 23, унаследованные от [устройстваHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|
|useUtc|Логический|Указать, является ли время Utc или клиент локальным.|
|time|TimeOfDay|В какое время планируется запустить сценарий. Эта коллекция может содержать не более 20 элементов.|

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




