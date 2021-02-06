---
title: Тип ресурса filterGroup
description: Определяет набор предложений, которые должны удовлетворяться объектом, чтобы считаться в области.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6338ae4b02b79d1512d5e9f695a69155197e2f4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131917"
---
# <a name="filtergroup-resource-type"></a>Тип ресурса filterGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет набор предложений, которые должны удовлетворяться объектом, чтобы считаться в области. Объект рассматривается в области для группы (группа оценивается как ) только в том случае, если все предложения группы `true` оцениваются как `true` .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|clauses|[Коллекция filterClause](synchronization-filterclause.md)|Условия фильтра для этой группы. Все предложения в группе должны быть выполнены, чтобы группа фильтров оценивалась как `true` .|
|name|String|Понятное для человека имя группы фильтров.|

## <a name="json-representation"></a>Представление в формате JSON

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
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


