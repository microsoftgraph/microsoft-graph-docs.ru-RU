---
title: Тип ресурса privilegedRole
description: Представляет роль Azure AD администратора, например глобального администратора, администратора выставления счетов, администратора служб, администратора пользователей и администратора паролей.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 8c96fc5c7de9eb907639f7d01795b85750eeaf0a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399315"
---
# <a name="privilegedrole-resource-type-deprecated"></a>Тип ресурса privilegedRole (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Представляет встроенную [Azure AD](/azure/active-directory/roles/permissions-reference) администратора, например глобального администратора **,** администратора выставления счетов, администратора служб, администратора пользователей и **администратора паролей**.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов privilegedRole](../api/privilegedrole-list.md) | Коллекция [privilegedRole](privilegedrole.md)|Получение коллекции privilegedRole.|
|[Получение privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Чтение свойств и связей объекта privilegedRole.|
|[Перечисление заданий](../api/privilegedrole-list-assignments.md) |Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)| Получение коллекции объектов назначения для этой роли.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Активируйте назначенную роль.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Деактивация назначенной роли.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Уникальный идентификатор роли администратора. Это строка GUID, которая имеет то же значение, что и идентификатор шаблона роли из Azure AD для данной роли. Только для чтения.|
|name|string|Имя роли.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|assignments|Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)| Назначения для этой роли. Только для чтения. Допускается значение null.|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| Параметры для этой роли. Только для чтения. Допускается значение null.|
|summary|[privilegedRoleSummary](privilegedrolesummary.md)| Сводная информация для этой роли. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->


