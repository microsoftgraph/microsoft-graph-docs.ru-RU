---
title: Тип ресурса unifiedRoleEligibilityScheduleInstance
description: Представляет экземпляр для получения прав на роль в клиенте.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 91ed173a26262fd6285df4d60518a80aded68b60
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134472"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>Тип ресурса unifiedRoleEligibilityScheduleInstance

Пространство имен: microsoft.graph

Представляет экземпляр для получения прав на роль в клиенте.

Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов unifiedRoleEligibilityScheduleInstance](../api/rbacapplication-list-roleeligibilityscheduleinstances.md)|[Коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Получение экземпляров прав на роль.|
|[Получение unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Получение экземпляра права на роль.|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[Коллекция unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Получение экземпляров допустимых ролей для вызывающего субъекта.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|String|Идентификатор области, относяшейся к приложению, если доступ к роли определяется приложением. Область действия роли определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область допустимости роли. Область действия роли определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). `$filter` Поддерживает (`eq`и `ne`по `null` значениям).|
|endDateTime|DateTimeOffset|Дата окончания экземпляра расписания.|
|id|String|Уникальный идентификатор объекта расписания. Наследуется от [сущности](../resources/entity.md).|
|memberType|String|Способ наследования допустимости роли. Это может быть либо `Inherited`, `Direct`, либо `Group`. Это также может означать, может ли **объект unifiedRoleEligibilitySchedule** управляться вызывающим объектом. Поддерживает `$filter` (`eq`, `ne`).|
|principalId|String|Идентификатор субъекта, который имеет право на роль. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$filter` (`eq`, `ne`). |
|roleDefinitionId|String|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , для которого имеет право субъект. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$filter` (`eq`, `ne`).|
|roleEligibilityScheduleId|String|Идентификатор объекта **unifiedRoleEligibilitySchedule** , из которого был создан этот экземпляр.|
|startDateTime|DateTimeOffset|При запуске этого экземпляра.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если права на роль относятся к приложению. Допускается значение null. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью действия роли. Только для чтения. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$expand`.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает право на роль в запросе. Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об объекте roleDefinition, на который ссылаются через **свойство roleDefinitionId** . Наследуется [от unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Поддерживает `$expand`.|

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

