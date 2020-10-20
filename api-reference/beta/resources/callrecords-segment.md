---
title: Тип ресурса "сегмент"
description: Тип сегмента
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 84f18568d1890b331d1bedd6d9e7114518fad3cf
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601666"
---
# <a name="segment-resource-type"></a>Тип ресурса "сегмент"

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет часть User-User взаимодействия или User-Meeting связи в случае вызова конференции. Типичный вызов VOIP будет иметь по одному сегменту на сеанс. В определенных сценариях, таких как звонки по протоколу PSTN, для каждого сеанса будет использоваться несколько сегментов из-за дополнительного обмена данными между серверами, необходимыми для подключения вызова.

## <a name="methods"></a>Методы

Не существует методов для прямого доступа к сегментам. Для получения сегментов для Каллрекорд используйте API [Get каллрекорд](../api/callrecords-callrecord-get.md) с `$expand=sessions($expand=segments)` API [сеанса или списка](../api/callrecords-session-list.md) `$expand=segments` . [callRecord](callrecords-callrecord.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Уникальный идентификатор сегмента. Только для чтения.|
|объекта|[Microsoft. Graph. Каллрекордс. Endpoint](callrecords-endpoint.md)|Конечная точка, которая инициировала этот сегмент.|
|вызываемого абонента|[Microsoft. Graph. Каллрекордс. Endpoint](callrecords-endpoint.md)|Конечная точка, которая ответила на этот сегмент.|
|failureInfo|[Microsoft. Graph. Каллрекордс. Фаилуреинфо](callrecords-failureinfo.md)|Сведения об ошибке, связанные с сегментом, если произошел сбой.|
|media|Коллекция [Microsoft. Graph. каллрекордс. Media](callrecords-media.md)|Носитель, связанный с этим сегментом.|
|startDateTime|DateTimeOffset|Время в формате UTC, когда начался сегмент. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Время в формате UTC, когда сегмент закончился. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.segment",
  "baseType": "",
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

