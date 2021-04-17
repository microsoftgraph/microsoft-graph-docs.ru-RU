---
title: тип ресурса attendanceInterval
description: Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1746adc802534f72aa9d139c6a16d8da62dd9fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882725"
---
# <a name="attendanceinterval-resource-type"></a>тип ресурса attendanceInterval

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| joinDateTime | DateTime | Участник time присоединился к UTC. |
| leaveDateTime | DateTime | Время участника, оставленного в UTC. |
| durationInSeconds | Int32 | Продолжительность интервала собрания в секундах; то есть разница между **joinDateTime** и **leaveDateTime.** |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceInterval"
}-->

```json

{
    "joinDateTime": "String (timestamp)",
    "leaveDateTime": "String (timestamp)",
    "durationInSeconds": "Int32"
}
    
```
