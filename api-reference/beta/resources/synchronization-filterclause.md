---
title: Тип ресурса Филтерклаусе
description: Представляет одно утверждение, которое должен удовлетворять объект Candidate.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91cc7f85dc4c42f806be5e365f21adb0d5e972fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968376"
---
# <a name="filterclause-resource-type"></a>Тип ресурса Филтерклаусе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|операторнаме|String|Имя оператора, применяемого к исходному и целевому операндам. Должен быть одним из поддерживаемых операторов. Могут быть обнаружены поддерживаемые операторы.|
|саурцеоперанднаме|String|Имя исходного операнда (тестируемого операнда). Имя исходного операнда должно быть соответствующим одному из имен атрибутов исходного объекта.|
|таржетоперанд|[филтероперанд](synchronization-filteroperand.md)|Значения, по которым будет выполняться тестирование исходного операнда.|

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


