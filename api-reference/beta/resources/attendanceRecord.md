---
title: тип ресурса attendanceRecord
description: Содержит сведения, связанные с записью посещаемости в отчете о посещаемости собрания.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20beeca97c790b8743c9038e7fddf0b5c6f69534
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896503"
---
# <a name="attendancerecord-resource-type"></a>тип ресурса attendanceRecord

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, связанные с записью посещаемости в отчете о посещаемости собрания.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| удостоверение | [Identity](identity.md) | Идентификатор, например имя отображения. |
| emailAddress | String | Адрес электронной почты. |
| totalAttendanceInSeconds | Int32 | Общая продолжительность посещаемости в секундах. |
| attendanceIntervals | [коллекция attendanceInterval](attendanceInterval.md) | Список периодов времени между присоединением и отъездом. |
| role | String | Роль участника. Возможные значения `None` , `Attendee` и `Presenter` `Organizer` .  |

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
