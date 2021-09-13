---
title: Тип ресурса shift
description: Представляет блок запланированных работ в расписании.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3b00e93f4622b91e7abe92a68007e870b5ab432e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032225"
---
# <a name="shift-resource-type"></a>Тип ресурса shift

Пространство имен: microsoft.graph

Представляет единицу запланированных работ в [расписании.](schedule.md) 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление смен](../api/schedule-list-shifts.md) | Коллекция [shift](shift.md) | Получите список **сдвигов в** этом расписании.|
|[Создание смены](../api/schedule-post-shifts.md) | [shift](shift.md) | Создайте новую **смену.**|
|[Получение смены](../api/shift-get.md) | [shift](shift.md) | Получите **смену** по ID.|
|[Замена смены](../api/shift-put.md) | [shift](shift.md) | Замените **смену**.|
|[Удаление смены](../api/shift-delete.md) | Нет | Удаление **переноса** из расписания.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |ID **смены**.|
| userId            |`string`      |ID пользователя, назначенного на **смену.** Обязательный элемент. |
| schedulingGroupId         |`string`      |ID группы планирования **является** частью смены. Обязательный элемент. |
| sharedShift   |[shiftItem](shiftitem.md)  |Общая версия этого **изменения,** которая просматривается как сотрудниками, так и руководителями. Обязательный элемент. |
| draftShift        |[shiftItem](shiftitem.md)        |Черновик версии этого **изменения,** который просматривается руководителями. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Время создания этой смены.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |Время последнего обновления  этого переноса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md)        |Удостоверение, которое в последний раз обновило этот **сдвиг.**|

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

