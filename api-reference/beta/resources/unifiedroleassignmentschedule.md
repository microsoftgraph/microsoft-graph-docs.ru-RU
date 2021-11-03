---
title: тип ресурса unifiedRoleAssignmentSchedule
description: Представляет расписание операций по активному назначению ролей через Azure AD управление привилегированными пользователями.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5fc9e1777dd3cb5510aa52bb8c6a6df25b4189a5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696686"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>тип ресурса unifiedRoleAssignmentSchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание назначения активной роли через Azure AD управление привилегированными пользователями. **УнифицированнаяRoleAssignmentSchedule** создается единой [службойRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) и используется для мгновенного создания [единой системыRoleAssignmentScheduleInstance.](unifiedroleassignmentscheduleinstance.md) Этот ресурс поддерживает список и извлекает операции для получения расписания для просмотра текущих и будущих назначений.

Наследует [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список unifiedRoleAssignmentSchedules](../api/unifiedroleassignmentschedule-list.md)|[коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получите список объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств.|
|[Get unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentSchedule.](../resources/unifiedroleassignmentschedule.md)|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получите список объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область для определенных объектов каталогов, например административных единиц. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|assignmentType|String|Тип назначения. Это может быть `Assigned` или `Activated` .|
|createdDateTime|DateTimeOffset|Время создания расписания. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|String|ID ролиAssignmentScheduleRequest, создав этот график. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|String|Уникальный идентификатор для unifiedRoleAssignmentSchedule. Key, not nullable, Read-only. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|String|Тип членства назначения. Это может быть `Inherited` или `Direct` , или `Group` .|
|modifiedDateTime|DateTimeOffset|При последнем обновлении расписания. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|String| Объект объекта, которому предоставляется назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Поддерживает `$filter` (`eq`).|
|roleDefinitionId|String|ID унифицированногоRoleDefinition для назначения. Только для чтения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Поддерживает `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса назначения ролей.|
|status|String|Состояние `roleAssignmentSchedule` для . Он может включать сообщения, связанные с `Provisioned` состоянием, как , и `Revoked` `Pending Provisioning` `Pending Approval` . Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|

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

