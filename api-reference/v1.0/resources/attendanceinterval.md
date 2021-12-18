---
title: тип ресурса attendanceInterval
description: Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 643dcfa2e7c032fba93af164271150c41b6693b2
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547570"
---
# <a name="attendanceinterval-resource-type"></a>тип ресурса attendanceInterval

Пространство имен: microsoft.graph

Содержит сведения, связанные с интервалом посещаемости [в attendanceRecord](attendancerecord.md).

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| durationInSeconds | Int32 | Продолжительность интервала собрания в секундах; то есть разница между **joinDateTime** и **leaveDateTime.** |
| joinDateTime | DateTime | Время, когда участник присоединился к UTC. |
| leaveDateTime | DateTime | Время, когда участник покинул UTC. |

> [!TIP]
> При отсутствии данных будет установлено значение **joinDateTime** или **leaveDateTime,** а значение длительностиInSeconds будет задавано в ответном органе метода `null` Get  `0` [meetingAttendanceReport.](/graph/api/meetingattendancereport-get?view=graph-rest-v1.0&preserve-view=true)

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
