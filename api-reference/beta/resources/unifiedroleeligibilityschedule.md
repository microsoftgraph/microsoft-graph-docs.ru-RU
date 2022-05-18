---
title: Тип ресурса unifiedRoleEligibilitySchedule
description: Представляет расписание для допустимых операций назначения ролей через Azure AD управление привилегированными пользователями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f89a81fcf64cffa8875f58ead56a95550b655a95
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461473"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>Тип ресурса unifiedRoleEligibilitySchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание назначения подходящей роли через Azure AD управление привилегированными пользователями. **UnifiedRoleEligibilitySchedule** создается с помощью [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) и используется для создания экземпляра [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md). Этот ресурс поддерживает операции списка и получения для получения расписания для просмотра текущих и будущих подходящих назначений.

Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleEligibilitySchedule](../api/rbacapplication-list-roleeligibilityschedules.md)|[Коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получение списка объектов [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) и их свойств.|
|[Получение unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Чтение свойств и связей объекта [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) .|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[Коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получение списка объектов [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdDateTime|DateTimeOffset|Время создания расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|Строка|Идентификатор roleEligibilityScheduleRequest, создавшего это расписание. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|id|String|Уникальный идентификатор объекта unifiedRoleEligibilitySchedule. Ключ, не допускающий значения NULL, только для чтения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|memberType|Строка|Тип членства допустимого назначения. Это может быть либо `Inherited`, `Direct`, либо `Group`.|
|modifiedDateTime|DateTimeOffset|Время последнего обновления расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|String| Идентификатор субъекта, которому предоставляется допустимое назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|
|roleDefinitionId|Строка|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение подходящей роли.|
|status|String|Состояние для .`roleEligibilitySchedule` Он может включать сообщения, связанные с состоянием, такие `Provisioned`как , `Revoked`, и `Pending Provisioning``Pending Approval`. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Будет нерекомендуемым. Наследуется от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
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

