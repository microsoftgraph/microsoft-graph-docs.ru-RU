---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который может использоваться в фильтре.
ms.openlocfilehash: 1a4e21aea2b65073a00c9797065f6788a66e2334
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076037"
---
# <a name="filteroperatorschema-resource-type"></a>Тип ресурса filterOperatorSchema

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описывает оператор, который можно использовать в [Фильтр](synchronization-filter.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Description    |
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
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->