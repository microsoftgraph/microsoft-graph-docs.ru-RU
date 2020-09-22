---
title: Тип ресурса Тимеоффрекуест
description: Представляет тип запроса на сдвиг для получения тимеофф.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1b1e6c3f55b716590a399c9324ea759ff93810d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073392"
---
# <a name="timeoffrequest-resource-type"></a>Тип ресурса Тимеоффрекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на сдвиг для получения [тимеофф](../resources/timeoff.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/timeoffrequest-list.md) | Коллекция [тимеоффрекуест](timeoffrequest.md) | Получение списка объектов **тимеоффрекуест** в этом расписании.|
| [получение](../api/timeoffrequest-get.md); | [тимеоффрекуест](timeoffrequest.md) | Чтение свойств и связей объекта **тимеоффрекуест** . |
| [Удаление](../api/timeoffrequest-delete.md) | Нет | Удаление объекта **тимеоффрекуест** . |
| [Утвердить](../api/timeoffrequest-approve.md)|Нет|Утверждение запроса на нерабочее время.|
| [Отклоня](../api/timeoffrequest-decline.md)|Нет|Отклонить запрос времени ожидания.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|тимеоффреасонид|String|Причина невыходного времени.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest",
  "baseType": ""
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


