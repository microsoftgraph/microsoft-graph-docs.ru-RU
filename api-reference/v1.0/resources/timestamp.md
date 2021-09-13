---
title: тип ресурса timeStamp
description: Сведения о дате и времени для точки времени.
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f284439f63d15c1cf6d070894a8f9f9074f69e24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59093990"
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

