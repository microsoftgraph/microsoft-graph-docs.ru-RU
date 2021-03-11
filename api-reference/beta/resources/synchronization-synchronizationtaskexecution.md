---
title: тип ресурса синхронизацииTaskExecution
description: Суммирует результаты работы синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d83092949e1f27c9dac9744d2b4b16be4bcbae0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722050"
---
# <a name="synchronizationtaskexecution-resource-type"></a>тип ресурса синхронизацииTaskExecution

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Суммирует результаты работы синхронизации.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|activityIdentifier           |String |Идентификатор запуска задания.|
|countEntitled                |Int64  |Количество обработанных записей, которые были назначены для этого приложения.|
|countEntitledForProvisioning |Int64  |Количество обработанных записей, которые были назначены для предварительной обработки.|
|countEscrowed                |Int64  |Количество записей, которые были escrowed (ошибки).|
|countEscrowedRaw             |Int64  |Количество записей, которые были депонированы, включая системные эскроу-|
|countExported                |Int64  |Количество экспортных записей.|
|countExports                 |Int64  |Количество записей, которые должны были экспортироваться.|
|countImported                |Int64  |Количество импортных записей.|
|countImportedDeltas          |Int64  |Количество импортируемых изменений дельты.|
|countImportedReferenceDeltas |Int64  |Количество импортируемых изменений дельты, относящихся к эталонным изменениям.|
|error                        |[синхронизацияError](synchronization-synchronizationerror.md)|В случае ошибки содержится объект **синхронизацииError** с подробными сведениями.|
|state                        |String |Код, подводя итоги этого запуска. Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timeBegan                    |DateTimeOffset|Время начала этого запуска задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|timeEnded                    |DateTimeOffset|Время окончания этого задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


