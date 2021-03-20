---
title: тип ресурса threatAssessmentResult
description: Представляет элемент результатов оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b127de108633389342a5d21ff8fac7d5e670b395
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952496"
---
# <a name="threatassessmentresult-resource-type"></a>тип ресурса threatAssessmentResult

Представляет элемент результатов оценки угроз.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String|Идентификатор результатов оценки угроз — это уникальный идентификатор глобального идентификатора (GUID).|
|message|String|Сообщение результата для каждой оценки угрозы.|
|resultType|[threatAssessmentResultType](enums.md#threatassessmentresulttype-values)|Тип результатов оценки угроз. Возможные значения: `checkPolicy`, `rescan`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "message": "String",
  "resultType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "threatAssessmentResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

