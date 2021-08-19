---
title: тип ресурса unifiedRoleScheduleInstanceBase
description: Базовое свойство экземпляра единого расписания ролей, объединяющего экземпляр расписания унифицированных ролей и экземпляр расписания унифицированных ролей
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4f22af61c513f8cc559948fb5519af5ac903d1d7c4ed650d2d11c6f5bf665282
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238946"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>тип ресурса unifiedRoleScheduleInstanceBase

Пространство имен: microsoft.graph

"Базовое свойство экземпляра единого расписания ролей, объединяющего экземпляр расписания унифицированных ролей и экземпляр расписания унифицированных ролей

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Id конкретной области приложения, когда область назначения является конкретной. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте "/" для области для клиента. Области приложений — это области, которые определяются и понимаются только этим приложением.|
|directoryScopeId|String|Id объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Области приложений — это области, которые определяются и понимаются только этим приложением.|
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

## <a name="json-representation"></a>Представление JSON
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
