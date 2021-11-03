---
title: тип ресурса unifiedRoleEligibilitySchedule
description: Представляет расписание операций назначения ролей с помощью Azure AD управление привилегированными пользователями.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e9cf19622cb707688711361b3ef71e405bbaf665
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695246"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>тип ресурса unifiedRoleEligibilitySchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание назначения подходящих ролей через Azure AD управление привилегированными пользователями. **УнифицированнаяRoleEligibilitySchedule** создается [унифицированнойRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) и используется для мгновенного создания единойRoleEligibilityScheduleInstance . [](unifiedroleeligibilityscheduleinstance.md) Этот ресурс поддерживает операции Список и Получение для получения расписания для просмотра текущих и будущих подходящих назначений.

Наследует [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список унифицированныхRoleEligibilitySchedules](../api/unifiedroleeligibilityschedule-list.md)|[коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получите список объектов [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) и их свойств.|
|[Get unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilitySchedule.](../resources/unifiedroleeligibilityschedule.md)|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получите список объектов [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область для определенных объектов каталогов, например административных единиц. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdDateTime|DateTimeOffset|Время создания расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|String|Идентификатор ролиEligibilityScheduleRequest, создавав этот график. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|id|String|Уникальный идентификатор для unifiedRoleEligibilitySchedule. Key, not nullable, Read-only. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|memberType|String|Тип членства в правом назначении. Это может быть `Inherited` или `Direct` , или `Group` .|
|modifiedDateTime|DateTimeOffset|При последнем обновлении расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|String| Идентификатор доверителем, которому предоставляется право на назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|
|roleDefinitionId|String|Идентификатор унифицированногоRoleDefinition для назначения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение ролей.|
|status|String|Состояние `roleEligibilitySchedule` для . Он может включать сообщения, связанные с `Provisioned` состоянием, как , и `Revoked` `Pending Provisioning` `Pending Approval` . Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Будет обесценить. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения, которое может быть присвоено. При условии, что вызыватели смогут получать объект каталога с помощью одновременно с получением `$expand` назначения ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на доверенного, который получает право назначения роли через запрос. При условии, что звонители могут получать основное использование одновременно с `$expand` получением назначения подходящих ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition, для которого имеется право назначения. При условии, что вызыватели могут получать определение ролей, используя одновременно с получением назначения ролей, которое `$expand` имеет право. roleDefinition.Id будет автоматически расширена. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

