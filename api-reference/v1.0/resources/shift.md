---
title: Тип ресурса shift
description: Представляет единицу измерения трудозатрат по расписанию.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e38b8a000829ead91bdee28779a0f6988dd936ef
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154306"
---
# <a name="shift-resource-type"></a>Тип ресурса shift

Пространство имен: microsoft.graph

Представляет единицу измерения запланированной работы по [расписанию](schedule.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление смен](../api/schedule-list-shifts.md) | Коллекция [shift](shift.md) | Получение списка **смен** в этом расписании.|
|[Создание смены](../api/schedule-post-shifts.md) | [shift](shift.md) | Создайте новую **смену**.|
|[Получение смены](../api/shift-get.md) | [shift](shift.md) | Получение **сдвига** по идентификатору.|
|[Замена смены](../api/shift-put.md) | [shift](shift.md) | Замените **смену**.|
|[Удаление смены](../api/shift-delete.md) | Нет | Удалить **смену** из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |Идентификатор **смены**.|
| userId            |`string`      |Идентификатор пользователя, назначенный **смене**. Обязательный. |
| schedulingGroupId         |`string`      |Идентификатор группы планирования, частью которой является **Смена** . Обязательный. |
| sharedShift   |[shiftItem](shiftitem.md)  |Общая версия этой **смены** , отображаемая как для сотрудников, так и для руководителей. Обязательный. |
| draftShift        |[shiftItem](shiftitem.md)        |Черновая версия этой **смены** , которая отображается руководителями. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Временная метка, на которую было впервые создана эта **Смена** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`        |Временная метка, на которую было Последнее обновление этой **смены** . Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedBy        | [identitySet](identityset.md)        |Идентификатор, который последним обновил этот **сдвиг**.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
