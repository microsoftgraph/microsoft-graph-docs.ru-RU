---
title: тип ресурса timeStamp
description: Сведения о дате и времени для точки времени.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a07dc3c6c1aa9bc787bed2e519ce8d4e7db4d582637fe2fdfbf41e79789a52f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163623"
---
# <a name="timestamp-resource-type"></a>тип ресурса timeStamp

Пространство имен: microsoft.graph

Сведения о дате и времени для точки времени.

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
|date|Date|Дата части timestamp.|
|time|TimeOfDay|Временная часть времени.|
|timeZone|String|Часть часового пояса timestamp, которая является одним из 24 продоальных областей в мире.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

