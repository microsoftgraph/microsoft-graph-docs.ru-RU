---
title: Тип ресурса synchronizationSchedule
description: Определяет расписание, используемая для запуска synchronizationJob.
ms.openlocfilehash: c0435b3957f138751f34a1e0e522683b352294da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078568"
---
# <a name="synchronizationschedule-resource-type"></a>Тип ресурса synchronizationSchedule

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Определяет расписание, используемая для запуска [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|истечение срока действия|DateTimeOffset|Дата и время истечения срока действия этого задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|interval|Продолжительность|Интервал между итерациями синхронизации.|
|state|String| Возможные значения: `Active`, `Disabled`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->