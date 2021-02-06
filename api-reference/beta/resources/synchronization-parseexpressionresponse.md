---
title: Тип ресурса parseExpressionResponse
description: 'Представляет ответ от действия synchronizationSchema: parseExpression.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: e564cb2ad7a80c91fec7d6298254fa19bde4537c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133149"
---
# <a name="parseexpressionresponse-resource-type"></a>Тип ресурса parseExpressionResponse

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ответ от действия [parseExpression.](../api/synchronization-synchronizationschema-parseexpression.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|error|publicError|Сведения об ошибке, если оценка выражения приводит к ошибке.|
|evaluationResult|Коллекция объектов string|Коллекция значений, производимых при оценке выражения.|
|evaluationSucceeded|Boolean|`true` если оценка прошла успешно.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Объект [attributeMappingSource,](synchronization-attributemappingsource.md) представляющий выражение с разчетом.|
|parsingSucceeded|Boolean|`true` если выражение было успешно разлино.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


