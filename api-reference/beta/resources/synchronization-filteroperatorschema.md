---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который может использоваться в фильтре.
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515197"
---
# <a name="filteroperatorschema-resource-type"></a>Тип ресурса filterOperatorSchema

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает оператор, который можно использовать в [Фильтр](synchronization-filter.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:--------------------------|:---------------|
|арность                       |String          |Арность оператора. Возможные значения: `Binary`, `Unary`. Значение по умолчанию — `Binary`.|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |Возможные значения: `All`, `Any`. Применяется только к многозначных атрибутов. `All`означает, что все значения должны соответствовать условие. `Any`означает, что по крайней мере одно значение должен удовлетворяют условию. Значение по умолчанию — `All`.|
|name                        |String                     |Имя оператора. |
|supportedAttributeTypes     |Коллекция String         |Атрибут типы, которые поддерживаются оператором. Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperatorschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
