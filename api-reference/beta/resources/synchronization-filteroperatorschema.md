---
title: Тип ресурса Филтероператорсчема
description: Описывает оператор, который можно использовать в фильтре.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e80b80a7f37af8b86dfd3925fe268dba89cea17
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217814"
---
# <a name="filteroperatorschema-resource-type"></a>Тип ресурса Филтероператорсчема

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает оператор, который можно использовать в [фильтре](synchronization-filter.md).

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:--------------------------|:---------------|
|равн                       |Строка          |Арность оператора. Возможные значения: `Binary`, `Unary`. Значение по умолчанию: `Binary`.|
|мултивалуедкомпарисонтипе   |скопеоператормултивалуедкомпарисонтипе          |Возможные значения: `All`, `Any`. Применяется только к многозначным атрибутам. `All`означает, что все значения должны удовлетворять условию. `Any`Указывает, что по крайней мере одно значение должно удовлетворять условию. Значение по умолчанию: `All`.|
|name                        |String                     |Имя оператора. |
|суппортедаттрибутетипес     |Коллекция String         |Типы атрибутов, поддерживаемые оператором. Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

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
