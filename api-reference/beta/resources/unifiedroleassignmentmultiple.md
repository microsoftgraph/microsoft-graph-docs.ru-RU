---
title: тип ресурса unifiedRoleAssignmentMultiple
description: Назначение ролей — это связь между определением роли и главным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f612fea9ce7aa54cce505a4f2d77370f45947c44
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442707"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>тип ресурса unifiedRoleAssignmentMultiple

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для предоставления доступа к ресурсам используется unifiedRoleAssignmentMultiple. Оно представляет определение роли, назначенное массиву принципов (как правило, пользователю) по массиву областей. Примером такого поставщика RBAC является Microsoft Intune. В Microsoft Intune можно создать назначение ролей с несколькими основными и несколькими областьми.

Необходимо **предоставить либо directoryScopeIds,** либо **appScopeIds.**

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Чтение свойств и связей объекта unifiedRoleAssignmentMultiple. |
| [Создание unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Создайте новую единую системуRoleAssignmentMultiple, разместив в коллекции roleAssignment. |
| [Обновление unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Обновление существующего объекта unifiedRoleAssignmentMultiple. |
| [Удаление unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | Нет | Удаление объекта unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| id | String | Уникальный идентификатор для единойRoleAssignmentMultiple. Key, not nullable, Read-only. |
| displayName | String | Имя назначения роли. Обязательный. |
| description | String | Описание назначения роли. |
| roleDefinitionId | String | ID унифицированногоRoleDefinition для назначения. |
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. Только для чтения.  |
| principalIds | Коллекция строк | Objectids of the principals to which the assignment is granted. |
| основные| Коллекция [directoryObject](directoryobject.md) | Коллекция только для чтения, ссылаясь на назначенных директоров. При условии, что звонители смогут получать главные принципы одновременно с `$expand` назначением ролей. Только для чтения. |
| directoryScopeIds | Коллекция строк | Ids объектов каталога, представляющих области назначения. Области назначения определяют набор ресурсов, к которым доверимы получили доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением. |
| directoryScopes | Коллекция [directoryObject](directoryobject.md) | Коллекция только для чтения, ссылаясь на объекты каталога, которые являются областью назначения. При условии, что вызыватели могут получать объекты каталога, используя одновременно `$expand` с назначением ролей. Только для чтения. |
| appScopeIds | Коллекция строк | Ids of the app specific scopes when the assignment scopes are app specific. Области назначения определяют набор ресурсов, для которых доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте "/" для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением. |
| appScopes | [коллекция appScope](appscope.md) |Коллекция только для чтения с подробными сведениями о конкретных областях приложения, когда области назначения являются конкретными приложениями. Объект containment. Только для чтения.  |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalIds": ["string"],
  "principals": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directoryScopeIds": ["string"],
  "directoryScopes": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "appScopeIds": ["string"],
  "appScopes": [{"@odata.type": "microsoft.graph.appScope"}],
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignmentMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


