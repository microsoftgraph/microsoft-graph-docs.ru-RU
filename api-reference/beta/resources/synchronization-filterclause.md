---
title: Тип ресурса Филтерклаусе
description: Представляет одно утверждение, которое должен удовлетворять объект-кандидат, и оценивается как `true` (объект соответствует утверждению) или `false` (объект не соответствует утверждению).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 788dcd8741d89639ce2c57511ae54e466815e366
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621426"
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
