---
title: тип ресурса meetingAttendanceReport
description: Содержит сведения, связанные с отчетом о посещаемости собрания.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f1ea75f6e57d0e095a470e715e080c7def05ab46
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896727"
---
# <a name="meetingattendancereport-resource-type"></a>тип ресурса meetingAttendanceReport

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, связанные с отчетом о посещаемости собрания.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| attendanceRecords           | [коллекция attendanceRecord](attendanceRecord.md)  | Список записей о посещаемости. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```json
{
  "attendanceRecords": [{"@odata.type": "#microsoft.graph.attendanceRecord"}]
}
```
