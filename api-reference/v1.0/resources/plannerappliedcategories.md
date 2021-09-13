---
title: тип ресурса plannerAppliedCategories
description: Ресурс **AppliedCategoriesCollection** представляет коллекцию категорий (или меток), которые были применены к задаче. Это часть объекта plannerTask.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7095c2f2069b89009c9f8cdbe5908812dd03620f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044400"
---
# <a name="plannerappliedcategories-resource-type"></a>тип ресурса plannerAppliedCategories

Пространство имен: microsoft.graph


Ресурс **AppliedCategoriesCollection** представляет коллекцию категорий (или меток), которые были применены к задаче. Это часть объекта [plannerTask.](plannertask.md)
К задаче может применяться до 6 категорий. Описания категорий, `category1` например, и `category2` т.д., являются частью объекта [сведений плана.](plannerplandetails.md) Это открытый тип.

## <a name="properties"></a>Свойства
Свойства открытого типа могут быть определены клиентом. В этом случае, однако, клиент должен предоставить , , , и / или как свойства с их значениями быть `category1` `category2` `category3` `category4` `category5` `category6` `true` boolean, когда соответствующие категории применяются к задаче. Пример показан ниже. Если они не применяются, свойства автоматически удаляются, устанавливая их значения в `false` boolean. 

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

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

