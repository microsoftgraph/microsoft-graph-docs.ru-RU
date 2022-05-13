---
title: Тип ресурса unifiedRoleScheduleInstanceBase
description: Базовое свойство экземпляра унифицированного расписания ролей, объединяющее экземпляр расписания назначения унифицированных ролей и экземпляр расписания соответствия унифицированной роли
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 78da74c6a867d6beed5dada2576d6248fc68ef37
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399448"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Тип ресурса unifiedRoleScheduleInstanceBase

Пространство имен: microsoft.graph

Базовое свойство экземпляра унифицированного расписания ролей, объединяющее экземпляры расписания назначения унифицированных ролей и экземпляры расписания соответствия унифицированным ролям.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. |
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. |
|id|String|Уникальный идентификатор объекта unifiedRoleAssignmentScheduleInstance. Ключ, не допускающий значения NULL, только для чтения.|
|principalId|String|Идентификатор субъекта, которому предоставляется назначение. Может быть группой или пользователем. |
|roleDefinitionId|String|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Только для чтения. <br> Поддерживает `$filter` (`eq`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если область назначения предназначена для конкретного приложения. Сущность containment. |
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью назначения. Включает извлечение объекта `$expand` каталога, используя одновременно с получением назначения роли. Только для чтения.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает назначение роли через запрос. Включает извлечение субъекта `$expand` , используя одновременно с получением назначения роли. Только для чтения.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|RoleDefinition для назначения. Позволяет получить определение роли одновременно `$expand` с получением назначения роли. Список roleDefinition.Id развертывается автоматически.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleInstanceBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String"
}
```
