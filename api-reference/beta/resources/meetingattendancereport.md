---
title: тип ресурса meetingAttendanceReport
description: Содержит сведения, связанные с отчетом о посещаемости собрания.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a46ab1bcdb0c8a901b5257184e96b72c79801ce7
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547695"
---
# <a name="meetingattendancereport-resource-type"></a>тип ресурса meetingAttendanceReport

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, связанные с отчетом о посещаемости собрания.

Отчеты о посещаемости собраний — это артефакты собраний в Интернете. Подробные сведения см. [в материале Online meeting artifacts and permissions.](/graph/cloud-communications-online-meeting-artifacts)

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[List meetingAttendanceReports](../api/meetingattendancereport-list.md)|[коллекция meetingAttendanceReport](../resources/meetingattendancereport.md)|Получите список объектов  [meetingAttendanceReport](../resources/meetingattendancereport.md) и их свойств.|
|[Get meetingAttendanceReport](../api/meetingattendancereport-get.md)|[meetingAttendanceReport](../resources/meetingattendancereport.md)|Ознакомьтесь с свойствами и отношениями объекта [meetingAttendanceReport.](../resources/meetingattendancereport.md)|

## <a name="properties"></a>Свойства

| Свойство              | Тип                                               | Описание                     |
|:----------------------|:---------------------------------------------------|:--------------------------------|
| id                    | Строка   | Уникальный идентификатор отчета о посещаемости. Только для чтения. |
| meetingEndDateTime    | DateTimeOffset | Время UTC по завершению собрания. Только для чтения.   |
| meetingStartDateTime  | DateTimeOffset | Время UTC при начале собрания. Только для чтения.   |
| totalParticipantCount | Int32 | Общее число участников. Только для чтения.  |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
| ------------ | ---- | ----------- |
| attendanceRecords | [коллекция attendanceRecord](attendanceRecord.md) | Список записей о посещаемости отчета о посещаемости. Только для чтения. |

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
  "@odata.type": "#microsoft.graph.meetingAttendanceReport",
  "id": "String(identifier)",
  "meetingEndDateTime": "String (timestamp)",
  "meetingStartDateTime": "String (timestamp)",
  "totalParticipantCount": "Int32",

  "attendanceRecords": [{"@odata.type": "#microsoft.graph.attendanceRecord"}]
}
```
