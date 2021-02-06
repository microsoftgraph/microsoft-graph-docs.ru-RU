---
title: Тип ресурса expressionInputObject
description: Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие synchronizationSchema parseExpression выполняет оценку выражения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 161589d9d8b6e3d06ef6afe31df0fde79bf938bb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132050"
---
# <a name="expressioninputobject-resource-type"></a>Тип ресурса expressionInputObject

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|definition|[objectDefinition](synchronization-objectdefinition.md)|Определение тестового объекта.|
|properties|[Коллекция stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)|Значения свойств тестового объекта.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


