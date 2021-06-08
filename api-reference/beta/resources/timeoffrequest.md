---
title: тип ресурса timeOffRequest
description: Представляет тип запроса на смену, чтобы занять время.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31d855f21164f933fe27acc824759cee08e16c16
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786070"
---
# <a name="timeoffrequest-resource-type"></a>тип ресурса timeOffRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на перенос, чтобы занять [timeOff](../resources/timeoff.md).

## <a name="methods"></a>Методы

| Метод       | Тип возвращаемых данных | Описание |
|:-------------|:------------|:------------|
| [Список](../api/timeoffrequest-list.md) | [коллекция timeOffRequest](timeoffrequest.md) | Получите список объектов **timeOffRequest** в этом расписании.|
| [получение](../api/timeoffrequest-get.md); | [timeOffRequest](timeoffrequest.md) | Ознакомьтесь с свойствами и отношениями объекта **timeOffRequest.** |
| [Delete](../api/timeoffrequest-delete.md) | Нет | Удаление **объекта timeOffRequest.** |
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


