---
title: Тип ресурса Девицехеалсскриптрунсчедуле
description: Базовый тип расписания запуска сценария работоспособности устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 813512f607b6b0bd4eaf633c41ccd5a28554936e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299382"
---
# <a name="devicehealthscriptrunschedule-resource-type"></a>Тип ресурса Девицехеалсскриптрунсчедуле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый тип расписания запуска сценария работоспособности устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|interval|Int32|Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания. Допустимые значения — от 1 до 23.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSchedule",
  "interval": 1024
}
```




