---
title: Тип ресурса Филтероператорсчема
description: Описывает оператор, который можно использовать в фильтре.
localization_priority: Normal
ms.openlocfilehash: 0f0ada4aaa02efa2484ffa75d88b2c8256f15fe8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342867"
---
# <a name="filteroperatorschema-resource-type"></a>Тип ресурса Филтероператорсчема

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает оператор, который можно использовать в фильтре [](synchronization-filter.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:--------------------------|:---------------|
|равн                       |String          |Арность оператора. Возможные значения: `Binary`, `Unary`. Значение по умолчанию: `Binary`.|
|Мултивалуедкомпарисонтипе   |Скопеоператормултивалуедкомпарисонтипе          |Возможные значения: `All`, `Any`. Применяется только к многозначным атрибутам. `All`означает, что все значения должны удовлетворять условию. `Any`Указывает, что по крайней мере одно значение должно удовлетворять условию. Значение по умолчанию: `All`.|
|name                        |String                     |Имя оператора. |
|Суппортедаттрибутетипес     |Коллекция String         |Типы атрибутов, поддерживаемые оператором. Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

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
  "suppressions": []
}
-->
