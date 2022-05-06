---
title: Тип ресурса unifiedRoleDefinition
description: Определение роли — это коллекция разрешений в Azure Active Directory (Azure AD).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f3a54d12ce4c11ee10d106759ccbaa0e32b80978
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246596"
---
# <a name="unifiedroledefinition-resource-type"></a>Тип ресурса unifiedRoleDefinition

Пространство имен: microsoft.graph

Определение роли — это коллекция разрешений в Azure Active Directory (Azure AD) с описанием операций, которые можно выполнить, и ресурсов, с которыми они могут выполняться.

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
|description|String| Описание объекта unifiedRoleDefinition. Только для чтения, **если isBuiltIn** имеет значение `true`. |
|displayName|String| Отображаемое имя объекта unifiedRoleDefinition. Только для чтения, **если isBuiltIn** имеет значение `true`. Обязательно.  Поддерживает $filter (`eq`, `in`).|
|id|String| Уникальный идентификатор определения роли. Ключ, не допускающий значения NULL, только для чтения. Наследуется от [сущности](../resources/entity.md). Поддерживает $filter (`eq`, `in`). |
|isBuiltIn|Boolean| Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в Azure Active Directory (Azure AD) или пользовательское определение. Только для чтения. Поддерживает $filter (`eq`, `in`). |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если `false` роль недоступна для назначения. Только для чтения, **если isBuiltIn** имеет значение true. |
|resourceScopes|Коллекция String| Список областей или разрешений, к которым применяется определение роли. В настоящее время поддерживается `/` только. Только для чтения, **если isBuiltIn** имеет значение true. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это будет нерекомендуемым. Присоединение области к назначению ролей.** | 
|rolePermissions|[Коллекция unifiedRolePermission](unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, **если isBuiltIn** имеет значение `true`. Обязательно. |
|templateId|String| Пользовательский идентификатор шаблона, который можно задать, если **isBuiltIn** имеет `false` значение, но доступен только для чтения, если **isBuiltIn** имеет значение `true`. Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах. |
|version|String| Указывает версию определения роли. Только для чтения, **если isBuiltIn** имеет значение `true`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|inheritsPermissionsFrom| [Коллекция unifiedRoleDefinition](unifiedroledefinition.md)| Доступная только для чтения коллекция определений ролей, от которых наследуется заданное определение роли. Только Azure AD встроенные роли (**isBuiltIn — isBuiltIn**`true`) поддерживают этот атрибут. Поддерживает `$expand`. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": "Boolean",
  "isEnabled": "Boolean",
  "resourceScopes": [
    "String"
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.unifiedRolePermission"
    }
  ],
  "templateId": "String",
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

