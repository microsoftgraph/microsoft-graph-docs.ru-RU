---
title: Тип ресурса unifiedRoleAssignmentScheduleInstance
description: Представляет экземпляр расписания для активных операций назначения ролей через Azure AD управление привилегированными пользователями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b62f1c8016bad6b5a1240eb953de444f9f3f9435
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399413"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>Тип ресурса unifiedRoleAssignmentScheduleInstance

Пространство имен: microsoft.graph 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет экземпляр для активного назначения роли через Azure AD управление привилегированными пользователями. **UnifiedRoleAssignmentScheduleInstance** создается с помощью [unifiedRoleAssignmentSchedule](unifiedroleassignmentschedule.md) и представляет фактическое назначение роли, созданное управление привилегированными пользователями. Этот ресурс поддерживает операции list и Get для просмотра текущих и будущих назначений.

Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-list.md)|[Коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Получение списка объектов [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) и их свойств.|
|[Получение unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-get.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Чтение свойств и связей объекта [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) .|
|[filterByCurrentUser](../api/unifiedroleassignmentscheduleinstance-filterbycurrentuser.md)|[Коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Получение списка объектов [unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|assignmentType|String|Тип назначения. Это может быть либо `Assigned` .`Activated`|
|createdDateTime|DateTimeOffset|Время создания расписания.|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|endDateTime|DateTimeOffset|Время истечения срока действия ролиAssignmentInstance|
|id|String|Уникальный идентификатор объекта unifiedRoleAssignmentScheduleInstance. Ключ, не допускающий значения NULL, только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|memberType|String|Тип членства назначения. Это может быть либо `Inherited`, `Direct`, либо `Group`.|
|principalId|String|Идентификатор субъекта, которому предоставляется назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleAssignmentOriginId|String|Идентификатор ролиAssignment в каталоге|
|roleAssignmentScheduleId|String|Идентификатор родительской ролиAssignmentSchedule для этого экземпляра|
|roleDefinitionId|String|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).  <br> Поддерживает `$filter` (`eq`).|
|startDateTime|DateTimeOffset|Время запуска roleAssignmentInstance|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Если roleAssignmentScheduleInstance активируется с помощью roleEligibilityScheduleRequest, это ссылка на связанный экземпляр расписания.|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если область назначения предназначена для конкретного приложения. Сущность containment. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на объект каталога, который является областью назначения. Предоставляется для того, чтобы вызывающие объекты могли получить объект каталога `$expand` , используя одновременно с получением назначения роли. Только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|Основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на субъект, который получает назначение роли через запрос. Предоставляется для того, чтобы вызывающие объекты `$expand` могли получить субъект одновременно с получением назначения роли. Только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее roleDefinition, для которых предназначено назначение. Предоставляется для того, чтобы вызывающие объекты могли получить определение роли `$expand` одновременно с получением назначения роли. roleDefinition.Id будет автоматически развернут. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|

## <a name="json-representation"></a>Представление в формате JSON
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

