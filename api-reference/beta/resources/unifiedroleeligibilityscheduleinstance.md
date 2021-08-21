---
title: тип ресурса unifiedRoleEligibilityScheduleInstance
description: Представляет экземпляр расписания для соответствующих операций назначения ролей через Azure AD управление привилегированными пользователями.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bf4e689e4379f34a0196506bcdecafa991b6d38c
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453788"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>тип ресурса unifiedRoleEligibilityScheduleInstance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет экземпляр для назначения подходящих ролей через Azure AD управление привилегированными пользователями. **УнифицированнаяRoleEligibilityScheduleInstance** создается [унифицированнойRoleEligibilitySchedule](unifiedroleeligibilityschedule.md) и представляет фактическое назначение подходящих ролей, созданное управление привилегированными пользователями. Этот ресурс поддерживает операции List и Get для просмотра текущих и будущих назначений.

Наследует [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список unifiedRoleEligibilityScheduleInstances](../api/unifiedroleeligibilityscheduleinstance-list.md)|[коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Получите список объектов [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) и их свойств.|
|[Get unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilityScheduleInstance.](../resources/unifiedroleeligibilityscheduleinstance.md)|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Получите список объектов [unifiedRoleEligibilityInstance](../resources/unifiedroleeligibilityscheduleinstance.md) и их свойств, предоставленных конкретному пользователю.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область для определенных объектов каталогов, например административных единиц. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|endDateTime|DateTimeOffset|Время истечения срока действия функции RoleEligibilityScheduleInstance.|
|id|String|Уникальный идентификатор для roleEligibilityScheduleInstance. Key, not nullable, Read-only.Inherited from [unifiedRoleScheduleInstanceBase.](../resources/unifiedrolescheduleinstancebase.md)|
|memberType|String|Тип членства назначения. Это может быть `Inherited` или `Direct` , или `Group` .|
|principalId|String|Идентификатор основного, которому предоставляется назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|roleDefinitionId|String|Идентификатор унифицированногоRoleDefinition для назначения. Только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).<br> Поддерживает `$filter` (`eq`).|
|roleEligibilityScheduleId|String|Идентификатор родительской ролиEligibilitySchedule для этого экземпляра.|
|startDateTime|DateTimeOffset|Время запуска roleEligibilityScheduleInstance.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели смогут получать объект каталога с помощью одновременно с получением `$expand` соответствующих назначений ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылаясь на доверенного, который получает право назначения роли через запрос. При условии, что звонители могут получать основное использование одновременно с получением `$expand` соответствующих назначений ролей. Только для чтения. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение ролей, используя одновременно с получением `$expand` соответствующих назначений ролей. roleDefinition.Id будет автоматически расширена. Унаследованный от [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleInstance",
  "baseType": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleInstance",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "memberType": "String",
  "roleEligibilityScheduleId": "String"
}
```

