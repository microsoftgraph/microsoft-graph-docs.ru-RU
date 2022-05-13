---
title: Тип ресурса privilegedRoleAssignment
description: 'Представляет назначение привилегированной роли для определенного пользователя. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 62ecfd138aa4a0d3d7649f57ef7750a06381a557
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397503"
---
# <a name="privilegedroleassignment-resource-type-deprecated"></a>Тип ресурса privilegedRoleAssignment (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Представляет назначение привилегированной роли для определенного пользователя. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление коллекции privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)|Получение коллекции объектов privilegedRoleAssignment.|
|[Получение privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Чтение свойств и связей объекта privilegedRoleAssignment.|
|[Создание задания](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Создайте новое назначение, выполнив публикацию в коллекции назначений.|
|[Удаление](../api/privilegedroleassignment-delete.md) | Нет |Удаление объекта privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Выполнение назначения ролей как бессрочного.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Выполнение назначения ролей как соответствующего требованиям.|
|[my](../api/privilegedroleassignment-my.md)|Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)|Получение назначений привилегированных ролей текущего пользователя.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|Дата и время в формате UTC, по истечении которого истекает срок действия временного назначения привилегированной роли. Для назначения постоянной роли значение равно NULL.|
|id|string| Уникальный идентификатор для назначения привилегированной роли. Только для чтения. Он имеет формат "userId_roleId", где userId — это строка GUID для идентификатора Azure AD пользователя, а roleId — строка GUID для идентификатора роли администратора Azure.|
|isElevated|логический|**Значение true** , если назначение роли активировано. **Значение false** , если назначение роли деактивировано.|
|resultMessage|string|Результирующее сообщение, задайте службой.|
|roleId|string|Идентификатор роли. В строковом формате GUID.|
|userId|строка|Идентификатор пользователя. В строковом формате GUID.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Только для чтения. Допускается значение null. Сведения о связанной роли.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


