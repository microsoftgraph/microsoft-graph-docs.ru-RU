---
title: тип ресурса timeOffRequest
description: Представляет тип запроса на перенос, чтобы занять время.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b7bde8033680b6da30def7182e93e5672504475d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019099"
---
# <a name="timeoffrequest-resource-type"></a>тип ресурса timeOffRequest

Пространство имен: microsoft.graph

Представляет тип запроса на перенос, чтобы занять [timeOff](../resources/timeoff.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/timeoffrequest-get.md); | [timeOffRequest](timeoffrequest.md) | Ознакомьтесь с свойствами и отношениями объекта **timeOffRequest.** |
| [Перечисление](../api/timeoffrequest-list.md) | [коллекция timeOffRequest](timeoffrequest.md) | Получите список объектов **timeOffRequest** в этом расписании.|
| [удаление](../api/timeoffrequest-delete.md); | Нет | Удаление **объекта timeOffRequest.** |
| [Утвердить](../api/timeoffrequest-approve.md)|Нет|Утверждение запроса на время.|
| [Отклонение](../api/timeoffrequest-decline.md)|Нет|Отклонение запроса на время.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
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

