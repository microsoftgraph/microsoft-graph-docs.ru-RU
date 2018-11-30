---
title: Тип ресурса filterClause
description: Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).
ms.openlocfilehash: 0861324849f224c4e750f0c7b926464280b9a377
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076033"
---
# <a name="filterclause-resource-type"></a>Тип ресурса filterClause

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|operatorName|String|Имя оператор, который должен применяться к исходной и целевой операндов. Должен быть один из поддерживаемых операторов. Для обнаружения поддерживаемых операторов.|
|sourceOperandName|String|Имя источника операнд (операнд проверяемой). Операнд имя источника должно соответствовать одному из имен атрибутов в объекте источника.|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|Значения, которые исходный операнд проверяется.|

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
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->