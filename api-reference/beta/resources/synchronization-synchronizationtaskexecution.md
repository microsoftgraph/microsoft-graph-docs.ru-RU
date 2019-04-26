---
title: Тип ресурса Синчронизатионтаскексекутион
description: Сводка результатов выполнения задания синхронизации.
localization_priority: Normal
ms.openlocfilehash: a9008dd7d51a1d07be75c5b9bbad34d636fff74c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339828"
---
# <a name="synchronizationtaskexecution-resource-type"></a>Тип ресурса Синчронизатионтаскексекутион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сводка результатов выполнения задания синхронизации.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Активитидентифиер           |String |Идентификатор запуска задания.|
|Каунтентитлед                |Int64  |Количество обработанных элементов, которые были назначены для этого приложения.|
|Каунтентитледфорпровисионинг |Int64  |Количество обработанных записей, которые были назначены для подготовки.|
|Каунтескровед                |Int64  |Количество условных (ошибочных) записей.|
|Каунтескроведрав             |Int64  |Количество условных записей, включая созданные системой.|
|Каунтекспортед                |Int64  |Количество экспортированных записей.|
|Каунтекспортс                 |Int64  |Количество записей, которые ожидались экспортировать.|
|Каунтимпортед                |Int64  |Количество импортированных записей.|
|Каунтимпортедделтас          |Int64  |Количество импортированных изменений изменений.|
|Каунтимпортедреференцеделтас |Int64  |Количество импортированных изменений изменений, относящихся к изменениям ссылок.|
|error                        |[Синчронизатионеррор](synchronization-synchronizationerror.md)|Если обнаружена ошибка, содержит объект **синчронизатионеррор** со сведениями.|
|state                        |String |Код, суммирующий результат этого запуска. Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|Тимебеган                    |DateTimeOffset|Время начала выполнения задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Тиминдед                    |DateTimeOffset|Время окончания выполнения задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

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
