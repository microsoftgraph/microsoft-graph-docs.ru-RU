---
title: тип ресурса privilegedRoleAssignmentRequest
description: Представляет запрос на операции назначения ролей в Privilegd Identity Management.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 59144fd6008e081eb6de29c94626fe5fb2c57af6
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454131"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>тип ресурса privilegedRoleAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос на операции назначения ролей в Privilegd Identity Management.

`privilegedRoleAssignmentRequest` — это объект, моделируемый билетами, используемый для управления жизненным циклом назначений ролей. Он представляет намерения и решения пользователей и администраторов, а также обеспечивает гибкость, чтобы включить реализацию повторяющихся schduling, ворота утверждения и так далее, по сравнению с непосредственной разоблачения и операций, а также и функций `POST` `LIST` на `MY` `Cancel` `governanceRoleAssignment` .

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Список](../api/privilegedroleassignmentrequest-list.md) | [коллекция privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Список запросов на назначение ролей.|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)|Создайте запрос для управления жизненным циклом существующего или нового назначения ролей.|
|[Отмена](../api/privilegedroleassignmentrequest-cancel.md)|  |Отмена ожидающих запросов на назначение ролей.|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |Получите запрос на назначение ролей для текущего requstor.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения. ID запроса на назначение ролей.|
|assignmentState|String| Состояние назначения. Это значение может быть для присвоения, если оно непосредственно назначено администраторами или активировано при назначении, назначенного `Eligible` `Active` `Active` пользователями.|
|duration|String| Продолжительность назначения ролей.|
|reason|String| Причина назначения роли.|
|requestedDateTime|DateTimeOffset| Только для чтения. Время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|roleId|String| ID роли.|
|schedule|[governanceSchedule](governanceschedule.md)| Объект расписания запроса назначения ролей.|
|status|String| Read-only.The status of the role assignment request. Значение может быть `NotStarted` , , , , , , , `Completed` , `RequestedApproval` `Scheduled` `Approved` `ApprovalDenied` `ApprovalAborted` `Cancelling` `Cancelled` `Revoked` `RequestExpired` .|
|ticketNumber|String| TicketNumber для назначения роли. |
|ticketSystem|String| TicketSystem для назначения ролей.|
|type|String| Представление типа операции при назначении ролей. Значение может `AdminAdd` быть: Администраторы добавляют пользователей в роли; `UserAdd` : Пользователи добавляют назначения ролей.|
|userId|String| ID пользователя.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| Объект roleInfo запроса назначения ролей.|

## <a name="json-representation"></a>Представление JSON

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


