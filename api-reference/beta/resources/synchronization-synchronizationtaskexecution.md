---
title: Тип ресурса synchronizationTaskExecution
description: Сводка результатов запустите задание синхронизации.
ms.openlocfilehash: 4aefba4bdf9ab850892344e6e34683e81d1a1afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078579"
---
# <a name="synchronizationtaskexecution-resource-type"></a>Тип ресурса synchronizationTaskExecution

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сводка результатов запустите задание синхронизации.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|activityIdentifier           |String |Идентификатор запуска задания.|
|countEntitled                |Int64  |Число обработанных записей, которые были им назначены для этого приложения.|
|countEntitledForProvisioning |Int64  |Число обработанных записей, которые были им назначены для подготовки.|
|countEscrowed                |Int64  |Число записей, которые были депонированные (ошибки).|
|countEscrowedRaw             |Int64  |Число записей, которые были депонированные, включая сгенерированное системой escrows.|
|countExported                |Int64  |Число экспортированные операции.|
|countExports                 |Int64  |Число записей, которые были им также экспортировать.|
|countImported                |Int64  |Число импортированных записей.|
|countImportedDeltas          |Int64  |Число импортированных дельта изменения.|
|countImportedReferenceDeltas |Int64  |Число импортированных дельта изменения, относящиеся к изменений ссылок.|
|error                        |[synchronizationError](synchronization-synchronizationerror.md)|Если произошла ошибка, содержит объект **synchronizationError** с подробностями.|
|state                        |String |Подведение итогов в результате выполнения кода. Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timeBegan                    |DateTimeOffset|При выполнении этого задания времени начала. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|timeEnded                    |DateTimeOffset|При выполнении этого задания времени окончания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->