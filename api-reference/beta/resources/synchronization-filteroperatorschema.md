---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который может использоваться в фильтре.
localization_priority: Normal
ms.openlocfilehash: 0d26fb58b77369b70ab185fa8ad5214d6b6c1e71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848281"
---
# <a name="filteroperatorschema-resource-type"></a>Тип ресурса filterOperatorSchema

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает оператор, который можно использовать в [Фильтр](synchronization-filter.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:--------------------------|:---------------|
|арность                       |Строка          |Арность оператора. Возможные значения: `Binary`, `Unary`. Значение по умолчанию — `Binary`.|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |Возможные значения: `All`, `Any`. Применяется только к многозначных атрибутов. `All`означает, что все значения должны соответствовать условие. `Any`означает, что по крайней мере одно значение должен удовлетворяют условию. Значение по умолчанию — `All`.|
|name                        |Строка                     |Имя оператора. |
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
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
