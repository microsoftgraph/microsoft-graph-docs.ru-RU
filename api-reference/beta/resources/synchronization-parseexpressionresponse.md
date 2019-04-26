---
title: Тип ресурса Парсикспрессионреспонсе
description: 'Представляет отклик от действия [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
ms.openlocfilehash: 14fcce13d2e78b99a8712c51768e6a94928fa07f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345560"
---
# <a name="parseexpressionresponse-resource-type"></a>Тип ресурса Парсикспрессионреспонсе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отклик от действия [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|error|Публицеррор|Сведения об ошибке, если вычисление выражений привело к ошибке.|
|Евалуатионресулт|Коллекция String|Коллекция значений, полученных при оценке выражения.|
|Евалуатионсукцеедед|Логический|`true`, если оценка выполнена успешно.|
|Парседекспрессион|[Аттрибутемаппингсаурце](synchronization-attributemappingsource.md)|Объект [аттрибутемаппингсаурце](synchronization-attributemappingsource.md) , представляющий проанализированное выражение.|
|Парсингсукцеедед|Логический|`true`, если выражение было успешно проанализировано.|

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
