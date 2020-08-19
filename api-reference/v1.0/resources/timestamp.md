---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0629eaabd282f03184be28ade67c2d17d5598602
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808146"
---
# <a name="timestamp-resource-type"></a>Тип ресурса timeStamp

Пространство имен: microsoft.graph

Сведения о дате и времени для определенного момента времени.

## <a name="json-representation"></a>Представление в формате JSON

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
