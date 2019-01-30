---
title: Тип ресурса parseExpressionResponse
description: 'Представляет ответ от [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие.'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641059"
---
# <a name="parseexpressionresponse-resource-type"></a>Тип ресурса parseExpressionResponse

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ответ от [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|error|OData.Error|Дополнительные сведения об ошибке, если вычисление выражения возникла ошибка.|
|evaluationResult|Коллекция String|Коллекция значений, созданные средством оценки выражения.|
|evaluationSucceeded|Boolean|`true`При оценке прошла успешно.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Объект [attributeMappingSource](synchronization-attributemappingsource.md) , представляющий проанализированного выражения.|
|parsingSucceeded|Boolean|`true`Если выражение успешно обработан.|

## <a name="json-representation"></a>Представление JSON

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
