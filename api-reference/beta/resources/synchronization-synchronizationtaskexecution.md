---
title: Тип ресурса synchronizationTaskExecution
description: Суммирует результаты запуска задания синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ac42a91ec35c1d81d81efa52f4306bbd1cfb2f55
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135039"
---
# <a name="synchronizationtaskexecution-resource-type"></a>Тип ресурса synchronizationTaskExecution

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Суммирует результаты запуска задания синхронизации.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|activityIdentifier           |Строка |Идентификатор запуска задания.|
|countEntitled                |Int64  |Количество обработанных записей, которые были назначены для этого приложения.|
|countEntitledForProvisioning |Int64  |Количество обработанных записей, которые были назначены для предоставления.|
|countEscrowed                |Int64  |Количество записей, которые были escrowed (ошибки).|
|countEscrowedRaw             |Int64  |Количество записей, которые были escrowed, включая созданные системой escrows.|
|countExported                |Int64  |Количество экспортных записей.|
|countExports                 |Int64  |Количество записей, которые должны были быть экспортироваться.|
|countImported                |Int64  |Количество импортируемых записей.|
|countImportedDeltas          |Int64  |Количество импортируемых изменений.|
|countImportedReferenceDeltas |Int64  |Количество импортируемых изменений, связанных с изменениями ссылок.|
|error                        |[synchronizationError](synchronization-synchronizationerror.md)|Если произошла ошибка, содержит объект **synchronizationError** с подробными сведениями.|
|state                        |String |Код, суммарный результат этого запуска. Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timeBegan                    |DateTimeOffset|Время начала этого задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|timeEnded                    |DateTimeOffset|Время окончания этого задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>Представление в формате JSON

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


