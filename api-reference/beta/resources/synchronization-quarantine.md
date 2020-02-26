---
title: Тип ресурса Синчронизатионкуарантине
description: Предоставляет сведения о состоянии карантина Синчронизатионжоб.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5e36d62c26225a3dda5fe0adb4610c56c226b79
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280703"
---
# <a name="synchronizationquarantine-resource-type"></a>Тип ресурса Синчронизатионкуарантине

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о состоянии карантина [синчронизатионжоб](synchronization-synchronizationjob.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|куррентбеган|DateTimeOffset|Дата и время последнего вычисления и ликвидации карантина. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|некстаттемпт|DateTimeOffset|Дата и время следующей попытки повторной оценки карантина. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|reason|String|Код, обозначающий, почему был наложен карантин. Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.|
|сериесбеган|DateTimeOffset|Дата и время первого помещения карантина в этот цикл (ряд начинается при первом включении карантина и сбрасывается, как только будет ликвидируется карантин). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|сериескаунт|Int64|Количество повторных попыток вычисления и вступления в действия карантина для этой серии (ряд начинается при первом включении карантина и сбрасывается, как только приликвидируется карантин).|
|error|[синчронизатионеррор](synchronization-synchronizationerror.md)|Описывает ошибки, которые произошли при переводе задания синхронизации в карантин.|

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
