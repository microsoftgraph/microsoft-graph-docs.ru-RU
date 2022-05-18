---
title: Тип ресурса unifiedRoleAssignmentSchedule
description: Представляет расписание для активных операций назначения ролей через Azure AD управление привилегированными пользователями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ab32cf141bf16b8b763c5b2d54700df7d3f3d8a9
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461627"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>Тип ресурса unifiedRoleAssignmentSchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание для назначения активной роли через Azure AD управление привилегированными пользователями. **UnifiedRoleAssignmentSchedule** создается с помощью [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) и используется для создания экземпляра [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md). Этот ресурс поддерживает операции получения списка и получения расписания для просмотра текущих и будущих назначений.

Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleAssignmentSchedule](../api/rbacapplication-list-roleassignmentschedules.md)|[Коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получение списка объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств.|
|[Получение unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Чтение свойств и связей объекта [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) .|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[Коллекция unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Получение списка объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|assignmentType|String|Тип назначения. Это может быть либо `Assigned` .`Activated`|
|createdDateTime|DateTimeOffset|Время создания расписания. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|Строка|Идентификатор ролиAssignmentScheduleRequest, создавшего это расписание. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|Строка|Уникальный идентификатор объекта unifiedRoleAssignmentSchedule. Ключ, не допускающий значения NULL, только для чтения. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|Строка|Тип членства назначения. Это может быть либо `Inherited`, `Direct`, либо `Group`.|
|modifiedDateTime|DateTimeOffset|Время последнего обновления расписания. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|Строка| Objectid субъекта, которому предоставляется назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Поддерживает `$filter` (`eq`).|
|roleDefinitionId|Строка|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Только для чтения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Поддерживает `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение роли.|
|status|String|Состояние для .`roleAssignmentSchedule` Он может включать сообщения, связанные с состоянием, такие `Provisioned`как , `Revoked`, и `Pending Provisioning``Pending Approval`. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Если roleAssignmentSchedule активируется roleEligibilitySchedule, это ссылка на это расписание.|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Будет нерекомендуемым. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если область назначения предназначена для конкретного приложения. Сущность containment. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на объект каталога, который является областью назначения. Предоставляется для того, чтобы вызывающие объекты могли получить объект каталога `$expand` , используя одновременно с получением назначения роли. Только для чтения. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|Основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на субъект, который получает назначение роли через запрос. Предоставляется для того, чтобы вызывающие объекты `$expand` могли получить субъект одновременно с получением назначения роли. Только для чтения. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее roleDefinition, для которых предназначено назначение. Предоставляется для того, чтобы вызывающие объекты могли получить определение роли `$expand` одновременно с получением назначения роли. roleDefinition.Id будет автоматически развернут. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

