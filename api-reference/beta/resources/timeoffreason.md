---
title: Тип ресурса Тимеоффреасон
description: Допустимая причина для выполнения времени ожидания в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582884"
---
# <a name="timeoffreason-resource-type"></a>Тип ресурса Тимеоффреасон

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Допустимая причина для экземпляра [тимеофф](timeoff.md) по расписанию. [](schedule.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание Тимеоффреасон](../api/schedule-post-timeoffreasons.md) | [Тимеоффреасон](timeoffreason.md) | Создание объекта `timeOffReason`.|
|[Список Тимеоффреасон](../api/schedule-list-timeoffreasons.md) | Коллекция [тимеоффреасон](timeoffreason.md) | Получение списка объектов `timeOffReasons` в расписании.|
|[Получение Тимеоффреасон](../api/timeoffreason-get.md) | [Тимеоффреасон](timeoffreason.md) | Получение `timeOffReason` по идентификатору.|
|[Замена Тимеоффреасон](../api/timeoffreason-put.md) | [Тимеоффреасон](timeoffreason.md) | Замена объекта `timeOffReason`.|
|[Удаление Тимеоффреасон](../api/timeoffreason-delete.md) | Нет | Объект `timeOffReason` помечается как неактивный.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `timeOffReason`.|
| displayName               | `string`                  | Имя файла `timeOffReason`. Обязательный. |
| Иконтипе | `enum`   | Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая. Обязательный. |
| isActive          |`bool`      | Указывает, можно ли использовать объект `timeOffReason` при создании новых сущностей или обновлении существующих. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Отметка `timeOffReason` времени первоначального создания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`         |Отметка `timeOffReason` времени последнего обновления. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedBy        |`microsoft.graph.identitySet`        |Учетная запись, которая последней обновила этот объект `timeOffReason`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason"
}-->

```json
{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffreason.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
