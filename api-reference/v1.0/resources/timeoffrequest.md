---
title: Тип ресурса timeOffRequest
description: Представляет тип запроса на смену для отключаемого времени.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e234873110f50ed66decaa04b5462a9ff6fcf9a2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154203"
---
# <a name="timeoffrequest-resource-type"></a>Тип ресурса timeOffRequest

Пространство имен: microsoft.graph

Представляет тип запроса на смену для [отключаемого времени.](../resources/timeoff.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение](../api/timeoffrequest-get.md) | [timeOffRequest](timeoffrequest.md) | Чтение свойств и связей объекта **timeOffRequest.** |
| [Список](../api/timeoffrequest-list.md) | [Коллекция timeOffRequest](timeoffrequest.md) | Получите список объектов **timeOffRequest** в этом расписании.|
| [удаление](../api/timeoffrequest-delete.md); | Нет | Удаление объекта **timeOffRequest.** |
| [Утвердить](../api/timeoffrequest-approve.md)|Нет|Утверждение запроса на неавключие.|
| [Отклонение](../api/timeoffrequest-decline.md)|Нет|Отклонение запроса на отключение.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
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

