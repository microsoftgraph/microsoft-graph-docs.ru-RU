---
title: тип ресурса synchronizationQuarantine
description: Предоставляет сведения о состоянии карантина синхронизацииJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 45381594a242251995de3d43bb7fd02e0638484b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720503"
---
# <a name="synchronizationquarantine-resource-type"></a>тип ресурса synchronizationQuarantine

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о состоянии карантина [синхронизацииJob.](synchronization-synchronizationjob.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|currentBegan|DateTimeOffset|Дата и время последней оценки и введения карантина. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|nextAttempt|DateTimeOffset|Дата и время, когда будет предпринята следующая попытка повторной оценки карантина. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|reason|String|Код, который означает, почему был введен карантин. Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.|
|seriesBegan|DateTimeOffset|Дата и время, когда карантин был впервые введен в этой серии (серия начинается при первом введении карантина и сбрасывается, как только карантин отменяется). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|seriesCount|Int64|Количество раз в этой серии карантин был повторно оценен и оставлен в силе (серия начинается при первом введении карантина и сбрасывается, как только карантин отменяется).|
|error|[синхронизацияError](synchronization-synchronizationerror.md)|Описывает ошибку(ы), которая произошла при вводе задания синхронизации в карантин.|

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
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


