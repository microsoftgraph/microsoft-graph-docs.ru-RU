---
title: Тип ресурса Shift
description: Смена — это единица запланированной работы в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d3a91cd7b4f2b4d8e32219514d1190599ac416de
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049633"
---
# <a name="shift-resource-type"></a>Тип ресурса Shift

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Единица запланированной работы по [расписанию](schedule.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание смены](../api/schedule-post-shifts.md) | [перемещен](shift.md) | Создание объекта `shift`.|
|[Перечисление смещений](../api/schedule-list-shifts.md) | Коллекция " [SHIFT](shift.md) " | Получение списка `shifts` по данному расписанию.|
|[Получение Shift](../api/shift-get.md) | [перемещен](shift.md) | Получение `shift` по идентификатору.|
|[Замена Shift](../api/shift-put.md) | [перемещен](shift.md) | Замена объекта `shift`.|
|[Удаление смены](../api/shift-delete.md) | Нет | Удаление `shift` из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор объекта `shift`.|
| userId            |`string`      |Идентификатор пользователя, `shift`назначенный. Обязательно. |
| Счедулингграупид         |`string`      |Идентификатор группы планирования, в которой `shift` входит. Обязательно. |
| Шаредшифт   |[Шифтитем](shiftitem.md)  |Общая версия этого `shift` объекта доступна как для сотрудников, так и для руководителей. Обязательно. |
| Драфтшифт        |[Шифтитем](shiftitem.md)        |Черновая версия этого `shift` элемента, просматриваемая руководителями. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Временная метка, на которую `shift` был создан впервые. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`        |Отметка времени `shift` последнего обновления. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedBy        | [identitySet](identityset.md)        |Учетная запись, которая последней обновила этот объект `shift`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
