---
title: тип ресурса attendanceInterval
description: Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 55b218cfcecb4f2f7d3d597881b612e36fe42860
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979252"
---
# <a name="attendanceinterval-resource-type"></a>тип ресурса attendanceInterval

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| joinDateTime | Даты и время | Участник time присоединился к UTC. |
| leaveDateTime | Даты и время | Время участника, оставленного в UTC. |
| durationInSeconds | Int32 | Продолжительность интервала собрания в секундах; то есть разница между **joinDateTime** и **leaveDateTime.** |

> [!TIP]
> При отсутствии данных будет задано значение **joinDateTime** или **leaveDateTime,** а значение продолжительностиInSeconds будет задат в ответном органе операции "Получить отчет о посещаемости `null`  `0` собрания". [](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true)

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
