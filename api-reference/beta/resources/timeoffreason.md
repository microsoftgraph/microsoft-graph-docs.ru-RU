---
title: тип ресурса timeOffReason
description: Веские причины для того, чтобы взять время в расписании.
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b35daada189490caaf2d37f24c777f1a24c3c885
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720881"
---
# <a name="timeoffreason-resource-type"></a>тип ресурса timeOffReason

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Веские основания для [экземпляра timeOff](timeoff.md) в [расписании](schedule.md).

## <a name="methods"></a>Методы

| Метод                                           | Тип возвращаемых данных                                  | Описание                                      |
| :----------------------------------------------- | :------------------------------------------- | :----------------------------------------------- |
| [Создание](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md)            | Создание нового **timeOffReason**.                  |
| [Перечисление](../api/schedule-list-timeoffreasons.md)   | [коллекция timeOffReason](timeoffreason.md) | Получите список **timeOffReason в** расписании. |
| [Получение](../api/timeoffreason-get.md)               | [timeOffReason](timeoffreason.md)            | Получите **timeOffReason по** ID.                   |
| [Replace](../api/timeoffreason-put.md)           | [timeOffReason](timeoffreason.md)            | Замените **timeOffReason**.                     |
| [Delete](../api/timeoffreason-delete.md)         | Нет                                         | **Пометить timeOffReason** как неактивное.            |

## <a name="properties"></a>Свойства

| Свойство             | Тип                          | Описание                                                                                                                                                                                                                                    |
| -------------------- | ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | `string`                      | ID **timeOffReason**.                                                                                                                                                                                                                   |
| displayName          | `string`                      | Имя **timeOffReason**. Обязательный.                                                                                                                                                                                                   |
| iconType             | `timeOffReasonIconType`       | Поддерживаемые типы значков: нет; автомобиль; календарь; запуск; плоскости; firstAid; врач; notWorking; часы; juryDuty; глобус; чашка; телефон; погода; зонт; piggyBank; собака; торт; trafficCone; пин-код; солнечный. Обязательный.                                       |
| isActive             | `Boolean`                     | Указывает, можно ли **использовать timeOffReason** при создании новых сущностям или обновлении существующих. Обязательный.                                                                                                                            |
| createdDateTime      | `DateTimeOffset`              | Штамп времени, на котором на **этот раз был созданOffReason** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime | `DateTimeOffset`              | Штамп времени, на котором **в этот раз был обновленOffReason** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.  |
| lastModifiedBy       | [identitySet](identityset.md) | Удостоверение, которое в последний раз обновлялось **на этот разOffReason**.                                                                                                                                                                                         |

## <a name="json-representation"></a>Представление JSON

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
