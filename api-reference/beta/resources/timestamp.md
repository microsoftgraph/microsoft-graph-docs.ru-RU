---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для точки во времени.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
author: JeremyKelley
ms.openlocfilehash: fb82ddf1e69b8ea06cb425ed5199d1f6c5862b52
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66737107"
---
# <a name="timestamp-resource-type"></a>Тип ресурса timeStamp

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о дате и времени для точки во времени.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|date|Date|Часть даты метки времени.|
|time|TimeOfDay|Часть времени метки времени.|
|timeZone|String|Часть часового пояса метки времени, которая является одной из 24 длинных областей в мире.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

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


