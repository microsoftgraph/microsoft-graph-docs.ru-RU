---
title: тип ресурса unifiedRoleEligibilitySchedule
description: Представляет расписание операций назначения ролей с помощью Azure AD управление привилегированными пользователями.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1593e819b3c57ee24dae0480aadcb7f532d2fbf4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299725"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>тип ресурса unifiedRoleEligibilitySchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет расписание назначения подходящих ролей через Azure AD управление привилегированными пользователями. A `roleEligibilitySchedule` создается `roleEligibilityScheduleRequest` и используется для мгновенного создания `roleEligibilityInstance` . Мы поддерживаем список и получаем операции для получения расписания для просмотра текущих и будущих подходящих назначений.

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
|appScopeId|Строка|Id конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте "/" для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdDateTime|DateTimeOffset|Время создания расписания. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|Строка|ID roleEligibilityScheduleRequest, создавав это расписание. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|Строка|Id объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|Строка|Уникальный идентификатор для unifiedRoleEligibilitySchedule. Key, not nullable, Read-only. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|Строка|Тип членства в правом назначении. Это может быть `Inherited` или `Direct` , или `Group` .|
|modifiedDateTime|DateTimeOffset|При последнем обновлении расписания. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|Строка| Объект объекта, которому предоставляется право на назначение. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinitionId|Строка|ID унифицированногоRoleDefinition, для который требуется назначение. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|Объект расписания запроса на назначение ролей.|
|status|String|Состояние `roleEligibilitySchedule` для . Он может включать сообщения, связанные с `Provisioned` состоянием, как , и `Revoked` `Pending Provisioning` `Pending Approval` . Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Будет обесценить. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения, которое может быть присвоено. При условии, что вызыватели смогут получать объект каталога с помощью одновременно с получением `$expand` назначения ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на доверенного, который получает право назначения роли через запрос. При условии, что звонители могут получать основное использование одновременно с `$expand` получением назначения подходящих ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition, для которого имеется право назначения. При условии, что вызыватели могут получать определение ролей, используя одновременно с получением назначения ролей, которое `$expand` имеет право. roleDefinition.Id будет автоматически расширена. Унаследованный от [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="json-representation"></a>Представление в формате JSON
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

