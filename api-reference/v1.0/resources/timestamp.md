---
title: тип ресурса timeStamp
description: Сведения о дате и времени для точки времени.
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d2ec9f5906b3cbddb8d81a8f84d2699360adaa32
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694360"
---
# <a name="timestamp-resource-type"></a>тип ресурса timeStamp

Пространство имен: microsoft.graph

Сведения о дате и времени для точки времени.

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|date|Date|Дата части timestamp.|
|time|TimeOfDay|Временная часть времени.|
|timeZone|String|Часть часового пояса timestamp, которая является одним из 24 продоальных областей в мире.|

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
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

