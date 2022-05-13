---
title: Тип ресурса privilegedRoleAssignmentRequest
description: Представляет запрос на операции назначения ролей в Privilegd Identity Management.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: a22049c1f3de095e7146a1e9cd901db8d6f5fd6a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398856"
---
# <a name="privilegedroleassignmentrequest-resource-type-deprecated"></a>Тип ресурса privilegedRoleAssignmentRequest (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Представляет запрос для операций назначения ролей в управление привилегированными пользователями (PIM).

`privilegedRoleAssignmentRequest` — это сущность, с помощью модели билета, используемая для управления жизненным циклом назначений ролей. Он представляет намерение и решение пользователей и администраторов, а также обеспечивает гибкость для реализации повторяющихся схем, шлюзов утверждения и т. д., `POST` `Cancel` `LIST` `MY` `governanceRoleAssignment`по сравнению с предоставлением непосредственного доступа и операций, а также функций в .

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Перечисление](../api/privilegedroleassignmentrequest-list.md) | [Коллекция privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Вывод списка запросов на назначение ролей.|
|[Создание](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Создайте запрос для управления жизненным циклом существующего или нового назначения ролей.|
|[Отмена](../api/privilegedroleassignmentrequest-cancel.md)|  |Отмена ожидающего запроса на назначение роли.|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |Получение запроса на назначение роли для текущего requstor.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения. Идентификатор запроса на назначение роли.|
|assignmentState|String| Состояние назначения. Значение может быть задано `Eligible` для `Active` допустимого назначения , `Active` если оно напрямую назначено администраторами или активировано для допустимого назначения пользователями.|
|duration|String| Длительность назначения роли.|
|reason|String| Причина назначения роли.|
|requestedDateTime|DateTimeOffset| Только для чтения. Время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|roleId|String| Идентификатор роли.|
|schedule|[governanceSchedule](governanceschedule.md)| Объект расписания запроса на назначение роли.|
|status|String| Только для чтения. Состояние запроса на назначение роли. Значение может быть `NotStarted`:`Completed`,,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,,`Cancelled`,`Revoked`,`RequestExpired`.|
|ticketNumber|String| Номер билета для назначения роли. |
|ticketSystem|String| Система ticketSystem для назначения роли.|
|type|String| Представляет тип операции назначения роли. Значение может быть: `AdminAdd`администраторы добавляют пользователей к ролям;`UserAdd` пользователи добавляют назначения ролей.|
|userId|String| Идентификатор пользователя.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| Объект roleInfo запроса на назначение роли.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}-->

```json
{
  "assignmentState": "String",
  "duration": "String",
  "id": "String (identifier)",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "roleId": "String",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": "String",
  "ticketNumber": "String",
  "ticketSystem": "String",
  "type": "String",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


