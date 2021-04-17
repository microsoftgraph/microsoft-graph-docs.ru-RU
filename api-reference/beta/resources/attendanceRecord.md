---
title: тип ресурса attendanceRecord
description: Содержит сведения, связанные с записью посещаемости в отчете о посещаемости собрания.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 025c878d8778604bab34dda15f6ab0fa2c541151
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882695"
---
# <a name="attendancerecord-resource-type"></a>тип ресурса attendanceRecord

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, связанные с записью посещаемости в отчете о посещаемости собрания.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| удостоверение | [Идентификация](identity.md) | Идентификатор, например имя отображения. |
| emailAddress | String | Адрес электронной почты. |
| totalAttendanceInSeconds | Int32 | Общая продолжительность посещаемости в секундах. |
| attendanceIntervals | [коллекция attendanceInterval](attendanceInterval.md) | Список периодов времени между присоединением и отъездом. |
| role | Строка | Роль участника. Возможные значения `None` , `Attendee` и `Presenter` `Organizer` .  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceRecord"
}-->

```json

{
    "emailAddress": "String",
    "totalAttendanceInSeconds": "Int32",
    "role": "String(None|Attendee|Presenter|Organizer)",
    "identity": {"@odata.type": "#microsoft.graph.identity"},
    "attendanceIntervals": [{"@odata.type": "#microsoft.graph.attendanceInterval"}]
}

```
