---
title: Тип ресурса unifiedRoleScheduleBase
description: Шаблон, предоставляющий свойства и связи, используемые в типах ресурсов unifiedRoleAssignmentSchedule и unifiedRoleEligibilitySchedule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9f778ac684ddb0ef9ae04647c4aa12193dff919c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134525"
---
# <a name="unifiedroleschedulebase-resource-type"></a>Тип ресурса unifiedRoleScheduleBase

Пространство имен: microsoft.graph

Шаблон, предоставляющий свойства и связи, используемые в [типах ресурсов unifiedRoleAssignmentSchedule](unifiedroleassignmentschedule.md) и [unifiedRoleEligibilitySchedule](unifiedroleeligibilityschedule.md) .


Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

Нет.

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRoleScheduleBases](../api/unifiedroleschedulebase-list.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) collection|Get a list of the [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) objects and their properties.|
|[Get unifiedRoleScheduleBase](../api/unifiedroleschedulebase-get.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|Read the properties and relationships of an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[Update unifiedRoleScheduleBase](../api/unifiedroleschedulebase-update.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|Update the properties of an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[Delete unifiedRoleScheduleBase](../api/unifiedroleschedulebase-delete.md)|None|Deletes an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[List appScope](../api/unifiedroleschedulebase-list-appscope.md)|[appScope](../resources/appscope.md) collection|Get the appScope resources from the appScope navigation property.|
|[Add appScope](../api/unifiedroleschedulebase-post-appscope.md)|[appScope](../resources/appscope.md)|Add appScope by posting to the appScope collection.|
|[List directoryScope](../api/unifiedroleschedulebase-list-directoryscope.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the directoryScope navigation property.|
|[Add directoryScope](../api/unifiedroleschedulebase-post-directoryscope.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScope by posting to the directoryScope collection.|
|[List principal](../api/unifiedroleschedulebase-list-principal.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the principal navigation property.|
|[Add principal](../api/unifiedroleschedulebase-post-principal.md)|[directoryObject](../resources/directoryobject.md)|Add principal by posting to the principal collection.|
|[List unifiedRoleDefinition](../api/unifiedroleschedulebase-list-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinition resources from the roleDefinition navigation property.|
|[Add unifiedRoleDefinition](../api/unifiedroleschedulebase-post-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|

-->

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, относяшейся к конкретному приложению, если назначение или право на доступ относятся к приложению. Область назначения или права на участие определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами.|
|createdDateTime|DateTimeOffset|При создании расписания.|
|createdUsing|String|Идентификатор объекта, с помощью которого было создано это расписание.|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения или допустимости. Область назначения или права на участие определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением.|
|id|String|Уникальный идентификатор объекта расписания. Наследуется от [сущности](../resources/entity.md).|
|modifiedDateTime|DateTimeOffset|Время последнего изменения расписания.|
|principalId|String|Идентификатор субъекта, которым было предоставлено назначение роли или право на участие.|
|roleDefinitionId|String|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , назначаемого субъекту или доступного субъекту.|
|status|String|Состояние назначения роли или запроса на приемлемость.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если доступ к роли или назначение относятся к приложению. Допускается значение null.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью действия или назначения роли. Только для чтения.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает назначение роли или может получить роль с помощью запроса.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об объекте roleDefinition, на который ссылаются через **свойство roleDefinitionId** .|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String"
}
```

