---
title: тип ресурса unifiedRoleAssignment
description: Назначение ролей — это связь между определением роли и главным в определенной области для предоставления доступа.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fd6323fa0eb99f440551916cbc535fa64a359275
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148533"
---
# <a name="unifiedroleassignment-resource-type"></a>тип ресурса unifiedRoleAssignment

Пространство имен: microsoft.graph

Назначение ролей используется для предоставления доступа к ресурсам. Оно представляет определение роли, назначенное директору (например, пользователю или группе, назначаемой для ролей) в определенной области.

Наследует от [объекта](entity.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Список unifiedRoleAssignments](../api/rbacapplication-list-roleassignments.md)|[коллекция unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Получите список объектов [unifiedRoleAssignment](../resources/unifiedroleassignment.md) и их свойств.|
|[Создание unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Создайте новый [объект unifiedRoleAssignment.](../resources/unifiedroleassignment.md)|
|[Get unifiedRoleAssignment](../api/unifiedroleassignment-get.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)|
|[Удаление unifiedRoleAssignment](../api/unifiedroleassignment-delete.md)|Нет|Удаляет объект [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для назначения ролей. Key, not nullable, Read-only. Наследуется от [сущности](entity.md).|
|roleDefinitionId|String| Идентификатор определения роли для назначения. Только для чтения. Поддерживает $filter ( `eq` , `in` ).|
|principalId|String| Идентификатор основного, которому предоставляется назначение. Поддерживает $filter ( `eq` , `in` ).|
|directoryScopeId|String|Идентификатор объекта каталога, представляющего область назначения.  Требуется либо это свойство, либо **appScopeId.** Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ. Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям. Используйте `/` для области для клиента. Используйте **appScopeId,** чтобы ограничить область только приложения. Поддерживает $filter ( `eq` , `in` ).|
|appScopeId|String|Идентификатор области, определенной для приложения, когда область назначения является конкретной для приложения.  Требуется либо это **свойство, либо directoryScopeId.** Области приложений — это области, которые определяются и понимаются только этим приложением. Используйте `/` для областей приложений для всех клиентов. Используйте **directoryScopeId,** чтобы ограничить область для определенных объектов каталогов, например административных единиц. Поддерживает $filter ( `eq` , `in` ).|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|основной|[directoryObject](directoryobject.md)| Ссылки на назначенного директора. Только для чтения. Поддерживает `$expand`.|
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|РольDefinition для назначения.  Поддерживает `$expand`. roleDefinition.Id будет автоматически расширена.
|directoryScope|[directoryObject](directoryobject.md)|Объект каталога, который является областью назначения. Только для чтения. Поддерживает `$expand`.|
|appScope|[appScope](appscope.md)|Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной. Объект containment. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "String (identifier)",
  "appScopeId": "String",
  "condition": "String",
  "directoryScopeId": "String",
  "principalId": "String",
  "roleDefinitionId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
