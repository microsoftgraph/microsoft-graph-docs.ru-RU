---
title: тип ресурса unifiedRoleScheduleInstanceBase
description: Базовое свойство экземпляра единого расписания ролей, объединяющего экземпляр расписания унифицированных ролей и экземпляр расписания унифицированных ролей
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 58fa78adf75381e3444d2be492077f7388e9ba9b
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510627"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>тип ресурса unifiedRoleScheduleInstanceBase

Пространство имен: microsoft.graph

Базовое свойство экземпляра единого расписания ролей, объединяющего экземпляры расписания назначения ролей и экземпляры расписания унифицированных ролей.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appScopeId|Строка|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId** , чтобы ограничить область для определенных объектов каталогов, например административных единиц. |
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения. Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. |
|id|String|Уникальный идентификатор для unifiedRoleAssignmentScheduleInstance. Key, not nullable, Read-only.|
|principalId|String|Идентификатор основного, которому предоставляется назначение. Может быть группой или пользователем. |
|roleDefinitionId|Строка|Идентификатор унифицированногоRoleDefinition для назначения. Только для чтения. <br> Поддерживает `$filter` (`eq`).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. |
|directoryScope|[directoryObject](../resources/directoryobject.md)|Объект каталога, который является областью назначения. Позволяет выполнять ирисовку объекта каталога `$expand` одновременно с получением назначения ролей. Только для чтения.|
|основной|[directoryObject](../resources/directoryobject.md)|Основной, получающе назначение ролей через запрос. Позволяет выполнять ирисовку `$expand` основного, используя одновременно с получением назначения ролей. Только для чтения.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|РольDefinition для назначения. Включает получение определения роли `$expand` одновременно с получением назначения роли. Автоматически roleDefinition.Id расширения.|

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
