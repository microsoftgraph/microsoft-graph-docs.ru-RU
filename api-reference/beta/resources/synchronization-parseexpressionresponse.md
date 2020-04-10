---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия Синчронизатионсчема: Парсикспрессион.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ef96bda8e9e28c655c4bbcf0153ea83ef5b0c8e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217607"
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
|евалуатионсукцеедед|Boolean|`true`, если оценка выполнена успешно.|
|парседекспрессион|[аттрибутемаппингсаурце](synchronization-attributemappingsource.md)|Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.|
|парсингсукцеедед|Boolean|`true`, если выражение было успешно проанализировано.|

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
