---
title: Тип ресурса Тимеоффреасон
description: Допустимая причина для выполнения времени ожидания в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8ba1e4bd596b82643ecbfa4b842e60232c182a4b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341976"
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
| Иконтипе | `timeOffReasonIconType`   | Поддерживаемые типы значков: нет; Мойка ведения запускается ходил Фирстаид; врача Нотворкинг; регистрации Журидути; любой кружк звонков Погода Общий Пиггибанк; Dog очень Траффикконе; крепления Веселая. Обязательный. |
| isActive          |`Boolean`      | Указывает, можно ли использовать объект `timeOffReason` при создании новых сущностей или обновлении существующих. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Отметка `timeOffReason` времени первоначального создания. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`         |Отметка `timeOffReason` времени последнего обновления. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedBy        | [identitySet](identityset.md)        |Учетная запись, которая последней обновила этот объект `timeOffReason`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
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
  "suppressions": []
}
-->
