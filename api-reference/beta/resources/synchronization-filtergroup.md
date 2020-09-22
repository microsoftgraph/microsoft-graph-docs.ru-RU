---
title: Тип ресурса Филтерграуп
description: Определяет набор предложений, которым должен удовлетворять объект, чтобы рассматриваться в области.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4dd174442cedf8f194bb9faf87d8e844b8c73163
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079767"
---
# <a name="filtergroup-resource-type"></a>Тип ресурса Филтерграуп

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет набор предложений, которым должен удовлетворять объект, чтобы рассматриваться в области. Объект рассматривается в области для группы (Группа оценивается как `true` ) только в том случае, если все предложения группы оцениваются `true` .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|предложения|Коллекция [филтерклаусе](synchronization-filterclause.md)|Предложения фильтра (условия) этой группы. Все предложения в группе должны быть удовлетворены для того, чтобы Группа фильтров вычислить значение `true` .|
|name|String|Понятное имя группы фильтров.|

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


