---
title: тип ресурса deviceHealthScriptHourlySchedule
description: Почасовая расписка скрипта для скрипта для устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9dd0db7952d20a5f67f5d484f2ee5447dbdd5458a9bfcb5b601bbbe3e27e55e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206419"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a>тип ресурса deviceHealthScriptHourlySchedule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Почасовая расписка скрипта для скрипта для устройств.


Наследует от [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|X значение каждые х часов для почасового расписания, каждые х дней для ежедневного расписания, каждые х недель для еженедельного расписания, каждые х месяцев для ежемесячного расписания. Допустимые значения от 1 до 23, унаследованные от [устройстваHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptHourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
  "interval": 1024
}
```




