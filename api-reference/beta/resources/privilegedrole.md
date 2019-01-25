---
title: Тип ресурса privilegedRole
description: 'Представляет роль администратора Azure AD, например: **глобального администратора, администратора выставления счетов, администратор службы, администратор пользователя, пароль администратора**, и т.д.'
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513748"
---
# <a name="privilegedrole-resource-type"></a>Тип ресурса privilegedRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет роль администратора Azure AD, например: **глобального администратора, администратора выставления счетов, администратор службы, администратор пользователя, пароль администратора**, и т.д.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список объектов privilegedRole](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) коллекции|Получите коллекцию privilegedRole.|
|[Получение privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Чтение свойства и связи объекта privilegedRole.|
|[Список назначений](../api/privilegedrole-list-assignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md) коллекции| Получите коллекцию объектов назначения для этой роли.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Активация назначенной роли.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Деактивируйте, назначенной роли.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Уникальный идентификатор для роли администратора. Он является строкой GUID, совпадает со значением идентификатора шаблона роли из Azure AD для данной роли. Только для чтения.|
|name|строка|Имя роли.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|assignments|[privilegedRoleAssignment](privilegedroleassignment.md) коллекции| Назначения для этой роли. Только для чтения. Допускается значение null.|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| Параметры для этой роли. Только для чтения. Допускается значение null.|
|Summary|[privilegedRoleSummary](privilegedrolesummary.md)| Сводные данные для этой роли. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
