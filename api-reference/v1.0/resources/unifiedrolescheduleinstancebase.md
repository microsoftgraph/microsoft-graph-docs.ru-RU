---
title: Тип ресурса unifiedRoleScheduleInstanceBase
description: Шаблон, предоставляющий свойства и связи, используемые в типах ресурсов unifiedRoleAssignmentScheduleInstance и unifiedRoleEligibilityScheduleInstance.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 241c0af15867d87775490e00bd0f098e13e9dd9a
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134546"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Тип ресурса unifiedRoleScheduleInstanceBase

Пространство имен: microsoft.graph

Шаблон, предоставляющий свойства и связи, используемые в [типах ресурсов unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md) и [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md) .


Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

Нет. 

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRoleScheduleInstanceBases](../api/unifiedrolescheduleinstancebase-list.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) collection|Get a list of the [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) objects and their properties.|
|[Get unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-get.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Read the properties and relationships of an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[Update unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-update.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Update the properties of an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[Delete unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-delete.md)|None|Deletes an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[List appScope](../api/unifiedrolescheduleinstancebase-list-appscope.md)|[appScope](../resources/appscope.md) collection|Get the appScope resources from the appScope navigation property.|
|[Add appScope](../api/unifiedrolescheduleinstancebase-post-appscope.md)|[appScope](../resources/appscope.md)|Add appScope by posting to the appScope collection.|
|[List directoryScope](../api/unifiedrolescheduleinstancebase-list-directoryscope.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the directoryScope navigation property.|
|[Add directoryScope](../api/unifiedrolescheduleinstancebase-post-directoryscope.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScope by posting to the directoryScope collection.|
|[List principal](../api/unifiedrolescheduleinstancebase-list-principal.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the principal navigation property.|
|[Add principal](../api/unifiedrolescheduleinstancebase-post-principal.md)|[directoryObject](../resources/directoryobject.md)|Add principal by posting to the principal collection.|
|[List unifiedRoleDefinition](../api/unifiedrolescheduleinstancebase-list-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinition resources from the roleDefinition navigation property.|
|[Add unifiedRoleDefinition](../api/unifiedrolescheduleinstancebase-post-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
-->

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, относяшейся к приложению, если назначение или право на роль относятся к приложению. Область назначения или права на роль определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами.|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения или права на роль. Область назначения или права на роль определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением.|
|id|String|Уникальный идентификатор объекта расписания. Наследуется от [сущности](../resources/entity.md).|
|principalId|String|Идентификатор субъекта, которым было предоставлено назначение роли или который имеет право на роль.|
|roleDefinitionId|String|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , назначаемого субъекту или доступного субъекту.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если назначение или право на роль относятся к приложению. Допускается значение null.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью действия назначения или роли. Только для чтения.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает назначение роли или права на роль через запрос.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об объекте roleDefinition, на который ссылаются через **свойство roleDefinitionId** .|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "baseType": "microsoft.graph.entity",
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

