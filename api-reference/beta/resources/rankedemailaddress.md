---
title: Тип ресурса Ранкедемаиладдресс
description: Представляет ранжированный адрес электронной почты.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: f0311b379d2768a2dc704730b7547334e5a64c97
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811422"
---
# <a name="rankedemailaddress-resource-type"></a>Тип ресурса Ранкедемаиладдресс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ранжированный адрес электронной почты.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|string|Адрес электронной почты.|
|rank|double|Ранг адреса электронной почты. В качестве ключа сортировки используется ранг, связанный с другими возвращенными результатами. Более высокое значение соответствует более актуальному результату. Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
