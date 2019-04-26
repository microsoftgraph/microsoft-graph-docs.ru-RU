---
title: Тип ресурса Филтерклаусе
description: Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).
localization_priority: Normal
ms.openlocfilehash: 657651af512fff0b1daf08985e0f14983ca253f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342977"
---
# <a name="filterclause-resource-type"></a>Тип ресурса Филтерклаусе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Операторнаме|String|Имя оператора, применяемого к исходному и целевому операндам. Должен быть одним из поддерживаемых операторов. Могут быть обнаружены поддерживаемые операторы.|
|Саурцеоперанднаме|String|Имя исходного операнда (тестируемого операнда). Имя исходного операнда должно быть соответствующим одному из имен атрибутов исходного объекта.|
|Таржетоперанд|[Филтероперанд](synchronization-filteroperand.md)|Значения, по которым будет выполняться тестирование исходного операнда.|

## <a name="json-representation"></a>Представление JSON

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
