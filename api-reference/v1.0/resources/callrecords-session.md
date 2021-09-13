---
title: Тип ресурса сеанса
description: Тип сеанса
ms.localizationpriority: medium
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c8afac51a3e1709c5aafd4314045c36d8b34184b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113786"
---
# <a name="session-resource-type"></a>Тип ресурса сеанса

Пространство имен: microsoft.graph.callRecords

Представляет собой User-User или User-Meeting связи в случае конференц-звонка.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление сеансов](../api/callrecords-session-list.md) | [коллекция microsoft.graph.callRecords.session](callrecords-session.md) | Извлечение списка сеансов, связанных с [объектом callRecord.](callrecords-callrecord.md)
 |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|string|Уникальный идентификатор для сеанса. Только для чтения.|
|вызываемая|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Конечная точка, которая инициировала сеанс.|
|вызываемая|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Конечная точка, которая ответила на сеанс.|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|Сведения о сбоях, связанных с сеансом, в случае сбоя сеанса.|
|модальности|коллекция microsoft.graph.callRecords.modality|Список способов, присутствующих на сеансе. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|Время UTC, когда первый пользователь присоединился к сеансу. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|endDateTime|DateTimeOffset|Время UTC, когда последний пользователь покинул сеанс. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|


## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|segments|[коллекция microsoft.graph.callRecords.segment](callrecords-segment.md)|Список сегментов, участвующих в сеансе. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.session",
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
