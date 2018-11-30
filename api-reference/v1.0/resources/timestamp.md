---
title: Тип ресурса метки времени
description: Дата и время сведения о времени.
ms.openlocfilehash: 4f392e880bb165841fd8a9a31b6ed00bf2ba36fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025132"
---
# <a name="timestamp-resource-type"></a>Тип ресурса метки времени

Дата и время сведения о времени.

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
|date|Date|Часть date метка времени.|
|time|TimeOfDay|Часть времени метка времени.|
|timeZone|String|Часовой пояс часть метки времени — это один из 24 продольными областей в мире.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->