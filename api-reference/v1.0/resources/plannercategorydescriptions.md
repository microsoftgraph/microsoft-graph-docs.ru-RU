---
title: Тип ресурса Планнеркатегоридескриптионс
description: 'Ресурс **планнеркатегоридескриптионс** представляет описательные метки для категорий, определенных для плана. Он принадлежит объекту сведений о плане. Может быть определено до 6 категорий. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7543b231fbad190be6ad7840611aec034adae053
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035310"
---
# <a name="plannercategorydescriptions-resource-type"></a>Тип ресурса Планнеркатегоридескриптионс

Ресурс **планнеркатегоридескриптионс** представляет описательные метки для категорий, определенных для плана. Он принадлежит объекту [сведений о плане](plannerplandetails.md) . Может быть определено до 6 категорий. 


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Category1|String|Метка, связанная с категорией 1|
|category2|String|Метка, сопоставленная с категорией 2|
|category3|String|Метка, связанная с категорией 3|
|category4|String|Метка, сопоставленная с категорией 4|
|category5|String|Метка, сопоставленная с категорией 5|
|category6|String|Метка, сопоставленная с категорией 6|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
