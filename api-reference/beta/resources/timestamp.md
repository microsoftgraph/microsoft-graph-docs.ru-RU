---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
ms.openlocfilehash: 5f96ad5c557bda93ef74787d9d909fce112cfb15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341955"
---
# <a name="timestamp-resource-type"></a>Тип ресурса timeStamp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о дате и времени для определенного момента времени.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|date|Date|Часть даты метки времени.|
|time|TimeOfDay|Часть времени метки времени.|
|timeZone|String|Часть временной метки, представляющая часовой пояс (одна из 24 лонгитудинал областей мира).|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
