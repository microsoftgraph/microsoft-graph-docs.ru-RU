---
title: Тип ресурса plannerAppliedCategories
description: Ресурс **AppliedCategoriesCollection** представляет коллекцию категорий (или метки), которые были применены к задаче. Он является частью объекта plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 604cf63d922ab59e038b5ccb8ea3b48a707a9bc0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981604"
---
# <a name="plannerappliedcategories-resource-type"></a>Тип ресурса plannerAppliedCategories


Ресурс **AppliedCategoriesCollection** представляет коллекцию категорий (или меток), примененных к задаче. Он является частью объекта [plannerTask](plannertask.md). К задаче можно применить до 6 категорий. Описания категорий, например `category1` и `category2`, являются частью объекта [сведений о плане](plannerplandetails.md). Это открытый тип.

## <a name="properties"></a>Свойства
Клиент может определять свойства открытого типа. В этом случае клиент должен указать значения для свойств `category1`, `category2`, `category3`, `category4`, `category5` или `category6`, а также использовать логическое значение `true` при применении соответствующих категорий к задаче. Ниже показан пример. Если не применить свойства, они будут автоматически удалены. Для этого им будет присвоено логическое значение `false`. 

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса в формате JSON

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
