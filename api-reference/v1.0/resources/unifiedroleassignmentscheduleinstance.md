---
title: Тип ресурса unifiedRoleAssignmentScheduleInstance
description: Представляет экземпляр для активного назначения ролей в клиенте.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 004a4af4b84712d824787e7d45d7b4f083d9fd6b
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549346"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>Тип ресурса unifiedRoleAssignmentScheduleInstance

Пространство имен: microsoft.graph

Представляет экземпляр для активного назначения ролей в клиенте. Активное назначение может быть выполнено через [назначения PIM](../api/rbacapplication-post-roleassignmentschedulerequests.md) и запросы на активацию или непосредственно через [API назначений ролей](../resources/unifiedroleassignment.md).

Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleAssignmentScheduleInstance](../api/rbacapplication-list-roleassignmentscheduleinstances.md)|[Коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Получение экземпляров активных назначений ролей.|
|[Получение unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-get.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Получение экземпляра активного назначения роли.|
|[filterByCurrentUser](../api/unifiedroleassignmentscheduleinstance-filterbycurrentuser.md)|[Коллекция unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Получение экземпляров активных назначений ролей для вызывающего субъекта.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, относяшейся к конкретному приложению, если назначение предназначено для приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. `$filter` Поддерживает (`eq`и `ne`по `null` значениям). Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|assignmentType|Строка|Тип назначения, которое может быть или `Assigned` `Activated`. Поддерживает `$filter` (`eq`, `ne`).|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. `$filter` Поддерживает (`eq`и `ne`по `null` значениям). Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|endDateTime|DateTimeOffset| Дата окончания экземпляра расписания.|
|id|String|Уникальный идентификатор объекта **unifiedRoleAssignmentScheduleInstance** . Наследуется от [сущности](../resources/entity.md).|
|memberType|Строка|Способ наследования назначений. Это может быть либо `Inherited`, `Direct`, либо `Group`. Это также может означать, может ли **объект unifiedRoleAssignmentSchedule** управляться вызывающим объектом. Поддерживает `$filter` (`eq`, `ne`).|
|principalId|Строка|Идентификатор субъекта, которым было предоставлено назначение роли. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$filter` (`eq`, `ne`). |
|roleAssignmentOriginId|Строка|Идентификатор назначения роли в Azure AD. Поддерживает `$filter` (`eq`, `ne`).|
|roleAssignmentScheduleId|String|Идентификатор объекта **unifiedRoleAssignmentSchedule** , из которого был создан этот экземпляр. Поддерживает `$filter` (`eq`, `ne`).|
|roleDefinitionId|Строка|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , назначаемого субъекту. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$filter` (`eq`, `ne`).|
|startDateTime|DateTimeOffset|При запуске этого экземпляра.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Если запрос от допустимого администратора для активации роли, этот параметр отобразит связанное допустимое назначение для этой активации. В противном случае это .`null` Поддерживает `$expand`.|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если назначение предназначено для приложения. Допускается значение null. Поддерживает `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью назначения. Только для чтения. Поддерживает `$expand`.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает назначение роли через запрос. Поддерживает `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об объекте roleDefinition, на который ссылаются через **свойство roleDefinitionId** . Поддерживает `$expand`.|

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

