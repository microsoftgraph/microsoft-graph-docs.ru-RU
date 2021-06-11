---
title: тип ресурса attendanceInterval
description: Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13b4e20a5233b865dd5417eed4d159bce07c8717
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896517"
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
