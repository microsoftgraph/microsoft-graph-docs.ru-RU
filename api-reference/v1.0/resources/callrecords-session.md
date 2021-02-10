---
title: Тип ресурса session
description: Тип сеанса
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9a61fca17c8b04e9f5c236d0104b2b93f1a6704e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153497"
---
# <a name="session-resource-type"></a>Тип ресурса session

Пространство имен: microsoft.graph.callRecords

Представляет User-User или User-Meeting в случае конференц-связи.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление сеансов](../api/callrecords-session-list.md) | [коллекция microsoft.graph.callRecords.session](callrecords-session.md) | Получить список сеансов, связанных с [объектом callRecord.](callrecords-callrecord.md)
 |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|string|Уникальный идентификатор сеанса. Только для чтения.|
|вызываемая|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Конечная точка, которая инициировала сеанс.|
|вызываемая|[microsoft.graph.callRecords.endpoint](callrecords-endpoint.md)|Конечная точка, ответив на сеанс.|
|failureInfo|[microsoft.graph.callRecords.failureInfo](callrecords-failureinfo.md)|Сведения о сбое, связанном с сеансом, если сеанс не был сбой.|
|модальности|Коллекция microsoft.graph.callRecords.modality|Список модальных режимов, присутствующих в сеансе. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|Время в UTC, когда первый пользователь присоединился к сеансу. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Время в UTC, когда последний пользователь покинул сеанс. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|segments|[Коллекция microsoft.graph.callRecords.segment](callrecords-segment.md)|Список сегментов, участвующих в сеансе. Только для чтения. Допускается значение null.|

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
