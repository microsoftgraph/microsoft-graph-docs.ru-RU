---
title: Тип ресурса Session
description: Тип сеанса
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8c1af52332c5650123d604b8e405bf88d0c2f965
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353128"
---
# <a name="session-resource-type"></a>Тип ресурса Session

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательское взаимодействие с пользователем или собрание пользователя в случае вызова конференции.

## <a name="methods"></a>Methods

Не существует методов для прямого доступа к сеансам. Используйте API [Get каллрекорд](../api/callrecords-callrecord-get.md) , `$expand=sessions` чтобы получить сеансы для [каллрекорд](callrecords-callrecord.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|string|Уникальный идентификатор сеанса. Только для чтения.|
|объекта|[Microsoft. Graph. Каллрекордс. Endpoint](callrecords-endpoint.md)|Конечная точка, которая инициировала сеанс.|
|вызываемого абонента|[Microsoft. Graph. Каллрекордс. Endpoint](callrecords-endpoint.md)|Конечная точка, которая ответила на сеанс.|
|failureInfo|[Microsoft. Graph. Каллрекордс. Фаилуреинфо](callrecords-failureinfo.md)|Сведения о сбое, связанные с сеансом в случае сбоя сеанса.|
|модальности|коллекция Microsoft. Graph. Каллрекордс. Modal|Список модальности, присутствующих в сеансе. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|UTC Фиме, когда первый пользователь присоединился к сеансу. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Время в формате UTC, когда последний пользователь оставил сеанс. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|


## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|segments|Коллекция [Microsoft. Graph. каллрекордс. segment](callrecords-segment.md)|Список сегментов, участвующих в сеансе. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "caller": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "callee": {"@odata.type": "microsoft.graph.callRecords.endpoint"},
  "failureInfo": {"@odata.type": "microsoft.graph.callRecords.failureInfo"},
  "modalities": ["string"],
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "session resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->