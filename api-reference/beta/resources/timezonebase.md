---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
localization_priority: Normal
ms.openlocfilehash: 8d968b8177da942c1b8940618c8ba965c362c914
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341871"
---
# <a name="timezonebase-resource-type"></a>Тип ресурса timeZoneBase

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Основное представление часового пояса.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| name | string | Имя часового пояса (стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс"). |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
