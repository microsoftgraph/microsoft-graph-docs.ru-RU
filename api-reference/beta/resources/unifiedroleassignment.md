---
title: Тип ресурса unifiedRoleAssignment
description: Назначение роли — это связь между определением роли и основным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4dc0ec6bb692c88d2b01a440bae1d7789bd042a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159033"
---
# <a name="unifiedroleassignment-resource-type"></a>Тип ресурса unifiedRoleAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для предоставления доступа к ресурсам используется unifiedRoleAssignment. Он представляет определение роли, назначенное основному пользователю в определенной области.

Требуется предоставить directoryScopeId или appScopeId.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get unifiedRoleAssignment](../api/unifiedroleassignment-get.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Чтение свойств и связей объекта unifiedRoleAssignment. |
| [Создание unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Создание нового unifiedRoleAssignment путем публикации в коллекции roleAssignment. |
| [Удаление unifiedRoleAssignment](../api/unifiedroleassignment-delete.md) | Нет | Удаление объекта unifiedRoleAssignment. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор unifiedRoleAssignment. Ключ, а не значение null, только для чтения. |
|roleDefinitionId|String| ИД unifiedRoleDefinition, для который требуется назначение. Только для чтения. |
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|Свойство, указывающее roleDefinition, для которого назначение. Предоставляется для того, чтобы вызыватели могли получить определение роли одновременно с получением `$expand` назначения роли. roleDefinition.Id будет автоматически расширена
|principalId|String| Objectid основного объекта, которому предоставлено назначение. |
|principal|[directoryObject](directoryobject.md)| Свойство, ссылаясь на назначенного директора. Предоставляется для того, чтобы вызыватели могли получить основное значение одновременно с получением `$expand` назначения роли. Только для чтения. |
|directoryScopeId|String|ИД объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым был предоставлен доступ для основного. Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями. Области приложения — это области, которые определяются и понятны только этому приложению.|
|directoryScope|[directoryObject](directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения. Предоставляется для того, чтобы вызыватели могли получить объект каталога одновременно с получением `$expand` назначения роли. Только для чтения. |
|appScopeId|String|ИД конкретной области приложения, если область назначения является конкретной областью приложения. Область назначения определяет набор ресурсов, к которым был предоставлен доступ для основного. Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями. Используйте "/" для области на клиенте. Области приложения — это области, которые определяются и понятны только этому приложению.|
|appScope|[appScope](appscope.md)|Свойство только для чтения с подробными сведениями об определенной области приложения, если область назначения является конкретной областью приложения. Объект Containment. |
|resourceScope|String| Область применения unifiedRoleAssignment. Это "/" для службы. **НЕ ИСПОЛЬЗУЙТЕ. Это свойство скоро будет неподготовлено.**|

## <a name="relationships"></a>Связи

Нет

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

