---
title: Тип ресурса unifiedRoleDefinition
description: Унифицированное определение роли — это коллекция разрешений
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d146f215586533b9564d267c686a437f1314d54b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159831"
---
# <a name="unifiedroledefinition-resource-type"></a>Тип ресурса unifiedRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

UnifiedRoleDefinition — это коллекция разрешений, перечисляет операции, которые можно выполнять, например чтение, запись и удаление.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [коллекция unifiedRoleDefinition](unifiedroledefinition.md) | Чтение списка объектов unifiedRoleDefinition и их свойств. |
| [Get unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Чтение свойств объекта unifiedRoleDefinition. |
| [Создание unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Создание объекта unifiedRoleDefinition. |
| [Обновление unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Обновление объекта unifiedRoleDefinition. |
| [Удаление unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | Нет | Удаление объекта unifiedRoleDefinition. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String| Описание unifiedRoleDefinition. Только для чтения, если isBuiltIn имеет true. |
|displayName|String| Отображаемое имя unifiedRoleDefinition. Только для чтения, если isBuiltIn имеет true. Обязательный.|
|id|String| Уникальный идентификатор для unifiedRoleDefinition. Ключ, а не значение null, только для чтения. |
|isBuiltIn|Boolean| Флаг, указывающий, является ли unifiedRoleDefinition частью набора по умолчанию, включенного в продукт или пользовательский. Только для чтения. |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если заведомо неверно, роль недоступна для назначения. Только для чтения, если isBuiltIn имеет true. |
|resourceScopes|Коллекция String| К списку областей применяются разрешения, предоставленные определением роли. В настоящее время поддерживается только "/". Только для чтения, если isBuiltIn имеет true. **НЕ ИСПОЛЬЗУЙТЕ. Скоро эта возможность будет неподготовлена. Присоединение области к назначению роли** | 
|rolePermissions|[коллекция unifiedRolePermission](unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, если isBuiltIn имеет true. Обязательно. |
|templateId|String| Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn имеет false. Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым для разных каталогов. Только для чтения, если isBuiltIn имеет true. |
|inheritsPermissionsFrom| [коллекция unifiedRoleDefinition](unifiedroledefinition.md)| Коллекция определений ролей только для чтения, от которую наследуется заданное определение роли. Этот атрибут поддерживается только встроенными ролями Azure AD. |
|version|String| Указывает версию unifiedRoleDefinition. Только для чтения, если isBuiltIn имеет true.|

## <a name="relationships"></a>Связи

Нет

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


