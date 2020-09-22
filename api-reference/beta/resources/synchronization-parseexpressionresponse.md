---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия Синчронизатионсчема: Парсикспрессион.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bd675b079f42856e85f54b7da84a091a0f57f4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988816"
---
# <a name="parseexpressionresponse-resource-type"></a>Тип ресурса Парсикспрессионреспонсе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отклик от действия [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|error|публицеррор|Сведения об ошибке, если вычисление выражений привело к ошибке.|
|евалуатионресулт|Коллекция String|Коллекция значений, полученных при оценке выражения.|
|евалуатионсукцеедед|Boolean|`true` , если оценка выполнена успешно.|
|парседекспрессион|[аттрибутемаппингсаурце](synchronization-attributemappingsource.md)|Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.|
|парсингсукцеедед|Boolean|`true` , если выражение было успешно проанализировано.|

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
  "suppressions": []
}
-->


