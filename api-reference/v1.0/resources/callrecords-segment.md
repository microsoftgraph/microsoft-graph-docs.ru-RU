---
title: тип ресурса segment
description: Тип сегмента
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9240e0189bd9cc8a7961894562cdc9178ba07893
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153475"
---
# <a name="segment-resource-type"></a>тип ресурса segment

Пространство имен: microsoft.graph.callRecords

Представляет часть User-User или User-Meeting связи в случае конференц-вызова. Типичный вызов VOIP будет иметь один сегмент на сеанс. В некоторых сценариях, таких как вызовы STN, в сеансе будет несколько сегментов, так как для подключения вызова требуется дополнительная связь "сервер-сервер".

## <a name="methods"></a>Методы

Методы прямого доступа к сегментам не существуют. Используйте API [Get callRecord](../api/callrecords-callrecord-get.md) с API или API сеанса списка, чтобы получить сегменты `$expand=sessions($expand=segments)` для [](../api/callrecords-session-list.md) `$expand=segments` [callRecord](callrecords-callrecord.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Уникальный идентификатор сегмента. Только для чтения.|
|вызываемая|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Конечная точка, которая инициировала этот сегмент.|
|вызываемая|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Конечная точка, ответив на этот сегмент.|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|Сведения о сбое, связанные с сегментом в случае сбоя.|
|media|[Коллекция microsoft.graph.callRecords.media](callrecords-media.md)|Носители, связанные с этим сегментом.|
|startDateTime|DateTimeOffset|Время начала сегмента в UTC. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Время окончания сегмента в UTC. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "media": [{"@odata.type": "microsoft.graph.callRecords.media"}],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "segment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
