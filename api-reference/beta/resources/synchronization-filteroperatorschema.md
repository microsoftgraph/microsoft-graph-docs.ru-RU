---
title: Тип ресурса filterOperatorSchema
description: Описывает оператор, который можно использовать в фильтре.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1128b12ffcadd36f2fdd2f34d27f95d973cdfd9d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131889"
---
# <a name="filteroperatorschema-resource-type"></a>Тип ресурса filterOperatorSchema

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает оператор, который можно использовать в [фильтре.](synchronization-filter.md)

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:--------------------------|:---------------|
|arity                       |Строка          |Arity of the operator. Возможные значения: `Binary`, `Unary`. Значение по `Binary` умолчанию: .|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |Возможные значения: `All`, `Any`. Применяется только к многоценным атрибутам. `All` означает, что все значения должны удовлетворять условию. `Any` означает, что условие должно удовлетворять хотя бы одному значению. Значение по `All` умолчанию: .|
|name                        |String                     |Имя оператора. |
|supportedAttributeTypes     |Коллекция объектов string         |Типы атрибутов, поддерживаемые оператором. Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": []
}
-->


