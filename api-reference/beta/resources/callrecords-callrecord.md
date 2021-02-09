---
title: Тип ресурса callRecord
description: Представляет один одноранговой звонок или групповой звонок между несколькими участниками, которые иногда называют собранием по сети.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 04335e2d804a0d1f824cfc70982e3c138812f8ce
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159684"
---
# <a name="callrecord-resource-type"></a>Тип ресурса callRecord

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет один одноранговой звонок или групповой звонок между несколькими участниками, которые иногда называют собранием по сети.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение callRecord](../api/callrecords-callrecord-get.md) | [microsoft.graph.callRecords.callRecord](callrecords-callrecord.md) | Чтение свойств и связей объекта **callRecord.** |
| [Получить вызовы STN](../api/callrecords-callrecord-getpstncalls.md) | [microsoft.graph.callRecords.pstnCallLogRow](callrecords-pstncalllogrow.md)| Чтение свойств объекта **pstnCallLogRow.** |
| [Get direct routing calls](../api/callrecords-callrecord-getdirectroutingcalls.md) | [microsoft.graph.callRecords.directRoutingLogRow](callrecords-directroutinglogrow.md)| Чтение свойств объекта **directRoutingLogRow.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Время в UTC, когда последний пользователь оставил вызов. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String|Уникальный идентификатор записи вызова. Только для чтения.|
|joinWebUrl|String|URL-адрес собрания, связанный с вызовом. Может быть не доступен для типа записи вызова peerToPeer.|
|lastModifiedDateTime|DateTimeOffset|Время создания записи вызова в UTC. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|модальности|Коллекция microsoft.graph.callRecords.modality|Список всех модальных режимов, используемых в вызове. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|organizer|[identitySet](identityset.md)|Удостоверение организатора.|
|participants|Коллекция [identitySet](identityset.md)|Список отдельных удостоверений, участвующих в вызове.|
|startDateTime|DateTimeOffset|Время в UTC, когда первый пользователь присоединился к вызову. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|type|microsoft.graph.callRecords.callType|Указывает тип вызова. Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|version|Int64|Монотонно увеличивающаяся версия записи вызова. Записи вызовов более высокой версии с тем же ИД включают дополнительные данные по сравнению с более низкой версией.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|sessions|[Коллекция microsoft.graph.callRecords.session](callrecords-session.md)|Список сеансов, участвующих в вызове. Одноранговые звонки обычно имеют только один сеанс, тогда как групповые вызовы обычно имеют по крайней мере один сеанс на участника. Только для чтения. Допускается значение null.|

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


