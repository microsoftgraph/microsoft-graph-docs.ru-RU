---
title: Тип ресурса synchronizationQuarantine
description: Предоставляет информацию о состоянии карантина synchronizationJob.
ms.openlocfilehash: b29da9644968ffe17abb02010f8aa5c304ca7905
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075608"
---
# <a name="synchronizationquarantine-resource-type"></a>Тип ресурса synchronizationQuarantine

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Предоставляет информацию о состоянии карантина [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|currentBegan|DateTimeOffset|Дата и время последнего карантина вычисляется и накладываемого. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|nextAttempt|DateTimeOffset|Дата и время, станут при следующей попытке выполните повторную оценку на карантин. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Причина|String|Код, который обозначает зачем накладываемого карантина. Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.|
|seriesBegan|DateTimeOffset|Дата и время, когда карантина был сначала установленных в этой серии (серии запускается при карантина сначала накладываемого и сброс сразу же удален карантина). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|seriesCount|Int64|Сколько раз в этой серии карантина было повторно вычисляется и фактически слева (серии запускается при карантина сначала накладываемого и сброс сразу же удален карантин).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->