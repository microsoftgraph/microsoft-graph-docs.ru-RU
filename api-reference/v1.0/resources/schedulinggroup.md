---
title: Тип ресурса schedulingGroup
description: Логическая группа участников расписания (как правило, по роли).
author: akumar39
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 8bb7a1d0750c6712fada9d3180280180299d85b4cd3bf0539be8b14880222f18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182373"
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
| displayName   | `string`      | Отображаемое имя для объекта **schedulingGroup**. Обязательное. |
| isActive          |`bool`      | Указывает, можно ли использовать объект `schedulingGroup` при создании новых сущностей или обновлении существующих. Обязательное. |
| userIds       | `collection(string)`    |  Список ИД пользователей, являющихся участниками **schedulingGroup**. Обязательное. |
| createdDateTime       |`DateTimeOffset`        |Время создания группы **schedulingGroup**. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |Время последнего обновления группы **schedulingGroup**. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. |
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

