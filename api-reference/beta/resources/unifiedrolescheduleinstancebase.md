---
title: тип ресурса unifiedRoleScheduleInstanceBase
description: Базовое свойство экземпляра единого расписания ролей, объединяющего экземпляр расписания унифицированных ролей и экземпляр расписания унифицированных ролей
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c681467dc77bff716c24fbb273640a3e1d7df689
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299510"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>тип ресурса unifiedRoleScheduleInstanceBase

Пространство имен: microsoft.graph

"Базовое свойство экземпляра единого расписания ролей, объединяющего экземпляр расписания унифицированных ролей и экземпляр расписания унифицированных ролей

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Id конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте "/" для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением.|
|directoryScopeId|Строка|Id объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением.|
|id|Строка|Уникальный идентификатор для unifiedRoleAssignmentScheduleInstance. Key, not nullable, Read-only.|
|principalId|Строка|Объект объекта, которому предоставляется назначение.|
|roleDefinitionId|Строка|ID унифицированногоRoleDefinition для назначения. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. |
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью назначения. Позволяет выполнять ирисовку объекта каталога одновременно с получением `$expand` назначения ролей. Только для чтения.|
|основной|[directoryObject](../resources/directoryobject.md)|Основной, получающе назначение ролей через запрос. Позволяет выполнять ирисовку основного, используя одновременно `$expand` с получением назначения ролей. Только для чтения.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|РольDefinition для назначения. Включает получение определения роли одновременно с получением `$expand` назначения роли. Автоматически roleDefinition.Id расширения.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleInstanceBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String"
}
```
