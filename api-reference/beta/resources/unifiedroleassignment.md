---
title: тип ресурса unifiedRoleAssignment
description: Назначение ролей — это связь между определением роли и главным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c52e6bb05c9258680a36f04ad428c24a3a2829fc
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239973"
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
|appScopeId|Строка|Идентификатор конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением.|
|resourceScope|Строка| Область применения unifiedRoleAssignment. Это для `/` всей службы. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось.**|

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|appScope|[appScope](appscope.md)|Сведения о конкретной области приложения, когда область назначения является конкретной. Объект containment. |
|directoryScope|[directoryObject](directoryobject.md)|Объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей. Только для чтения. Поддерживает `$expand`. |
|основной|[directoryObject](directoryobject.md)| Назначенная директор. При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей. Только для чтения. Поддерживает `$expand`. |
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|РольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. **roleDefinition.id** будет автоматически расширена. Поддерживает `$expand`. |



## <a name="json-representation"></a>Представление в формате JSON

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

