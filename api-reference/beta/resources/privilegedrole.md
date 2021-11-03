---
title: тип ресурса privilegedRole
description: Представляет роль администратора Azure AD, например глобального администратора, администратора биллинга, администратора службы, администратора пользователей и администратора паролей.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 756ffd580a2f44fad1631bbfd153d1320f1aef05
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687678"
---
# <a name="privilegedrole-resource-type-deprecated"></a>тип ресурса privilegedRole (неподготовленный)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Представляет встроенную роль администратора [Azure AD,](/azure/active-directory/roles/permissions-reference)например глобального администратора, администратора биллинга, администратора **службы,** администратора пользователей и **администратора паролей.**


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список объектов privilegedRole](../api/privilegedrole-list.md) | Коллекция [privilegedRole](privilegedrole.md)|Получите коллекцию privilegedRole.|
|[Получение privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Чтение свойств и связей объекта privilegedRole.|
|[Перечисление заданий](../api/privilegedrole-list-assignments.md) |Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)| Получите коллекцию объектов назначения для этой роли.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Активируйте назначенную роль.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Деактивировать назначенную роль.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Уникальный идентификатор роли администратора. Это строка GUID и имеет то же значение, что и id шаблона ролей из Azure AD для данной роли. Только для чтения.|
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


