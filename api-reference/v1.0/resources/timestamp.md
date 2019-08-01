---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33dbc9821d2a58763d81249aebe21a9a2c3aee08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033588"
---
# <a name="timestamp-resource-type"></a>Тип ресурса timeStamp

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
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|date|Date|Часть даты метки времени.|
|time|TimeOfDay|Часть времени метки времени.|
|timeZone|String|Часть временной метки, представляющая часовой пояс (одна из 24 лонгитудинал областей мира).|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
