---
title: Тип ресурса schedulingGroup
description: Логическая группа участников расписания (как правило, по роли).
author: akumar39
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 018359ab0dd6702a2fda40bf5f0b29c639211f4a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719306"
---
# <a name="schedulinggroup-resource-type"></a>Тип ресурса schedulingGroup

Пространство имен: microsoft.graph

Логическая группа участников [расписания](schedule.md) (как правило, по роли). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/schedule-list-schedulinggroups.md) | Коллекция объектов [schedulingGroup](schedulinggroup.md) | Вы можете просмотреть список объектов **schedulingGroups** в расписании.|
|[Создание](../api/schedule-post-schedulinggroups.md); | [schedulingGroup](schedulinggroup.md) | Создание нового объекта **schedulingGroup**|
|[Получение](../api/schedulinggroup-get.md); | [schedulingGroup](schedulinggroup.md) | Получение объекта **schedulingGroup** по ИД|
|[удаление](../api/schedulinggroup-delete.md); | Нет | Обозначение объекта **schedulingGroup** как неактивного.|
|[Замена](../api/schedulinggroup-put.md) | [schedulingGroup](schedulinggroup.md) | Замена объекта **schedulingGroup**.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            | `string`      |ИД объекта **schedulingGroup**|
| displayName   | `string`      | Отображаемое имя для объекта **schedulingGroup**. Обязательный. |
| isActive          |`bool`      | Указывает, можно ли использовать объект `schedulingGroup` при создании новых сущностей или обновлении существующих. Обязательный. |
| userIds       | `collection(string)`    |  Список ИД пользователей, являющихся участниками **schedulingGroup**. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Метка времени первоначального создания объекта **schedulingGroup**. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |Метка времени последнего обновления объекта **schedulingGroup**. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md) |Учетная запись, которая последней обновила этот объект **schedulingGroup**.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "isActive": true,
  "userIds": ["String (identifier)"],
  "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

