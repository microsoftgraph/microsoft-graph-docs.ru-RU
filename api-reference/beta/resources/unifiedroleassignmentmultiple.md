---
title: тип ресурса unifiedRoleAssignmentMultiple
description: Определение роли, назначенное массиву принципов (как правило, пользователю) по массиву областей.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4dc43e36ce1f224a920f99d02210268d68b42d40
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764033"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>тип ресурса unifiedRoleAssignmentMultiple

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для предоставления доступа к ресурсам в рамках управления Microsoft 365 [RBAC](rolemanagement.md)используется единое управление RbleAssignmentMultiple. Оно представляет определение роли, назначенное массиву принципов (как правило, пользователю) в массиве областей. 

Можно создать назначение ролей с несколькими основными и несколькими областьми.

Необходимо предоставить **либо directoryScopeIds,** либо **appScopeIds.**

В настоящее время поддерживаются следующие поставщики RBAC:
- Облачный КОМПЬЮТЕР 
- Microsoft Intune

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список объектов roleAssignment](../api/rbacapplicationmultiple-list-roleassignments.md) | [коллекция unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Ознакомьтесь со списком объектов unifiedRoleAssignmentMultiple и их свойствами. |
| [Создание unifiedRoleAssignmentMultiple](../api/rbacapplicationmultiple-post-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Создайте новую единую системуRoleAssignmentMultiple, разместив в коллекции roleAssignment. |
| [Получение unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Чтение свойств и связей объекта unifiedRoleAssignmentMultiple. |
| [Обновление unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Обновление существующего объекта unifiedRoleAssignmentMultiple. |
| [Удаление unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | Нет | Удаление объекта unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| appScopeIds | Коллекция объектов string | Ids of the app specific scopes when the assignment scopes are app specific. Области назначения определяют набор ресурсов, для которых доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением. |
| description | Строка | Описание назначения роли. |
| directoryScopeIds | Коллекция объектов string | Ids объектов каталога, представляющих области назначения. Области назначения определяют набор ресурсов, к которым доверимы получили доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением. |
| displayName | String | Имя назначения роли. Обязательный. |
| id | String | Уникальный идентификатор для единойRoleAssignmentMultiple. Key, not nullable, Read-only. |
| roleDefinitionId | String | Идентификатор унифицированногоRoleDefinition для назначения. |
| principalIds | Коллекция объектов string | Идентификаторы директоров, которым предоставляется назначение.  Поддерживает `$filter` `any` (только оператор). |


## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| appScopes | [коллекция appScope](appscope.md) |Коллекция только для чтения с подробными сведениями о конкретных областях приложения, когда области назначения являются конкретными приложениями. Объект containment. Только для чтения.  |
| directoryScopes | Коллекция [directoryObject](directoryobject.md) | Коллекция только для чтения, ссылаясь на объекты каталога, которые являются областью назначения. При условии, что вызыватели могут получать объекты каталога, используя одновременно `$expand` с назначением ролей. Только для чтения.  Поддерживает `$expand`.|
| основные| Коллекция [directoryObject](directoryobject.md) | Коллекция только для чтения, ссылаясь на назначенных директоров. При условии, что звонители смогут получать главные принципы одновременно с `$expand` назначением ролей. Только для чтения.  Поддерживает `$expand`.|
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |Указывает рольDefinition, для которую это назначение. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли.  Поддерживает `$filter` `eq` (оператор на **id,** **isBuiltIn** и **displayName** и `startsWith` оператор на **displayName)** и `$expand` . |


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


