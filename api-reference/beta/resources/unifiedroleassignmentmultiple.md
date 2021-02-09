---
title: Тип ресурса unifiedRoleAssignmentMultiple
description: Назначение роли — это связь между определением роли и основным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4df17c6b112cefe03a12631ee763f49e976fb568
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159845"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>Тип ресурса unifiedRoleAssignmentMultiple

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для предоставления доступа к ресурсам используется unifiedRoleAssignmentMultiple. Он представляет определение роли, назначенное массиву основных ролей (обычно пользователю) в массиве областей. Примером такого поставщика RBAC является Microsoft Intune. В Microsoft Intune можно создать назначение роли с несколькими основными и несколькими уровнями.

Требуется **предоставить directoryScopeIds** или **appScopeIds.**

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Чтение свойств и связей объекта unifiedRoleAssignmentMultiple. |
| [Создание unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Создание новой unifiedRoleAssignmentMultiple путем публикации в коллекции roleAssignment. |
| [Обновление unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Обновление существующего объекта unifiedRoleAssignmentMultiple. |
| [Удаление unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | Нет | Удаление объекта unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| id | String | Уникальный идентификатор unifiedRoleAssignmentMultiple. Ключ, не значение null, только для чтения. |
| displayName | String | Имя назначения роли. Обязательный. |
| description | String | Описание назначения роли. |
| roleDefinitionId | String | ИД unifiedRoleDefinition, для который требуется назначение. |
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |Свойство, указывающее roleDefinition, для которого назначение. Предоставляется, чтобы вызыватели могли получить определение роли одновременно с получением `$expand` назначения роли. Только для чтения.  |
| principalIds | Коллекция String | Objectids of the principals to which the assignment is granted. |
| principals| Коллекция [directoryObject](directoryobject.md) | Коллекция только для чтения, ссылаясь на назначенную сумму. Предоставляется для того, чтобы вызыватели могли получать основных ролей, используя `$expand` одновременно с получением назначения роли. Только для чтения. |
| directoryScopeIds | Коллекция String | ИД объектов каталога, представляющих области назначения. Области назначения определяют набор ресурсов, к которым были предоставлены доступ к этим ресурсам. Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями. Области приложения — это области, которые определяются и понятны только этому приложению. |
| directoryScopes | Коллекция [directoryObject](directoryobject.md) | Коллекция только для чтения, ссылаясь на объекты каталога, которые являются областью назначения. Предоставляется для того, чтобы вызыватели могли получать объекты каталога одновременно с получением `$expand` назначения роли. Только для чтения. |
| appScopeIds | Коллекция String | Ids of the app specific scopes when the assignment scopes are app specific. Области назначения определяют набор ресурсов, к которым был предоставлен доступ для основного. Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями. Используйте "/" для области на клиенте. Области приложения — это области, которые определяются и понятны только этому приложению. |
| appScopes | [Коллекция appScope](appscope.md) |Коллекция только для чтения с подробными сведениями об областях приложения, если области назначения являются конкретными для приложения. Объект Containment. Только для чтения.  |

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


