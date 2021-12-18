---
title: тип ресурса attendanceRecord
description: Содержит сведения, связанные с записью посещаемости в собранииAttendanceReport.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3771dda15dbcb56fabc7cfdefa6a105268d9c77e
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547577"
---
# <a name="attendancerecord-resource-type"></a>тип ресурса attendanceRecord

Пространство имен: microsoft.graph

Содержит сведения, связанные с записью посещаемости [в собранииAttendanceReport](meetingattendancereport.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список посещаемостиRecords](../api/attendancerecord-list.md)|[коллекция attendanceRecord](../resources/attendancerecord.md)|Получите список объектов [attendanceRecord](../resources/attendancerecord.md) и их свойств.|

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| attendanceIntervals | [коллекция attendanceInterval](attendanceinterval.md) | Список периодов времени между присоединением и выходом из собрания. |
| emailAddress | String | Адрес электронной почты пользователя, связанного с этой записью atttendance. |
| удостоверение | [identity](identity.md) | Удостоверение пользователя, связанного с этой записью atttendance. |
| role | Строка | Роль участника. Возможные значения: `None`, `Attendee`, `Presenter` и `Organizer`.  |
| totalAttendanceInSeconds | Int32 | Общая продолжительность посещаемости в секундах. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attendanceRecord",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.attendanceRecord",
  "emailAddress": "String",
  "totalAttendanceInSeconds": "Int32",
  "role": "String(None|Attendee|Presenter|Organizer)",
  "identity": {
    "@odata.type": "#microsoft.graph.identity"
  },
  "attendanceIntervals": [
    {
      "@odata.type": "#microsoft.graph.attendanceInterval"
    }
  ]
}
```
