---
title: Тип ресурса Синчронизатионстатус
description: Представляет текущее состояние Синчронизатионжоб.
localization_priority: Normal
ms.openlocfilehash: 042dd05eb5633573a15eeb663b032ed531636aab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339845"
---
# <a name="synchronizationstatus-resource-type"></a>Тип ресурса Синчронизатионстатус

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние [синчронизатионжоб](synchronization-synchronizationjob.md).

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Описание    |
|:--------------------------------------|:----------|:---------------|
|code|String|Высокий уровень кода состояния задания синхронизации. Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|Каунтсукцессивекомплетефаилурес|Int64|Количество последовательных попыток выполнения этого задания.|
|Ескровспрунед|Логический|`true`значение, которое было удаляться из-за ошибок на уровне объектов во время первоначальной синхронизации. Если во время первоначальной синхронизации вы повлияете на пороговое значение, то получится пороговое значение ошибок, которые обычно помещают в карантин. Вместо того чтобы переходить в карантин, процесс синхронизации очищает ошибки задания и продолжается до завершения первоначальной синхронизации. После завершения первоначальной синхронизации задание будет приостановлено и ждать, пока клиент очистит ошибки.|
|Ластексекутион|[Синчронизатионтаскексекутион](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении задания.|
|Ластсукцессфулексекутион|[Синчронизатионтаскексекутион](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении задания, у которого нет ошибок.|
|Ластсукцессфулексекутионвисекспортс|[Синчронизатионтаскексекутион](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении задания, экспортируемые объекты в целевой каталог.|
|progress|Коллекция [синчронизатионпрогресс](synchronization-synchronizationprogress.md)|Сведения о ходе выполнения задания в направлении завершения.|
|папку|[Синчронизатионкуарантине](synchronization-quarantine.md)|Если задание находится в карантине, сведения о карантине.|
|Стеадистатефирстачиеведтиме|DateTimeOffset|Время, в течение которого было выполнено стабильное состояние (больше изменений процесса). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Стеадистателастачиеведтиме|DateTimeOffset|Время, в течение которого было последнее время последнего изменения процесса (без дополнительных изменений). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Синчронизедентрикаунтбитипе|Коллекция [стрингкэйлонгвалуепаир](synchronization-stringkeylongvaluepair.md)|Число синхронизированных объектов, перечисленных по типу объекта.|
|Траублешутингурл|String|В случае ошибки URL-адрес с действиями по устранению неполадок для проблемы.|

### <a name="synchronization-status-code-details"></a>Сведения о коде состояния синхронизации

| Значение                              | Описание    |
|:-----------------------------------|:---------------|
|NotConfigured                       |Задание не настроено и никогда не выполнялось. Авторизация не предоставлена. |
|Нотрун                              |Задание было настроено и, возможно, начато, но не завершило свое первое выполнение.|
|Активные                              |Задание выполняется периодически.|
|Приостановлено                              |Задание было приостановлено (обычно администратором), но в настоящее время оно не запущено, но состояние задания сохраняется.|
|Карантин                          |Задание находится в карантине. Это может произойти при большом объеме ошибок или критических ошибках, таких как отозванные или просроченные учетные данные. Во время карантина процесс синхронизации будет пытаться запустить задание с ограниченной частотой.|

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
  "suppressions": []
}
-->
