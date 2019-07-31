---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a2c2bc0291eca7c04f246c6f62424b0bab10dced
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964783"
---
# <a name="parseexpressionresponse-resource-type"></a>Тип ресурса Парсикспрессионреспонсе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отклик от действия [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|error|Публицеррор|Сведения об ошибке, если вычисление выражений привело к ошибке.|
|Евалуатионресулт|Коллекция строк|Коллекция значений, полученных при оценке выражения.|
|Евалуатионсукцеедед|Boolean|`true`, если оценка выполнена успешно.|
|Парседекспрессион|[Аттрибутемаппингсаурце](synchronization-attributemappingsource.md)|Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.|
|Парсингсукцеедед|Boolean|`true`, если выражение было успешно проанализировано.|

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
