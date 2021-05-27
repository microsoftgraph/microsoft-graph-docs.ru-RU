---
title: тип ресурса unifiedRoleAssignmentSchedule
description: Представляет расписание операций по активному назначению ролей через Azure AD управление привилегированными пользователями.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f89a6e1c7fecac535c8f0a50d7888aa65c7d94cc
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682280"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>тип ресурса unifiedRoleAssignmentSchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание назначения активной роли через Azure AD управление привилегированными пользователями. A `roleAssignmentSchedule` создается `roleAssignmentScheduleRequest` и используется для мгновенного создания `roleAssignmentInstance` . Мы поддерживаем список и получаем операции для получения расписания для просмотра текущих и будущих назначений.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список unifiedRoleAssignmentSchedules](../api/unifiedroleassignmentschedule-list.md)|[коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получите список объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств.|
|[Get unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentSchedule.](../resources/unifiedroleassignmentschedule.md)|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получите список объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Id конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте "/" для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|assignmentType|String|Тип назначения. Это может быть `Assigned` или `Activated` .|
|createdDateTime|DateTimeOffset|Время создания расписания. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|String|ID ролиAssignmentScheduleRequest, создав этот график. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|String|Id объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|String|Уникальный идентификатор для unifiedRoleAssignmentSchedule. Key, not nullable, Read-only. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|String|Тип членства назначения. Это может быть `Inherited` или `Direct` , или `Group` .|
|modifiedDateTime|DateTimeOffset|При последнем обновлении расписания. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|String| Объект объекта, которому предоставляется назначение. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinitionId|String|ID унифицированногоRoleDefinition для назначения. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса назначения ролей.|
|status|String|Состояние `roleAssignmentSchedule` для . Он может включать сообщения, связанные с `Provisioned` состоянием, как , и `Revoked` `Pending Provisioning` `Pending Approval` . Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Если рольAssignmentSchedule активируется roleEligibilitySchedule, это ссылка на этот график.|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Будет обесценить. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на главного, получаюного назначение ролей через запрос. При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. roleDefinition.Id будет автоматически расширена. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentSchedule",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "assignmentType": "String",
  "memberType": "String"
}
```

