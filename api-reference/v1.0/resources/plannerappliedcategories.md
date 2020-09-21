---
title: Тип ресурса Планнерапплиедкатегориес
description: Ресурс **апплиедкатегориесколлектион** представляет коллекцию категорий (или меток), которые были применены к задаче. Он является частью объекта plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: fac4c69e9827e903d18f8665bc9b33e7c32705e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037628"
---
# <a name="plannerappliedcategories-resource-type"></a>Тип ресурса Планнерапплиедкатегориес

Пространство имен: microsoft.graph


Ресурс **апплиедкатегориесколлектион** представляет коллекцию категорий (или меток), которые были применены к задаче. Он является частью объекта [plannerTask](plannertask.md) .
К задаче может быть применено до 6 категорий. Описания категорий, например `category1` , и `category2` т. д., входят в состав объекта " [сведения о плане](plannerplandetails.md) ". Это открытый тип.

## <a name="properties"></a>Свойства
Клиентская возможность может определять свойства открытого типа. В этом случае клиент должен предоставлять `category1` , `category2` ,, `category3` `category4` `category5` и/или `category6` как свойства со своими значениями `true` Boolean при применении соответствующих категорий к задаче. Пример показан ниже. Если они не применяются, свойства автоматически удаляются путем присвоения их значений `false` логическому значению. 

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

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

