---
title: тип ресурсов synchronizationStatus
description: Представляет текущее состояние синхронизацииJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 86320e6af31dae39f86ebe87f8490e24c7c33f57
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722057"
---
# <a name="synchronizationstatus-resource-type"></a>тип ресурсов synchronizationStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние [синхронизацииJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Свойства

| Свойство                              | Тип      | Описание    |
|:--------------------------------------|:----------|:---------------|
|code|String|Код состояния высокого уровня задания синхронизации. Возможные значения: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|Количество последовательных сбойных работ.|
|escrowsPruned|Boolean|`true` если эскроуы задания (ошибки на уровне объекта) были обрезки во время начальной синхронизации. Escrows можно обрезать, если во время начальной синхронизации вы достигнете порога ошибок, которые обычно помещали бы задание в карантин. Вместо того чтобы ходить в карантин, процесс синхронизации очищает ошибки задания и продолжается до завершения начальной синхронизации. После завершения начальной синхронизации задание приостанавливется и будет ждать, пока клиент очистит ошибки.|
|lastExecution|[синхронизацияTaskExecution](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении задания.|
|lastSuccessfulExecution|[синхронизацияTaskExecution](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении этого задания, в котором не было никаких ошибок.|
|lastSuccessfulExecutionWithExports|[синхронизацияTaskExecution](synchronization-synchronizationtaskexecution.md)|Сведения о последнем выполнении задания, которое экспортирует объекты в целевой каталог.|
|progress|[коллекция synchronizationProgress](synchronization-synchronizationprogress.md)|Сведения о ходе выполнения задания.|
|карантин|[синхронизацияКварантин](synchronization-quarantine.md)|Если задание находится в карантине, сведения о карантине.|
|steadyStateFirstAchievedTime|DateTimeOffset|Время, когда было достигнуто стабильное состояние (больше никаких изменений в процессе) было достигнуто. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|steadyStateLastAchievedTime|DateTimeOffset|Время, когда стабильное состояние (больше не изменяется в процессе) было достигнуто в последний раз. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|synchronizedEntryCountByType|[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection|Количество синхронизированных объектов, перечисленных по типу объекта.|
|устранение неполадокUrl|String|В случае ошибки URL-адрес с действиями по устранению неполадок для проблемы.|

### <a name="synchronization-status-code-details"></a>Сведения о коде состояния синхронизации

| Значение                              | Описание    |
|:-----------------------------------|:---------------|
|NotConfigured                       |Задание не было настроено и никогда не запускалось. Авторизация не была предоставлена. |
|NotRun                              |Задание было настроено и, возможно, запущено, но не завершило первый запуск.|
|Активное                              |Задание работает периодически.|
|Приостановка                              |Задание было приостановлено (обычно администратором) и в настоящее время не запущено, но состояние задания сохранено.|
|Карантин                          |Задание находится на карантине. Это может произойти, когда существует большой объем ошибок или критически важных ошибок, таких как аннулированные или просроченные учетные данные. В карантине процесс синхронизации будет пытаться выполнить задание с пониженной частотой.|

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


