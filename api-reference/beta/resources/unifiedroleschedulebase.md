---
title: тип ресурса unifiedRoleScheduleBase
description: Базовое свойство унифицированных расписаний ролей, объединяющих унифицированные графики назначения ролей и унифицированные графики прав на роль
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 86338096720a54322a418a98a88c8b4edc26297ae20583064a2a2aaf434e976d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122112"
---
# <a name="unifiedroleschedulebase-resource-type"></a>тип ресурса unifiedRoleScheduleBase

Пространство имен: microsoft.graph

Базовое свойство унифицированных расписаний ролей, объединяющих унифицированные графики назначения ролей и унифицированные графики прав на роль

## <a name="properties"></a>Свойства

| Свойство         | Тип           | Описание               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | Строка         | Id конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте "/" для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением. |
| createdDateTime  | DateTimeOffset | Время создания расписания. |
| createdUsing     | Строка         | ID ролиAssignmentScheduleRequest, создав этот график. |
| directoryScopeId | String         | Id объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением. |
| id               | String         | Уникальный идентификатор для unifiedRoleAssignmentSchedule. Key, not nullable, Read-only. |
| modifiedDateTime | DateTimeOffset | При последнем обновлении расписания. |
| principalId      | Строка         | Объект объекта, которому предоставляется назначение. |
| roleDefinitionId | Строка         | ID унифицированногоRoleDefinition для назначения. Только для чтения. |
| status           | String         | Состояние `roleAssignmentSchedule` для . Он может включать сообщения, связанные с `Provisioned` состоянием, как , и `Revoked` `Pending Provisioning` `Pending Approval` . |

## <a name="relationships"></a>Связи

| Связь   | Тип                                                                               | Описание               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | Будет обесценить. |
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
