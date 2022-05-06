---
title: Тип ресурса unifiedRoleDefinition
description: Унифицированное определение роли — это коллекция разрешений
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 93bc01ac19e0f976463821342524b060141e6182
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247233"
---
# <a name="unifiedroledefinition-resource-type"></a>Тип ресурса unifiedRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию разрешений с перечислением операций, таких как чтение, запись и удаление, которые могут выполняться поставщиком RBAC в Microsoft 365 управления [RBAC.](rolemanagement.md)

В настоящее время поддерживаются следующие поставщики RBAC:
- Облачный ПК 
- управление устройствами (Intune)
- каталог (Azure AD) 
- управление правами (Azure AD)


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [Коллекция unifiedRoleDefinition](unifiedroledefinition.md) | Чтение списка объектов unifiedRoleDefinition и их свойств. |
| [Получение unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Чтение свойств объекта unifiedRoleDefinition. |
| [Создание roleDefinitions](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Создайте объект unifiedRoleDefinition. |
| [Обновление unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Обновление объекта unifiedRoleDefinition. |
| [Удаление unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | Нет | Удаление объекта unifiedRoleDefinition. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String| Описание объекта unifiedRoleDefinition. Только для чтения, **если isBuiltIn** имеет значение true. |
|displayName|String| Отображаемое имя объекта unifiedRoleDefinition. Только для чтения, **если isBuiltIn** имеет значение true. Обязательно.  Поддерживает (`$filter``eq`и `startsWith` только операторы).|
|id|String| Уникальный идентификатор для unifiedRoleDefinition. Ключ, не допускающий значения NULL, только для чтения.  Поддерживает ( `$filter` только`eq` оператор). |
|isBuiltIn|Boolean| Флаг, указывающий, является ли unifiedRoleDefinition частью набора по умолчанию, включенного в продукт или пользовательский. Только для чтения.  Поддерживает ( `$filter` только`eq` оператор).|
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если задано значение false, роль недоступна для назначения. Только для чтения, **если isBuiltIn** имеет значение true. |
|resourceScopes|Коллекция String| К списку областей применяются разрешения, предоставленные определением роли. В настоящее время поддерживается `/` только. Только для чтения, если isBuiltIn имеет значение true. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это будет нерекомендуемым. Присоединение области к назначению ролей** | 
|rolePermissions|[Коллекция unifiedRolePermission](unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, **если isBuiltIn** имеет значение true. Обязательно. |
|templateId|String| Пользовательский идентификатор шаблона, который можно задать, если isBuiltIn имеет значение false. Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах. Только для чтения, **если isBuiltIn** имеет значение true. |
|version|String| Указывает версию unifiedRoleDefinition. Только для чтения, **если isBuiltIn** имеет значение true.|

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|inheritsPermissionsFrom| [Коллекция unifiedRoleDefinition](unifiedroledefinition.md)| Доступная только для чтения коллекция определений ролей, от которых наследуется заданное определение роли. Только Azure AD встроенные роли поддерживают этот атрибут. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": ["String"],
  "rolePermissions": [{"@odata.type": "microsoft.graph.unifiedRolePermission"}],
  "templateId": "String",
  "inheritsPermissionsFrom": [{"@odata.type": "microsoft.graph.unifiedRoleDefinition"}],
  "version": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


