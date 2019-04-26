---
title: Тип ресурса Ранкедемаиладдресс
description: Представляет ранжированный адрес электронной почты.
localization_priority: Normal
ms.openlocfilehash: 0c92f46c587b4f615b640e47b8d82a33aefc5e50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344111"
---
# <a name="rankedemailaddress-resource-type"></a>Тип ресурса Ранкедемаиладдресс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ранжированный адрес электронной почты.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|string|Адрес электронной почты.|
|rank|double|Ранг адреса электронной почты. В качестве ключа сортировки используется ранг, связанный с другими возвращенными результатами. Более высокое значение соответствует более актуальному результату. Релевантность определяется сигналами связи, сотрудничества и рабочих отношений.|

## <a name="json-representation"></a>Представление JSON

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
