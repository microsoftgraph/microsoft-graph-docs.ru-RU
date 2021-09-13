---
title: тип ресурсов сегмента
description: Тип сегмента
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8301508cebf11b6ff4970aa8b334f2d7912a6055
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113814"
---
# <a name="segment-resource-type"></a>тип ресурсов сегмента

Пространство имен: microsoft.graph.callRecords

Представляет часть User-User или User-Meeting связи в случае конференц-звонка. Типичный вызов VOIP будет иметь один сегмент в сеансе. В некоторых сценариях, таких как вызовы PSTN, в сеансе будет несколько сегментов из-за дополнительной связи между сервером и сервером, необходимой для подключения вызова.

## <a name="methods"></a>Методы

Нет методов непосредственного доступа к сегментам. Чтобы получить сегменты [для callRecord,](../api/callrecords-callrecord-get.md) используйте api Get `$expand=sessions($expand=segments)` [](../api/callrecords-session-list.md) `$expand=segments` [callRecord](callrecords-callrecord.md)с api или API сеанса List.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Уникальный идентификатор для сегмента. Только для чтения.|
|вызываемая|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Конечная точка, которая инициировала этот сегмент.|
|вызываемая|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Конечная точка, которая ответила на этот сегмент.|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|Сведения о сбое, связанные с сегментом в случае сбоя.|
|мультимедиа|[коллекция microsoft.graph.callRecords.media](callrecords-media.md)|Носители, связанные с этим сегментом.|
|startDateTime|DateTimeOffset|Время UTC, когда начался сегмент. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|endDateTime|DateTimeOffset|Время UTC после окончания сегмента. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="relationships"></a>Отношения

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
