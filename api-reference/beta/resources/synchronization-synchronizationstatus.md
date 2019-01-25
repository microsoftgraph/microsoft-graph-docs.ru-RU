---
title: Тип ресурса synchronizationStatus
description: Представляет текущее состояние synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523766"
---
# <a name="synchronizationstatus-resource-type"></a>Тип ресурса synchronizationStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Описание    |
|:--------------------------------------|:----------|:---------------|
|code|String|Код высокого уровня состояния заданий синхронизации. Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|Последовательные время это задание не удалось.|
|escrowsPruned|Логическое|`true`Если задание escrows (ошибки уровня объекта) удаляются во время начальной синхронизации. Escrows можно удаляются при достижении порогового значения ошибок, которые обычно находится в карантине задание во время начальной синхронизации. Вдаваясь в карантин, процесс синхронизации очищает ошибок заданий и продолжает вплоть до завершения начальной синхронизации. После завершения начальной синхронизации задание приостановить и дождитесь клиента для очистки ошибки.|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Подробные сведения о последнего выполнения задания.|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Подробные сведения о последнего выполнения этого задания, не пришлось возникновения ошибок.|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Подробные сведения о последнего выполнения задания, которое экспортированных объектов в целевой каталог.|
|Progress|[synchronizationProgress](synchronization-synchronizationprogress.md) коллекции|Подробные сведения о ходе выполнения задания.|
|карантин|[synchronizationQuarantine](synchronization-quarantine.md)|Если задание находится в карантине, сведения о карантине.|
|steadyStateFirstAchievedTime|DateTimeOffset|Время, когда сначала достигнутым в стабильном состоянии (больше нет изменений для процесса). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|steadyStateLastAchievedTime|DateTimeOffset|Время, когда последнего достигнуть стабильном состоянии (больше нет изменений для процесса). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|synchronizedEntryCountByType|[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) коллекции|Количество синхронизированных объектов, перечисленные по типу объекта.|
|troubleshootingUrl|String|В случае ошибки, URL-адрес с помощью действия по устранению неполадок для проблему.|

### <a name="synchronization-status-code-details"></a>Сведения о коде состояния синхронизации

| Значение                              | Описание    |
|:-----------------------------------|:---------------|
|NotConfigured                       |Задание не настроен и ни разу. Не было указано. |
|NotRun                              |Задание был настроен и возможно работы, но еще не завершено его первого потока.|
|Активное                              |Задание выполняется периодически.|
|Приостановлена работа                              |Задание приостановлено (обычно администратором) и в настоящее время не работает, но сохранять состояние задания.|
|Карантин                          |Задание находится в карантине. Это может произойти при наличии большое количество ошибок или критические ошибки, такие как отозван Просроченные учетные данные. Находясь в карантин, процесс синхронизации будет пытаться с ограниченной частоту выполнения задания.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
