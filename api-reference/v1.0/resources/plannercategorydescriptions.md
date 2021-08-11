---
title: тип ресурса plannerCategoryDescriptions
description: 'Ресурс **plannerCategoryDescriptions** представляет описательные метки для категорий, определенных для плана. Он относится к объекту сведений плана. Может быть определено до 6 категорий. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5dcb6a9b2825b2a246f1bef9b55c453c6c53c1d8c6e56a45474bfa804d8caa15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54154919"
---
# <a name="plannercategorydescriptions-resource-type"></a>тип ресурса plannerCategoryDescriptions

Пространство имен: microsoft.graph

Ресурс **plannerCategoryDescriptions** представляет описательные метки для категорий, определенных для плана. Он относится к [объекту сведений плана.](plannerplandetails.md) Может быть определено до 6 категорий. 


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|category1|String|Метка, связанная с категорией 1|
|category2|String|Метка, связанная с категорией 2|
|category3|String|Метка, связанная с категорией 3|
|category4|String|Метка, связанная с категорией 4|
|category5|String|Метка, связанная с категорией 5|
|category6|String|Метка, связанная с категорией 6|

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

