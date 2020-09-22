---
title: Тип ресурса Синчронизатионтаскексекутион
description: Сводка результатов выполнения задания синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d777a575290699c2a936902614aa8ef0e8b042d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094920"
---
# <a name="synchronizationtaskexecution-resource-type"></a>Тип ресурса Синчронизатионтаскексекутион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сводка результатов выполнения задания синхронизации.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|активитидентифиер           |Строка |Идентификатор запуска задания.|
|каунтентитлед                |Int64  |Количество обработанных элементов, которые были назначены для этого приложения.|
|каунтентитледфорпровисионинг |Int64  |Количество обработанных записей, которые были назначены для подготовки.|
|каунтескровед                |Int64  |Количество условных (ошибочных) записей.|
|каунтескроведрав             |Int64  |Количество условных записей, включая созданные системой.|
|каунтекспортед                |Int64  |Количество экспортированных записей.|
|каунтекспортс                 |Int64  |Количество записей, которые ожидались экспортировать.|
|каунтимпортед                |Int64  |Количество импортированных записей.|
|каунтимпортедделтас          |Int64  |Количество импортированных изменений изменений.|
|каунтимпортедреференцеделтас |Int64  |Количество импортированных изменений изменений, относящихся к изменениям ссылок.|
|error                        |[синчронизатионеррор](synchronization-synchronizationerror.md)|Если обнаружена ошибка, содержит объект **синчронизатионеррор** со сведениями.|
|state                        |String |Код, суммирующий результат этого запуска. Возможные значения: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|тимебеган                    |DateTimeOffset|Время начала выполнения задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|тиминдед                    |DateTimeOffset|Время окончания выполнения задания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

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


