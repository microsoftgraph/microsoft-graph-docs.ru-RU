---
title: Тип ресурса schedulingGroup
description: Логическая группа участников расписания (как правило, по роли).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 9f4f494b21a1139ba9a9e0771dcbc41d363bab2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965301"
---
# <a name="schedulinggroup-resource-type"></a>Тип ресурса schedulingGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Логическая группа участников [расписания](schedule.md) (как правило, по роли). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание объекта schedulingGroup](../api/schedule-post-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) | Создание объекта `schedulingGroup`.|
|[Список объектов schedulingGroup](../api/schedule-list-schedulinggroups.md) | Коллекция [schedulingGroup](schedulinggroup.md) | Получение списка объектов `schedulingGroups` в расписании.|
|[Получение объекта schedulingGroup](../api/schedulinggroup-get.md) | [schedulingGroup](schedulinggroup.md) | Получение `schedulingGroup` по идентификатору.|
|[Замена объекта schedulingGroup](../api/schedulinggroup-put.md) | [schedulingGroup](schedulinggroup.md) | Замена объекта `schedulingGroup`.|
|[Удаление объекта schedulingGroup](../api/schedulinggroup-delete.md) | Нет | Объект `schedulingGroup` помечается как неактивный.|

## <a name="properties"></a>Свойства
|Имя          |Тип           |Описание                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            | `string`      |Идентификатор объекта `schedulingGroup`.|
| displayName   | `string`      | Отображаемое имя объекта `schedulingGroup`. Обязательный. |
| isActive          |`bool`      | Указывает, можно ли использовать объект `schedulingGroup` при создании новых сущностей или обновлении существующих. Обязательный. |
| userIds       | `collection(string)`    |  Список идентификаторов пользователей, являющихся участниками группы `schedulingGroup`. Обязательный. |
| createdDateTime       |`DateTimeOffset`        |Метка времени создания объекта `schedulingGroup`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedDateTime      |`DateTimeOffset`        |Метка времени последнего обновления объекта `schedulingGroup`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| lastModifiedBy        | [identitySet](identityset.md) |Учетная запись, которая последней обновила этот объект `schedulingGroup`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

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
