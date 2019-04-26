---
title: Тип ресурса schedulingGroup
description: Логическая группа участников расписания (как правило, по роли).
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562956"
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
| lastModifiedBy        |`microsoft.graph.identitySet`        |Учетная запись, которая последней обновила этот объект `schedulingGroup`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
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
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
