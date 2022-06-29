---
title: Тип ресурса unifiedRoleEligibilitySchedule
description: Представляет расписание для допустимых операций назначения ролей через Azure AD управление привилегированными пользователями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e581e021df25547b276609d4075c162fcc5fed3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439923"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>Тип ресурса unifiedRoleEligibilitySchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|appScopeId|String|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|createdDateTime|DateTimeOffset|Время создания расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|String|Идентификатор roleEligibilityScheduleRequest, создавшего это расписание. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|id|String|Уникальный идентификатор объекта unifiedRoleEligibilitySchedule. Ключ, не допускающий значения NULL, только для чтения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Поддерживает `$filter` (`eq`).|
|memberType|String|Тип членства допустимого назначения. Это может быть либо `Inherited`, `Direct`, либо `Group`. Поддерживает `$filter` (`eq`).|
|modifiedDateTime|DateTimeOffset|Время последнего обновления расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|String| Идентификатор субъекта, которому предоставляется допустимое назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|
|roleDefinitionId|String|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение подходящей роли.|
|status|String|Состояние для .`roleEligibilitySchedule` Он может включать сообщения, связанные с состоянием, такие `Provisioned`как , `Revoked`, и `Pending Provisioning``Pending Approval`. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если область назначения предназначена для конкретного приложения. Сущность containment. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на объект каталога, который является областью допустимого назначения. Предоставляется, чтобы вызывающие объекты могли получить объект каталога `$expand` одновременно с получением допустимого назначения роли. Только для чтения. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|Основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на участника, который получает допустимое назначение роли через запрос. Предоставляется для того, чтобы вызывающие абоненты `$expand` могли получать субъект одновременно с получением допустимого назначения роли. Только для чтения. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее roleDefinition, для которых предназначено допустимое назначение. Предоставляется, чтобы вызывающие объекты могли получить определение роли `$expand` одновременно с получением допустимого назначения роли. roleDefinition.Id будет автоматически развернут. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

