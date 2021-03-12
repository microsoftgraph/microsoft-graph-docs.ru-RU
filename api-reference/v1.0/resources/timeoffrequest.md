---
title: тип ресурса timeOffRequest
description: Представляет тип запроса на перенос, чтобы занять время.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 76eea937b03f3eb117e6b5f870a316f268df615c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721699"
---
# <a name="timeoffrequest-resource-type"></a>тип ресурса timeOffRequest

Пространство имен: microsoft.graph

Представляет тип запроса на перенос, чтобы занять [timeOff](../resources/timeoff.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/timeoffrequest-get.md); | [timeOffRequest](timeoffrequest.md) | Ознакомьтесь с свойствами и отношениями объекта **timeOffRequest.** |
| [List](../api/timeoffrequest-list.md) | [коллекция timeOffRequest](timeoffrequest.md) | Получите список объектов **timeOffRequest** в этом расписании.|
| [удаление](../api/timeoffrequest-delete.md); | Нет | Удаление **объекта timeOffRequest.** |
| [Утвердить](../api/timeoffrequest-approve.md)|Нет|Утверждение запроса на время.|
| [Отклонение](../api/timeoffrequest-decline.md)|Нет|Отклонение запроса на время.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|timeOffReasonId|String|Причина простоя.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest"
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

