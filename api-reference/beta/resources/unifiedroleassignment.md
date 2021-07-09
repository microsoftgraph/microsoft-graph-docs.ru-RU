---
title: тип ресурса unifiedRoleAssignment
description: Назначение ролей — это связь между определением роли и главным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 16e03168f9eee4af8c6e69c7ee4fb774494643b4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351001"
---
# <a name="unifiedroleassignment-resource-type"></a>тип ресурса unifiedRoleAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для предоставления доступа к ресурсам используется единая системаRoleAssignment. Он представляет определение роли, назначенное основному (обычно пользователю) в определенной области.

Необходимо предоставить directoryScopeId или appScopeId.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список unifiedRoleAssignment](../api/rbacapplication-list-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Ознакомьтесь со списком объектов unifiedRoleAssignment и их свойствами. |
| [Get unifiedRoleAssignment](../api/unifiedroleassignment-get.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Чтение свойств и связей объекта unifiedRoleAssignment. |
| [Создание unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Создайте новую унифицированную функциюRoleAssignment, разместив в коллекции roleAssignment. |
| [Удаление unifiedRoleAssignment](../api/unifiedroleassignment-delete.md) | Нет | Удаление объекта unifiedRoleAssignment. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Уникальный идентификатор для единойRoleAssignment. Key, not nullable, Read-only. |
|roleDefinitionId|Строка| Идентификатор унифицированногоRoleDefinition для назначения. Только для чтения. Поддерживает `$filter` `eq` (только оператор). |
|principalId|Строка| Идентификатор основного, которому предоставляется назначение. Поддерживает `$filter` `eq` (только оператор). |
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением.|
|appScopeId|Строка|Идентификатор конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением.  Для поставщика управления правами используйте области приложений для указания каталога, например `/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997` .|
|resourceScope|Строка| Область применения unifiedRoleAssignment. Это для `/` всей службы. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось.**|

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|appScope|[appScope](appscope.md)|Сведения о конкретной области приложения, когда область назначения является конкретной. Объект containment. |
|directoryScope|[directoryObject](directoryobject.md)|Объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей. Только для чтения. Поддерживает `$expand`. |
|основной|[directoryObject](directoryobject.md)| Назначенная директор. При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей. Только для чтения. Поддерживает `$expand`. |
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|РольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. **roleDefinition.id** будет автоматически расширена. Поддерживает `$expand`. |



## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalId": "String",
  "principal": {"@odata.type": "microsoft.graph.directoryObject"},
  "directoryScopeId": "String",
  "directoryScope": {"@odata.type": "microsoft.graph.directoryObject"},
  "appScopeId": "String",
  "appScope": {"@odata.type": "microsoft.graph.appScope"},
  "resourceScope": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
