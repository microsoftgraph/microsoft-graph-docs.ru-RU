---
title: Тип ресурса Девицехеалсскриптрунсчедуле
description: Базовый тип расписания запуска сценария работоспособности устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a1f28c4e6cfe5c1155c7cf96446d76dff609d6d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178530"
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



