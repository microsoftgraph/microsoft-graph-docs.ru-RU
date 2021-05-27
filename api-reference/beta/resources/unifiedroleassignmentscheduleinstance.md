---
title: тип ресурса unifiedRoleAssignmentScheduleInstance
description: Представляет экземпляр расписания для активных операций назначения ролей через Azure AD управление привилегированными пользователями.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 205218bc1ab3bbb76cfd6566dd6a6c968e7f1f02
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682147"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>тип ресурса unifiedRoleAssignmentScheduleInstance

Пространство имен: microsoft.graph 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет экземпляр для активного назначения ролей через Azure AD управление привилегированными пользователями. A `roleAssignmentInstance` создается `roleAssignmentSchedule` и представляет фактическую рольAssignment, созданную управление привилегированными пользователями. Мы поддерживаем список и получаем операции на roleAssignmentInstance для просмотра текущих и будущих назначений.

Наследует [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список unifiedRoleAssignmentScheduleInstances](../api/unifiedroleassignmentscheduleinstance-list.md)|[коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Получите список объектов [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) и их свойств.|
|[Get unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-get.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)|
|[filterByCurrentUser](../api/unifiedroleassignmentscheduleinstance-filterbycurrentuser.md)|[коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Получите список объектов [unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Id конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте "/" для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|assignmentType|String|Тип назначения. Это может быть `Assigned` или `Activated` .|
|createdDateTime|DateTimeOffset|Время создания расписания.|
|directoryScopeId|String|Id объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|endDateTime|DateTimeOffset|Время истечения срока действия ролиAssignmentInstance|
|id|String|Уникальный идентификатор для unifiedRoleAssignmentScheduleInstance. Key, not nullable, Read-only. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|memberType|String|Тип членства назначения. Это может быть `Inherited` или `Direct` , или `Group` .|
|principalId|String|Объект объекта, которому предоставляется назначение. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleAssignmentOriginId|String|ID ролиAssignment в каталоге|
|roleAssignmentScheduleId|String|ID родительской ролиAssignmentSchedule для этого экземпляра|
|roleDefinitionId|String|ID унифицированногоRoleDefinition для назначения. Только для чтения. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|startDateTime|DateTimeOffset|Время запуска ролиAssignmentInstance|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Если рольAssignmentScheduleInstance активируется roleEligibilityScheduleRequest, это ссылка на соответствующий экземпляр расписания.|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на главного, получаюного назначение ролей через запрос. При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. roleDefinition.Id будет автоматически расширена. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleInstance",
  "baseType": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleInstance",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentType": "String",
  "memberType": "String",
  "roleAssignmentOriginId": "String",
  "roleAssignmentScheduleId": "String"
}
```

