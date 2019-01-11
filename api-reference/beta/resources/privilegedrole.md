---
title: Тип ресурса privilegedRole
description: 'Представляет роль администратора Azure AD, например: **глобального администратора, администратора выставления счетов, администратор службы, администратор пользователя, пароль администратора**, и т.д.'
localization_priority: Normal
ms.openlocfilehash: 75763e18731cb969623cc4df6360d50abc018b41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860860"
---
# <a name="privilegedrole-resource-type"></a>Тип ресурса privilegedRole

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
|id|строка|Уникальный идентификатор для роли администратора. Он является строкой GUID, совпадает со значением идентификатора шаблона роли из Azure AD для данной роли. Только для чтения.|
|name|строка|Имя роли.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|assignments|[privilegedRoleAssignment](privilegedroleassignment.md) коллекции| Назначения для этой роли. Только для чтения. Допускается значение null.|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| Параметры для этой роли. Только для чтения. Допускается значение null.|
|Сводка|[privilegedRoleSummary](privilegedrolesummary.md)| Сводные данные для этой роли. Только для чтения. Допускается значение null.|

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
