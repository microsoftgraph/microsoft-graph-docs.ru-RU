---
title: Тип ресурса unifiedRoleEligibilityScheduleInstance
description: Представляет экземпляр расписания для допустимых операций назначения ролей через Azure AD управление привилегированными пользователями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 14345412d06d1a36210f1cb2c5cfd5c2cf18c5a1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439368"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>Тип ресурса unifiedRoleEligibilityScheduleInstance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет экземпляр для получения прав на роль в клиенте.

Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleEligibilityScheduleInstance](../api/rbacapplication-list-roleeligibilityscheduleinstances.md)|[Коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|GGet экземпляров прав на роль.|
|[Получение unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Получение экземпляра права на роль.|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[Коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Получение экземпляров допустимых ролей для вызывающего субъекта.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|endDateTime|DateTimeOffset|Время истечения срока действия roleEligibilityScheduleInstance.|
|id|String|Уникальный идентификатор для roleEligibilityScheduleInstance. Key, not nullable, Read-only.Inherited from [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|memberType|Строка|Тип членства назначения. Это может быть либо `Inherited`, `Direct`, либо `Group`.|
|principalId|String|Идентификатор субъекта, которому предоставляется назначение. Может быть группой или пользователем. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|roleDefinitionId|String|Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).<br> Поддерживает `$filter` (`eq`).|
|roleEligibilityScheduleId|Строка|Идентификатор родительской ролиEligibilitySchedule для этого экземпляра.|
|startDateTime|DateTimeOffset|Время запуска roleEligibilityScheduleInstance.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если область назначения предназначена для конкретного приложения. Сущность containment. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на объект каталога, который является областью назначения. Предоставляется таким образом, чтобы вызывающие объекты могли получать объект каталога `$expand` одновременно с получением соответствующих назначений ролей. Только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$expand`.|
|Основной|[directoryObject](../resources/directoryobject.md)|Свойство, ссылающееся на участника, который получает допустимое назначение роли через запрос. Предоставляется для того, чтобы вызывающие абоненты `$expand` могли получить субъект, используя одновременно с получением допустимых назначений ролей. Только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Свойство, указывающее roleDefinition, для которых предназначено назначение. Предоставляется, чтобы вызывающие объекты могли получить определение роли `$expand` одновременно с получением соответствующих назначений ролей. roleDefinition.Id будет автоматически развернут. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$expand`.|

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

