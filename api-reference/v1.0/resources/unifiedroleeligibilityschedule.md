---
title: Тип ресурса unifiedRoleEligibilitySchedule
description: Представляет расписание для получения прав на роль в клиенте.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3bf5929c146cf054022ef33b2be73db323a0f13c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134432"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>Тип ресурса unifiedRoleEligibilitySchedule

Пространство имен: microsoft.graph

Представляет расписание для соответствия роли в клиенте и используется для создания экземпляра [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md).


Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleEligibilitySchedule](../api/rbacapplication-list-roleeligibilityschedules.md)|[Коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получение расписаний для операций с правом на участие в роли.|
|[Получение unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получение расписания для операции соответствия роли.|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[Коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получение расписаний для прав на роль, для которых вошед в систему пользователь является субъектом.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, относяшейся к приложению, если доступ к роли определяется приложением. Область действия роли определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|createdDateTime|DateTimeOffset|При создании расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|String|Идентификатор объекта, с помощью которого было создано это расписание. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область допустимости роли. Область действия роли определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|id|String|Уникальный идентификатор объекта расписания. Наследуется от [сущности](../resources/entity.md). Поддерживает `$filter` (`eq`).|
|memberType|String|Способ наследования допустимости роли. Это может быть либо `Inherited`, `Direct`, либо `Group`. Это также может означать, может ли **объект unifiedRoleEligibilitySchedule** управляться вызывающим объектом. Поддерживает `$filter` (`eq`, `ne`).|
|modifiedDateTime|DateTimeOffset|Время последнего изменения расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|String|Идентификатор субъекта, который имеет право на роль. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Поддерживает `$filter` (`eq`, `ne`).|
|roleDefinitionId|String|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , для которого имеет право субъект. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Период допустимости роли.|
|status|String|Состояние запроса на участие в роли. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Возможные значения: `Canceled`, , `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`и `Revoked``ScheduleCreated`. Значение null не допускается. Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если права на роль относятся к приложению. Допускается значение null. Поддерживает `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью действия роли. Только для чтения. Поддерживает `$expand`.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который имеет право на роль в запросе. Поддерживает `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об объекте roleDefinition, на который ссылаются через **свойство roleDefinitionId** . Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilitySchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilitySchedule",
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
  "memberType": "String"
}
```

