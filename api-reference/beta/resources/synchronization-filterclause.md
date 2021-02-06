---
title: Тип ресурса filterClause
description: Представляет одно утверждение, которое должен удовлетворять объект-кандидат.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc633f6e25373713679da30a5b319ab8ae99fb04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131924"
---
# <a name="filterclause-resource-type"></a>Тип ресурса filterClause

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет одно утверждение, которое должно удовлетворяться объектом-кандидатом, и оценивается либо (объект удовлетворяет утверждению), либо (объект не удовлетворяет `true` `false` утверждению).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|operatorName|Строка|Имя оператора, применяемого к исходным и целевым операндам. Должен быть одним из поддерживаемых операторов. Поддерживаемые операторы можно обнаружить.|
|sourceOperandName|Строка|Имя операнда источника (проверяемого операнда). Имя операнда источника должно соответствовать одному из имен атрибутов в объекте-источнике.|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|Значения, с которые будет тестироваться исходный операнд.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


