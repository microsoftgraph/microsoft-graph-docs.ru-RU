---
title: Тип ресурса filterGroup
description: Определяет набор условий, которые должны соответствовать объекта следует учитывать в области. Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.
localization_priority: Normal
ms.openlocfilehash: 174c02518069e949c49887d9e21e778e8455509a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836115"
---
# <a name="filtergroup-resource-type"></a>Тип ресурса filterGroup

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Определяет набор условий, которые должны соответствовать объекта следует учитывать в области. Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|предложения|[filterClause](synchronization-filterclause.md) коллекции|Фильтрация условия (условия) этой группы. Все предложения в группе должны быть выполнены в порядке для группы фильтра для вычисления `true`.|
|name|Строка|Понятное имя группы фильтра.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
