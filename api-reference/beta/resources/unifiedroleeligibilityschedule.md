---
title: тип ресурса unifiedRoleEligibilitySchedule
description: Представляет расписание операций назначения ролей с помощью Azure AD управление привилегированными пользователями.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f446c5bed547fc4697c535b57f271e998c8ebfab
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510585"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>тип ресурса unifiedRoleEligibilitySchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание назначения подходящих ролей через Azure AD управление привилегированными пользователями. **УнифицированнаяRoleEligibilitySchedule** создается с помощью [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) и используется для мгновенного создания единой [системыRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md). Этот ресурс поддерживает операции Список и Получение для получения расписания для просмотра текущих и будущих подходящих назначений.

Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список унифицированныхRoleEligibilitySchedules](../api/unifiedroleeligibilityschedule-list.md)|[коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получите список объектов [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) и их свойств.|
|[Get unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) .|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[коллекция unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Получите список объектов [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId** , чтобы ограничить область для определенных объектов каталогов, например административных единиц. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdDateTime|DateTimeOffset|Время создания расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|Строка|Идентификатор ролиEligibilityScheduleRequest, создавав этот график. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|id|String|Уникальный идентификатор для unifiedRoleEligibilitySchedule. Key, not nullable, Read-only. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|memberType|Строка|Тип членства в правом назначении. Это может быть или `Inherited`, `Direct`или `Group`.|
|modifiedDateTime|DateTimeOffset|При последнем обновлении расписания. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|Строка| Идентификатор доверителем, которому предоставляется право на назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|
|roleDefinitionId|Строка|Идентификатор унифицированногоRoleDefinition для назначения. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение ролей.|
|status|String|Состояние для `roleEligibilitySchedule`. Он может включать сообщения, связанные с состоянием, как `Provisioned`, `Revoked`и `Pending Provisioning``Pending Approval`. Наследуется [от unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Поддерживает `$filter` (`eq`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Будет обесценить. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения, которое может быть присвоено. При условии, что вызыватели смогут получать объект каталога `$expand` с помощью одновременно с получением назначения ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на доверенного, который получает право назначения роли через запрос. При условии, что звонители `$expand` могут получать основное использование одновременно с получением назначения подходящих ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition, для которого имеется право назначения. При условии, что вызыватели могут получать определение ролей `$expand` , используя одновременно с получением назначения ролей, которое имеет право. roleDefinition.Id будет автоматически расширена. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

