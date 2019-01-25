---
title: Тип ресурса plannerAppliedCategories
description: Ресурс **AppliedCategoriesCollection** представляет коллекцию категорий (или метки), которые были применены к задаче. Он является частью объекта plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b4e3ae92d179669d449d33c34ade4ae4476570fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517668"
---
# <a name="plannerappliedcategories-resource-type"></a>Тип ресурса plannerAppliedCategories

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **AppliedCategoriesCollection** представляет коллекцию категорий (или меток), примененных к задаче. Он является частью объекта [plannerTask](plannertask.md). К задаче можно применить до 6 категорий. Описания категорий, например `category1` и `category2`, являются частью объекта [сведений о плане](plannerplandetails.md). Это открытый тип.

## <a name="properties"></a>Свойства
Клиент может определять свойства открытого типа. В этом случае клиент должен указать значения для свойств `category1`, `category2`, `category3`, `category4`, `category5` или `category6`, а также использовать логическое значение `true` при применении соответствующих категорий к задаче. Ниже показан пример. Если не применить свойства, они будут автоматически удалены. Для этого им будет присвоено логическое значение `false`. 

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

Пример: 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerappliedcategories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
