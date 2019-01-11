---
title: Тип ресурса parseExpressionResponse
description: 'Представляет ответ от [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие.'
localization_priority: Normal
ms.openlocfilehash: 550a46b0c27c2ca8d2d4c01baa975d8a204546f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832951"
---
# <a name="parseexpressionresponse-resource-type"></a>Тип ресурса parseExpressionResponse

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ответ от [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) действие.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|error|OData.Error|Дополнительные сведения об ошибке, если вычисление выражения возникла ошибка.|
|evaluationResult|Коллекция String|Коллекция значений, созданные средством оценки выражения.|
|evaluationSucceeded|Логический|`true`При оценке прошла успешно.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Объект [attributeMappingSource](synchronization-attributemappingsource.md) , представляющий проанализированного выражения.|
|parsingSucceeded|Логический|`true`Если выражение успешно обработан.|

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
