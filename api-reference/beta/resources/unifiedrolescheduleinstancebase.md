---
title: Тип ресурса unifiedRoleScheduleInstanceBase
description: Шаблон, предоставляющий свойства и связи, используемые в типах ресурсов unifiedRoleAssignmentScheduleInstance и unifiedRoleEligibilityScheduleInstance.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a5248cfe962dbaf75b19ae3777a3d6a35f70e37e
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898702"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Тип ресурса unifiedRoleScheduleInstanceBase

Пространство имен: microsoft.graph

Шаблон, предоставляющий свойства и связи, используемые в [типах ресурсов unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md) и [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md) .


Наследует [от сущности](../resources/entity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, относяшейся к приложению, если назначение или право на роль относятся к приложению. Область назначения или права на роль определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами.|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения или права на роль. Область назначения или права на роль определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением.|
|id|Строка|Уникальный идентификатор объекта расписания. Наследуется от [сущности](../resources/entity.md).|
|principalId|Строка|Идентификатор субъекта, которым было предоставлено назначение роли или который имеет право на роль.|
|roleDefinitionId|Строка|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , назначаемого субъекту или доступного субъекту.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если назначение или право на роль относятся к приложению. Допускается значение null.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью действия назначения или роли. Только для чтения.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает назначение роли или права на роль через запрос.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об объекте roleDefinition, на который ссылаются через **свойство roleDefinitionId** .|

## <a name="json-representation"></a>Представление JSON
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