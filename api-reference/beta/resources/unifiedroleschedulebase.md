---
title: Тип ресурса unifiedRoleScheduleBase
description: Базовое свойство унифицированных расписаний ролей, объединяющее унифицированные расписания назначения ролей и унифицированные расписания соответствия роли
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dbe8b597286bacd9c6f8d0a7dc17cf82296fadb9
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398835"
---
# <a name="unifiedroleschedulebase-resource-type"></a>Тип ресурса unifiedRoleScheduleBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовое свойство унифицированных расписаний ролей, объединяющее унифицированные расписания назначения ролей и унифицированные расписания соответствия роли

## <a name="properties"></a>Свойства

| Свойство         | Тип           | Описание               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | String         | Идентификатор области, относяшейся к приложению, если область назначения предназначена для конкретного приложения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области приложения — это области, которые определяются и распознаются только этим приложением. Используется `/` для областей приложений на уровне клиента. Используйте **directoryScopeId** , чтобы ограничить область определенными объектами каталога, например административными единицами или всеми пользователями. |
| createdDateTime  | DateTimeOffset | Время создания расписания. |
| createdUsing     | String         | Идентификатор ролиAssignmentScheduleRequest, создавшего это расписание. |
| directoryScopeId | String         | Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым участнику был предоставлен доступ. Области каталога — это общие области, хранящиеся в каталоге, которые распознаются несколькими приложениями. Используется `/` для области на уровне клиента. Используйте **appScopeId** , чтобы ограничить область только приложением. |
| id               | String         | Уникальный идентификатор объекта unifiedRoleAssignmentSchedule. Ключ, не допускающий значения NULL, только для чтения. |
| modifiedDateTime | DateTimeOffset | Время последнего обновления расписания. |
| principalId      | String         | Идентификатор субъекта, которому предоставляется назначение. Поддерживает `$filter` (`eq`). |
| roleDefinitionId | String         | Идентификатор объекта unifiedRoleDefinition, для который предназначено назначение. Только для чтения. Поддерживает `$filter` (`eq`). |
| status           | String         | Состояние для .`roleAssignmentSchedule` Он может включать сообщения, связанные с состоянием, такие `Provisioned`как , `Revoked`, и `Pending Provisioning``Pending Approval`. Поддерживает `$filter` (`eq`).  |

## <a name="relationships"></a>Связи

| Связь   | Тип                                                                               | Описание               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance (не рекомендуется) | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | Устарело. |
| appScope       | [appScope](../resources/appscope.md)                                               | Свойство только для чтения с подробными сведениями об области приложения, если область назначения предназначена для конкретного приложения. Сущность containment. |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | Свойство, ссылающееся на объект каталога, который является областью назначения. Предоставляется для того, чтобы вызывающие объекты могли получить объект каталога `$expand` , используя одновременно с получением назначения роли. Только для чтения. |
| Основной      | [directoryObject](../resources/directoryobject.md)                                 | Свойство, ссылающееся на субъект, который получает назначение роли через запрос. Предоставляется для того, чтобы вызывающие объекты `$expand` могли получить субъект одновременно с получением назначения роли. Только для чтения. |
| roleDefinition | [unifiedRoleDefinition](../resources/unifiedroledefinition.md)                     | Свойство, указывающее roleDefinition, для которых предназначено назначение. Предоставляется для того, чтобы вызывающие объекты могли получить определение роли `$expand` одновременно с получением назначения роли. roleDefinition.Id будет автоматически развернут. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->

```json
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
