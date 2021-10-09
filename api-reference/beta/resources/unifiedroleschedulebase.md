---
title: тип ресурса unifiedRoleScheduleBase
description: Базовое свойство унифицированных расписаний ролей, объединяющих унифицированные графики назначения ролей и унифицированные графики прав на роль
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e93caa68371527a06d18a92249ed285af1fb6e19
ms.sourcegitcommit: 11be55b40804b07f4c422f09f601afa97c7d31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2021
ms.locfileid: "60256545"
---
# <a name="unifiedroleschedulebase-resource-type"></a>тип ресурса unifiedRoleScheduleBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовое свойство унифицированных расписаний ролей, объединяющих унифицированные графики назначения ролей и унифицированные графики прав на роль

## <a name="properties"></a>Свойства

| Свойство         | Тип           | Описание               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | Строка         | Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область действия определенными объектами каталогов, например административными единицами или всеми пользователями. |
| createdDateTime  | DateTimeOffset | Время создания расписания. |
| createdUsing     | Строка         | Идентификатор ролиAssignmentScheduleRequest, создав этот график. |
| directoryScopeId | String         | Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. |
| id               | Строка         | Уникальный идентификатор для unifiedRoleAssignmentSchedule. Key, not nullable, Read-only. |
| modifiedDateTime | DateTimeOffset | При последнем обновлении расписания. |
| principalId      | Строка         | Идентификатор основного, которому предоставляется назначение. Поддерживает `$filter` (`eq`). |
| roleDefinitionId | String         | Идентификатор унифицированногоRoleDefinition для назначения. Только для чтения. Поддерживает `$filter` (`eq`). |
| status           | String         | Состояние `roleAssignmentSchedule` для . Он может включать сообщения, связанные с `Provisioned` состоянием, как , и `Revoked` `Pending Provisioning` `Pending Approval` . Поддерживает `$filter` (`eq`).  |

## <a name="relationships"></a>Связи

| Связь   | Тип                                                                               | Описание               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance (Deprecated) | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | Устарело. |
| appScope       | [appScope](../resources/appscope.md)                                               | Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | Свойство, ссылаясь на объект каталога, который является областью назначения. При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей. Только для чтения. |
| основной      | [directoryObject](../resources/directoryobject.md)                                 | Свойство, ссылаясь на главного, получаюного назначение ролей через запрос. При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей. Только для чтения. |
| roleDefinition | [unifiedRoleDefinition](../resources/unifiedroledefinition.md)                     | Свойство, указывающее рольDefinition для назначения. При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли. roleDefinition.Id будет автоматически расширена. |

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
