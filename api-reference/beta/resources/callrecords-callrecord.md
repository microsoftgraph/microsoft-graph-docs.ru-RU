---
title: Тип ресурса Каллрекорд
description: Представляет один одноранговый вызов или групповой вызов между несколькими участниками, которые иногда называют собранием по сети.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a119b95daf651ca5a91c269210a81a9a9a3cc1f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071585"
---
# <a name="callrecord-resource-type"></a>Тип ресурса Каллрекорд

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет один одноранговый вызов или групповой вызов между несколькими участниками, которые иногда называют собранием по сети.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение callRecord](../api/callrecords-callrecord-get.md) | [Microsoft. Graph. Каллрекордс. Каллрекорд](callrecords-callrecord.md) | Чтение свойств и связей объекта **каллрекорд** . |
| [Получение звонков PSTN](../api/callrecords-callrecord-getpstncalls.md) | [Microsoft. Graph. Каллрекордс. Пстнкалллогров](callrecords-pstncalllogrow.md)| Чтение свойств объекта **пстнкалллогров** . |
| [Получение прямых вызовов маршрутизации](../api/callrecords-callrecord-getdirectroutingcalls.md) | [Microsoft. Graph. Каллрекордс. Директраутинглогров](callrecords-directroutinglogrow.md)| Чтение свойств объекта **директраутинглогров** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Время в формате UTC, когда последний пользователь оставил вызов. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String|Уникальный идентификатор для записи вызова. Только для чтения.|
|жоинвебурл|String|URL-адрес собрания, связанный с вызовом. Может быть недоступен для типа записи вызовов Пиртопир.|
|lastModifiedDateTime|DateTimeOffset|Время в формате UTC при создании записи вызова. Тип DatetimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается как время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|модальности|коллекция Microsoft. Graph. Каллрекордс. Modal|Список всех модальности, используемых в вызове. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|organizer|[identitySet](identityset.md)|Удостоверение субъекта Организации.|
|participants|Коллекция [identitySet](identityset.md)|Список уникальных удостоверений, участвующих в вызове.|
|startDateTime|DateTimeOffset|Время в формате UTC, когда первый пользователь присоединился к вызову. Тип DatetimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается как время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|type|Microsoft. Graph. Каллрекордс. callType|Указывает тип вызова. Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|version|Int64|Монотонно увеличивающаяся версия записи вызова. Более высокие записи вызовов с одинаковым ИДЕНТИФИКАТОРом содержат дополнительные данные по сравнению с более низкой версией.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|сеансов|Коллекция [Microsoft. Graph. каллрекордс. Session](callrecords-session.md)|Список сеансов, участвующих в вызове. Одноранговые вызовы обычно имеют только один сеанс, в то время как для групповых вызовов обычно используется по крайней мере один сеанс на каждый участник. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "modalities": ["string"],
  "organizer": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}],
  "startDateTime": "String (timestamp)",
  "type": "string",
  "version": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


