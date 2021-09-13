---
title: тип ресурса unifiedRoleDefinition
description: Определение роли — это коллекция разрешений в Azure Active Directory (Azure AD).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2307b6fd429e8cc4942a5a50e04316ee77332671
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148527"
---
# <a name="unifiedroledefinition-resource-type"></a>тип ресурса unifiedRoleDefinition

Пространство имен: microsoft.graph

Определение ролей — это набор разрешений в Azure Active Directory Azure AD, в котором перечисляются операции, которые можно выполнить, и ресурсы, с которыми они могут выполняться.

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
|description|String| Описание единогоRoleDefinition. Только для чтения, **когда isBuiltIn** `true` является . |
|displayName|String| Имя отображения для unifiedRoleDefinition. Только для чтения, **когда isBuiltIn** `true` является . Обязательно.  Поддерживает $filter ( `eq` , `in` ).|
|id|String| Уникальный идентификатор определения роли. Key, not nullable, Read-only. Наследуется от [сущности](../resources/entity.md). Поддерживает $filter ( `eq` , `in` ). |
|isBuiltIn|Boolean| Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в Azure Active Directory (Azure AD) или настраиваемого определения. Только для чтения. Поддерживает $filter ( `eq` , `in` ). |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если `false` роль недоступна для назначения. Только для чтения, **когда isBuiltIn** является правдой. |
|resourceScopes|Коллекция String| Список областей или разрешений, к которые применяется определение роли. В настоящее `/` время поддерживается только. Только для чтения, **когда isBuiltIn** является правдой. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это будет отохошено. Прикрепить область к назначению ролей.** | 
|rolePermissions|[коллекция unifiedRolePermission](unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, **когда isBuiltIn** `true` является . Обязательно. |
|templateId|String| Настраиваемый идентификатор шаблона, который можно установить, когда **isBuiltIn,** но только для `false` чтения, **когда isBuiltIn** `true` . Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах. |
|version|String| Указывает версию определения роли. Только для чтения, **когда isBuiltIn** `true` является .|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|inheritsPermissionsFrom| [коллекция unifiedRoleDefinition](unifiedroledefinition.md)| Только для чтения набор определений ролей, которые наследует заданное определение роли. Только встроенные роли Azure AD **(isBuiltIn** `true` есть) поддерживают этот атрибут. Поддерживает `$expand`. |

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

