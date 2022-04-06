---
title: тип ресурса unifiedRoleScheduleBase
description: Базовое свойство унифицированных расписаний ролей, объединяющих унифицированные графики назначения ролей и унифицированные графики прав на роль
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 19b7c93dfcec24db531e7ae61924dda3e84695d3
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510150"
---
# <a name="unifiedroleschedulebase-resource-type"></a>тип ресурса unifiedRoleScheduleBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовое свойство унифицированных расписаний ролей, объединяющих унифицированные графики назначения ролей и унифицированные графики прав на роль

## <a name="properties"></a>Свойства

| Свойство         | Тип           | Описание               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | Строка         | Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId** , чтобы ограничить область действия определенными объектами каталогов, например административными единицами или всеми пользователями. |
| createdDateTime  | DateTimeOffset | Время создания расписания. |
| createdUsing     | Строка         | Идентификатор ролиAssignmentScheduleRequest, создав этот график. |
| directoryScopeId | Строка         | Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. |
| id               | String         | Уникальный идентификатор для unifiedRoleAssignmentSchedule. Key, not nullable, Read-only. |
| modifiedDateTime | DateTimeOffset | При последнем обновлении расписания. |
| principalId      | Строка         | Идентификатор основного, которому предоставляется назначение. Поддерживает `$filter` (`eq`). |
| roleDefinitionId | Строка         | Идентификатор унифицированногоRoleDefinition для назначения. Только для чтения. Поддерживает `$filter` (`eq`). |
| status           | String         | Состояние для `roleAssignmentSchedule`. Он может включать сообщения, связанные с состоянием, как `Provisioned`, `Revoked`и `Pending Provisioning``Pending Approval`. Поддерживает `$filter` (`eq`).  |

## <a name="relationships"></a>Связи

| Связь   | Тип                                                                               | Описание               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance (Deprecated) | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | Устарело. |
| appScope       | [appScope](../resources/appscope.md)                                               | Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога `$expand` с помощью одновременно с назначением ролей. Только для чтения. |
| основной      | [directoryObject](../resources/directoryobject.md)                                 | Свойство, ссылаясь на главного, получаюного назначение ролей через запрос. При условии, что звонители могут получать основное использование `$expand` одновременно с назначением ролей. Только для чтения. |
| roleDefinition | [unifiedRoleDefinition](../resources/unifiedroledefinition.md)                     | Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли `$expand` , используя одновременно с назначением роли. roleDefinition.Id будет автоматически расширена. |

## <a name="json-representation"></a>Представление JSON

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
