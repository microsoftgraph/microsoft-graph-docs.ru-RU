---
title: тип ресурса unifiedRoleDefinition
description: Единое определение роли — это набор разрешений
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c1d9f11a71aa9b6a611cab259801f34cd889deb5
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524632"
---
# <a name="unifiedroledefinition-resource-type"></a>тип ресурса unifiedRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию разрешений с перечислением операций, таких как чтение, запись и удаление, которые могут выполняться поставщиком RBAC в рамках управления Microsoft 365 [RBAC](rolemanagement.md).

В настоящее время поддерживаются следующие поставщики RBAC:
- Облачный КОМПЬЮТЕР 
- управление устройствами (Intune)
- каталог (Azure AD) 
- управление правами (Azure AD)


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [коллекция unifiedRoleDefinition](unifiedroledefinition.md) | Ознакомьтесь со списком объектов unifiedRoleDefinition и их свойствами. |
| [Get unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Ознакомьтесь с свойствами объекта unifiedRoleDefinition. |
| [Создание unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Создайте объект unifiedRoleDefinition. |
| [Обновление unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Обновление объекта unifiedRoleDefinition. |
| [Удаление unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | Нет | Удаление объекта unifiedRoleDefinition. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|Строка| Описание единогоRoleDefinition. Только для чтения, **когда isBuiltIn** является правдой. |
|displayName|Строка| Имя отображения для unifiedRoleDefinition. Только для чтения, **когда isBuiltIn** является правдой. Обязательно.  Поддерживает `$filter` `eq` (и `startsWith` только операторов).|
|id|Строка| Уникальный идентификатор для единойRoleDefinition. Key, not nullable, Read-only.  Поддерживает `$filter` `eq` (только оператор). |
|isBuiltIn|Boolean| Флаг, указывающий, является ли unifiedRoleDefinition частью набора по умолчанию, включенного в продукт или настраиваемый. Только для чтения.  Поддерживает `$filter` `eq` (только оператор).|
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если значение false, роль недоступна для назначения. Только для чтения, **когда isBuiltIn** является правдой. |
|resourceScopes|Коллекция String| К списку областей применяются разрешения, предоставленные определением ролей. В настоящее `/` время поддерживается только. Только для чтения, когда isBuiltIn является правдой. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это будет отохошено. Присоединение области к назначению ролей** | 
|rolePermissions|[коллекция unifiedRolePermission](unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, **когда isBuiltIn** является правдой. Обязательно. |
|templateId|Строка| Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным. Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах. Только для чтения, **когда isBuiltIn** является правдой. |
|version|String| Указывает версию единойRoleDefinition. Только для чтения, **когда isBuiltIn** является правдой.|

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|inheritsPermissionsFrom| [коллекция unifiedRoleDefinition](unifiedroledefinition.md)| Только для чтения набор определений ролей, которые наследует заданное определение роли. Только встроенные роли Azure AD поддерживают этот атрибут. |

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


