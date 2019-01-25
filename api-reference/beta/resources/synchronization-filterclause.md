---
title: Тип ресурса filterClause
description: Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523871"
---
# <a name="filterclause-resource-type"></a>Тип ресурса filterClause

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет один утверждения, в котором объект-кандидат должны соответствовать и вычисляется на любой `true` (объект должна удовлетворять утверждение) или `false` (объект не удовлетворяет утверждение).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
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
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
