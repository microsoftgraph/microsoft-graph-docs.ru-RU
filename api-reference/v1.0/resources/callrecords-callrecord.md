---
title: тип ресурса callRecord
description: Тип callRecord
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c6944d6a9cad10015f20a2b168645d71349cf829
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952531"
---
# <a name="callrecord-resource-type"></a>тип ресурса callRecord

Пространство имен: microsoft.graph.callRecords

Представляет один одноранговой вызов или групповой вызов между несколькими участниками, иногда именуемого как онлайн-собрание.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение callRecord](../api/callrecords-callrecord-get.md) | [microsoft.graph.callRecords.callRecord](callrecords-callrecord.md) | Чтение свойств и связей объекта callRecord. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Время UTC, когда последний пользователь покинул вызов. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String|Уникальный идентификатор для записи вызовов. Только для чтения.|
|joinWebUrl|String|Собрание URL-адреса, связанного с вызовом. Может быть недоступным для типа записи вызовов peerToPeer.|
|lastModifiedDateTime|DateTimeOffset|Время UTC при создания записи вызовов. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|модальности|коллекция modality|Список всех способов, используемых в вызове. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`, `screenSharing`, `unknownFutureValue`.|
|organizer|[identitySet](identityset.md)|Удостоверение организатора.|
|participants|Коллекция [identitySet](identityset.md)|Список различных удостоверений, участвующих в вызове.|
|startDateTime|DateTimeOffset|Время UTC, когда первый пользователь присоединился к вызову. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|type|callType|Указывает тип вызова. Возможные значения: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|version|Int64|Монотонно увеличивающаяся версия записи вызовов. Записи вызовов более высокой версии с тем же ид включают дополнительные данные по сравнению с более низкой версией.|

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
