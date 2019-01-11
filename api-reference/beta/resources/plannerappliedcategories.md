---
title: Тип ресурса plannerAppliedCategories
description: Ресурс **AppliedCategoriesCollection** представляет коллекцию категорий (или метки), которые были применены к задаче. Он является частью объекта plannerTask.
localization_priority: Normal
ms.openlocfilehash: a47317f907b8ee934a59a320af67e94ce6d3bf8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856016"
---
# <a name="plannerappliedcategories-resource-type"></a>Тип ресурса plannerAppliedCategories

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
