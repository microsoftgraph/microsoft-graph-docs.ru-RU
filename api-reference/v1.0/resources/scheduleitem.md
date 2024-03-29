---
title: тип ресурса scheduleItem
description: Элемент, описывая доступность пользователя, соответствующего фактическому событию в календаре по умолчанию пользователя. Этот элемент также применяется к ресурсу (комната или оборудование).
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 86dc2c44f93635bd38363984d7dda8debe21147f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035971"
---
# <a name="scheduleitem-resource-type"></a>тип ресурса scheduleItem

Пространство имен: microsoft.graph

Элемент, описывая доступность пользователя, соответствующего фактическому событию в календаре по умолчанию пользователя. Этот элемент также применяется к ресурсу (комната или оборудование).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, который заканчивается соответствующим событием. |
|isPrivate |Логический |Чувствительность соответствующего события. True, если событие помечено `private` , ложное в противном случае. Необязательно.|
|location |Строка | Расположение, в котором проводится или посещается соответствующее событие. Необязательно.|
|начать |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в который начинается соответствующее событие. |
|status |freeBusyStatus | Состояние доступности пользователя или ресурса во время соответствующего события. Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | Строка субъекта соответствующего события. Необязательно.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

