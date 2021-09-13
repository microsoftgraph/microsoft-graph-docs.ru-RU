---
title: тип ресурса unifiedRoleScheduleBase
description: Базовое свойство унифицированных расписаний ролей, объединяющих унифицированные графики назначения ролей и унифицированные графики прав на роль
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b65d7d41feccfa8336ea347936433da2437f0f6b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59050882"
---
# <a name="unifiedroleschedulebase-resource-type"></a>тип ресурса unifiedRoleScheduleBase

Пространство имен: microsoft.graph

Базовое свойство унифицированных расписаний ролей, объединяющих унифицированные графики назначения ролей и унифицированные графики прав на роль

## <a name="properties"></a>Свойства

| Свойство         | Тип           | Описание               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | String         | Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область действия определенными объектами каталогов, например административными единицами или всеми пользователями. |
| createdDateTime  | DateTimeOffset | Время создания расписания. |
| createdUsing     | String         | Идентификатор ролиAssignmentScheduleRequest, создав этот график. |
| directoryScopeId | String         | Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. |
| id               | String         | Уникальный идентификатор для unifiedRoleAssignmentSchedule. Key, not nullable, Read-only. |
| modifiedDateTime | DateTimeOffset | При последнем обновлении расписания. |
| principalId      | String         | Идентификатор основного, которому предоставляется назначение. Поддерживает `$filter` (`eq`). |
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
