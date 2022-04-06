---
title: тип ресурса attendanceRecord
description: Содержит сведения, связанные с записью посещаемости в собранииAttendanceReport.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 957daa2412997f6db32de8f57ae196edd89e4b4e
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672086"
---
# <a name="attendancerecord-resource-type"></a>тип ресурса attendanceRecord

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| registrantId | String | Уникальный идентификатор [собранияRegistrant](meetingregistrantbase.md). Представляет, когда участник зарегистрировался для собрания. |
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
  "registrantId": "String",
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
