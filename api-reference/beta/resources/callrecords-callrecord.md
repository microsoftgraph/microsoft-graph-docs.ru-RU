---
title: тип ресурса callRecord
description: Представляет один одноранговой вызов или групповой вызов между несколькими участниками, иногда именуемого как онлайн-собрание.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e0d9c93d696df969dd3cf78939d81a41385c8084
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58772228"
---
# <a name="callrecord-resource-type"></a>тип ресурса callRecord

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет один одноранговой вызов или групповой вызов между несколькими участниками, иногда именуемого как онлайн-собрание.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение callRecord](../api/callrecords-callrecord-get.md) | [microsoft.graph.callRecords.callRecord](callrecords-callrecord.md) | Ознакомьтесь с свойствами и отношениями объекта **callRecord.** |
| [getPstnCalls](../api/callrecords-callrecord-getpstncalls.md) | [коллекция microsoft.graph.callRecords.pstnCallLogRow](callrecords-pstncalllogrow.md) | Список **объектов pstnCallLogRow** в записи вызовов. |
| [getDirectRoutingCalls](../api/callrecords-callrecord-getdirectroutingcalls.md) | [коллекция microsoft.graph.callRecords.directRoutingLogRow](callrecords-directroutinglogrow.md)| Список **объектов directRoutingLogRow** для записи вызовов. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Время UTC, когда последний пользователь покинул вызов. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|Строка|Уникальный идентификатор для записи вызовов. Только для чтения.|
|joinWebUrl|String|Собрание URL-адреса, связанного с вызовом. Может быть недоступным для типа записи вызовов peerToPeer.|
|lastModifiedDateTime|DateTimeOffset|Время UTC при создания записи вызовов. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|модальности|Коллекция modality|Список всех способов, используемых в вызове. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|organizer|[identitySet](identityset.md)|Удостоверение организатора.|
|participants|Коллекция [identitySet](identityset.md)|Список различных удостоверений, участвующих в вызове.|
|startDateTime|DateTimeOffset|Время UTC, когда первый пользователь присоединился к вызову. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|type|callType|Указывает тип вызова. Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|version|Int64|Монотонно увеличивающаяся версия записи вызовов. Записи вызовов более высокой версии с тем же ИД включают дополнительные данные по сравнению с более низкой версией.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|сеансы|[коллекция microsoft.graph.callRecords.session](callrecords-session.md)|Список сеансов, участвующих в вызове. Одноранговые вызовы обычно имеют только один сеанс, в то время как групповые вызовы обычно имеют по крайней мере один сеанс на каждого участника. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.callRecord",
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


