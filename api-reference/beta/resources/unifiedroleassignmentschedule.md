---
title: тип ресурса unifiedRoleAssignmentSchedule
description: Представляет расписание операций по активному назначению ролей через Azure AD управление привилегированными пользователями.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8f5f58fd2130f4eaae7cf35d9fecc3b00d34c9b1
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509051"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>тип ресурса unifiedRoleAssignmentSchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание назначения активной роли через Azure AD управление привилегированными пользователями. **УнифицированнаяRoleAssignmentSchedule** создается единой [службойRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) и используется для мгновенного создания единой [системыRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md). Этот ресурс поддерживает список и извлекает операции для получения расписания для просмотра текущих и будущих назначений.

Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список unifiedRoleAssignmentSchedules](../api/unifiedroleassignmentschedule-list.md)|[коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получите список объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств.|
|[Get unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) .|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получите список объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId** , чтобы ограничить область для определенных объектов каталогов, например административных единиц. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|assignmentType|Строка|Тип назначения. Это может быть или `Assigned` `Activated`.|
|createdDateTime|DateTimeOffset|Время создания расписания. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|Строка|ID ролиAssignmentScheduleRequest, создав этот график. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|String|Уникальный идентификатор для unifiedRoleAssignmentSchedule. Key, not nullable, Read-only. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|Строка|Тип членства назначения. Это может быть или `Inherited`, `Direct`или `Group`.|
|modifiedDateTime|DateTimeOffset|При последнем обновлении расписания. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|Строка| Объект объекта, которому предоставляется назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Поддерживает `$filter` (`eq`).|
|roleDefinitionId|Строка|ID унифицированногоRoleDefinition для назначения. Только для чтения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Поддерживает `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса назначения ролей.|
|status|String|Состояние для `roleAssignmentSchedule`. Он может включать сообщения, связанные с состоянием, как `Provisioned`, `Revoked`и `Pending Provisioning``Pending Approval`. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Если рольAssignmentSchedule активируется roleEligibilitySchedule, это ссылка на этот график.|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Будет обесценить. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога `$expand` с помощью одновременно с назначением ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на главного, получаюного назначение ролей через запрос. При условии, что звонители могут получать основное использование `$expand` одновременно с назначением ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли `$expand` , используя одновременно с назначением роли. roleDefinition.Id будет автоматически расширена. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

