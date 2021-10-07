---
title: тип ресурса propertyRule
description: Определяет набор условий для отображения displayTemplate
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7f1e021e4bc735ff7f5efd322e0a5a8080e5816b
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214941"
---
# <a name="propertyrule-resource-type"></a>тип ресурса propertyRule

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет набор условий для отображения [displayTemplate.](../resources/externalconnectors-displaytemplate.md) Правила используют формат: (свойство из схемы элемента) + (операция) + (значение). Например, **propertyRule может** указать, что "itemTitle" "содержит" "contoso". Поэтому **displayTemplate** не будет отображаться, если itemTitle не содержит значение "contoso".

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|операция|String|Указывает операции, выполняемые при оценке одного **свойстваRule,** где и строка из коллекции являются `property` `values` соответствующими оперантами. Возможные значения: `null`, `equals`, `notEquals`, `contains`, `notContains`, `lessThan`, `greaterThan`, `startsWith`, `unknownFutureValue`. Обязательный.|
|свойство|String|Свойство из [схемы externalItem.](../resources/externalconnectors-externalitem.md) Обязательный.|
|values|Коллекция строк|Коллекция с одной или многими строками. Указанная строка (ы) будет соответствовать указанному свойству с помощью указанной операции. Обязательный.|
|valuesJoinedBy|binaryOperator|Оператор join для оценки нескольких **свойствRules.** Например, если указано, то все свойстваRules должны быть верными, чтобы `and` **свойствоRule** было  верным. Возможные значения: `or`, `and`. Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.propertyRule"
}
-->
``` json
{
  "property": "String",
  "operation": "String",
  "valuesJoinedBy": "String",
  "values": [
    "String"
  ]
}
```

