---
title: Тип ресурса plannerCategoryDescriptions
description: 'Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту сведений о плане. Можно задать до 6 категорий. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1cf1ee1c6e8ccc4e90f78985b352062fce37df88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984348"
---
# <a name="plannercategorydescriptions-resource-type"></a>Тип ресурса plannerCategoryDescriptions

Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту [сведений о плане](plannerplandetails.md). Можно задать до 6 категорий. 


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|category1|String|Метка, сопоставленная с категорией 1.|
|category2|String|Метка, сопоставленная с категорией 2.|
|category3|String|Метка, сопоставленная с категорией 3.|
|category4|String|Метка, сопоставленная с категорией 4.|
|category5|String|Метка, сопоставленная с категорией 5.|
|category6|String|Метка, сопоставленная с категорией 6.|

## <a name="json-representation"></a>Представление в формате JSON
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
