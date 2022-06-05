---
title: Тип ресурса unifiedRoleScheduleBase
description: Шаблон, предоставляющий свойства и связи, используемые в типах ресурсов unifiedRoleAssignmentSchedule и unifiedRoleEligibilitySchedule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e422b4b30da252c028003abd35134ea1c06874e
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898338"
---
# <a name="unifiedroleschedulebase-resource-type"></a>Тип ресурса unifiedRoleScheduleBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Шаблон, предоставляющий свойства и связи, используемые в [типах ресурсов unifiedRoleAssignmentSchedule](unifiedroleassignmentschedule.md) и [unifiedRoleEligibilitySchedule](unifiedroleeligibilityschedule.md) .


Наследует [от сущности](../resources/entity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, относяшейся к конкретному приложению, если назначение или право на доступ относятся к приложению. Область назначения или права на участие определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами.|
|createdDateTime|DateTimeOffset|При создании расписания.|
|createdUsing|Строка|Идентификатор объекта, с помощью которого было создано это расписание.|
|directoryScopeId|Строка|Идентификатор объекта каталога, представляющего область назначения или допустимости. Область назначения или права на участие определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением.|
|id|Строка|Уникальный идентификатор объекта расписания. Наследуется от [сущности](../resources/entity.md).|
|modifiedDateTime|DateTimeOffset|Время последнего изменения расписания.|
|principalId|Строка|Идентификатор субъекта, которым было предоставлено назначение роли или право на участие.|
|roleDefinitionId|Строка|Идентификатор объекта [unifiedRoleDefinition](unifiedroledefinition.md) , назначаемого субъекту или доступного субъекту.|
|status|String|Состояние назначения роли или запроса на приемлемость.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями об области приложения, если доступ к роли или назначение относятся к приложению. Допускается значение null.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью действия или назначения роли. Только для чтения.|
|Основной|[directoryObject](../resources/directoryobject.md)|Субъект, который получает назначение роли или может получить роль с помощью запроса.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Подробные сведения об объекте roleDefinition, на который ссылаются через **свойство roleDefinitionId** .|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String"
}
```