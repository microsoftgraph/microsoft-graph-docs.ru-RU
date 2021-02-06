---
title: Тип ресурса synchronizationStatus
description: Представляет текущее состояние synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bb832fa8d62f2c666b430c242a49bd9138de1b57
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135053"
---
# <a name="synchronizationstatus-resource-type"></a>Тип ресурса synchronizationStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние [synchronizationJob.](synchronization-synchronizationjob.md)

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Описание    |
|:--------------------------------------|:----------|:---------------|
|code|Строка|Высокоуровневый код состояния задания синхронизации. Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|Количество последовательных сбойов этого задания.|
|escrowsPruned|Boolean|`true` если объектные объекты задания (ошибки на уровне объекта) были обрезаются во время начальной синхронизации. Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine. Вместо того чтобы ходить в карантин, процесс синхронизации очищает ошибки задания и продолжается до завершения начальной синхронизации. После завершения начальной синхронизации задание будет приостановлено и будет ждать, пока клиент очистит ошибки.|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении задания.|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении этого задания без ошибок.|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении задания, которое экспортирует объекты в целевой каталог.|
|progress|[Коллекция synchronizationProgress](synchronization-synchronizationprogress.md)|Сведения о ходе выполнения задания.|
|карантин|[synchronizationQuarantine](synchronization-quarantine.md)|Если задание находится в карантине, сведения о карантине.|
|steadyStateFirstAchievedTime|DateTimeOffset|Время, когда было достигнуто стабильное состояние (больше не внося изменений в процесс). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|steadyStateLastAchievedTime|DateTimeOffset|Время последнего достижения устойчивого состояния (без изменений в процессе). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|synchronizedEntryCountByType|[Коллекция stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)|Количество синхронизированных объектов, перечисленных по типу объекта.|
|troubleshootingUrl|Строка|В случае ошибки URL-адрес с действиями по устранению неполадок для проблемы.|

### <a name="synchronization-status-code-details"></a>Сведения о коде состояния синхронизации

| Значение                              | Описание    |
|:-----------------------------------|:---------------|
|NotConfigured                       |Задание не было настроено и никогда не запускалось. Авторизация не предоставлена. |
|NotRun                              |Задание было настроено и, возможно, запущено, но не завершило свой первый запуск.|
|Активное                              |Задание работает периодически.|
|Приостановлено                              |Задание было приостановлено (обычно администратором) и в настоящее время не запущено, но состояние задания сохраняется.|
|Карантин                          |Задание находится в карантине. Это может произойти в случае большого объема ошибок или критических ошибок, таких как отозванные или просроченные учетные данные. В карантине процесс синхронизации попытается выполнить задание с уменьшенной частотой.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": []
}
-->


