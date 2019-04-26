---
title: Тип ресурса Планнерапплиедкатегориес
description: Ресурс **апплиедкатегориесколлектион** представляет коллекцию категорий (или меток), которые были применены к задаче. Он является частью объекта plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a927adb78bc0fe1c5135281043ecbdd3afe09a60
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344627"
---
# <a name="plannerappliedcategories-resource-type"></a>Тип ресурса Планнерапплиедкатегориес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **апплиедкатегориесколлектион** представляет коллекцию категорий (или меток), которые были применены к задаче. Он является частью объекта [plannerTask](plannertask.md) .
К задаче может быть применено до 6 категорий. Описания категорий, например `category1`, `category2` и т. д., входят в состав объекта " [сведения о плане](plannerplandetails.md) ". Это открытый тип.

## <a name="properties"></a>Свойства
Клиентская возможность может определять свойства открытого типа. `category1`В этом случае клиент должен предоставлять, `category2`, `category3` `category4`, `category5` и/или `category6` как свойства со своими значениями `true` Boolean при применении соответствующих категорий к задаче. Пример показан ниже. Если они не применяются, свойства автоматически удаляются путем присвоения их значений `false` логическому значению. 

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

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

Пример. 

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
  "suppressions": []
}
-->
