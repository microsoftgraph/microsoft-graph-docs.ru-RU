---
title: Тип ресурса privilegedRoleAssignmentRequest
description: Представляет запрос для операций назначения роли управления удостоверениями Privilegd.
localization_priority: Normal
ms.openlocfilehash: a0cb0bc03d8bb2436e45139bc9db5322cc3970cf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571751"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>Тип ресурса privilegedRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос для операций назначения роли управления удостоверениями Privilegd.

`privilegedRoleAssignmentRequest`смоделировать билетов сущности, используется для управления жизненным циклом назначения ролей. Он представляет намерения/решение для пользователей и администраторов, а также обеспечивает гибкость для внедрения повторяющаяся schduling, шлюзы утверждения и т. д. по сравнению с непосредственно предоставление `POST` и `LIST` операции в том числе в `MY` и `Cancel` функции на `governanceRoleAssignment`.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) коллекции|Список запросов назначения ролей.|
|[Create](../api/privilegedroleassignmentrequest-post.md)|  [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|Создание запроса для управления жизненным циклом существующего или нового назначения роли.|
|[Cancel](../api/privilegedroleassignmentrequest-cancel.md)|  |Отмена назначения запроса ожидающие роли.|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |Получите запрос назначения ролей для текущего запрашивающего.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Только для чтения. Идентификатор запроса назначений ролей.|
|assignmentState|Строка| Состояние назначения. Значение может быть `Eligible` подходящими назначения `Active` - если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей.|
|duration|Строка| Длительность назначения ролей.|
|Причина|Строка| Причина для назначения ролей.|
|requestedDateTime|DateTimeOffset| Только для чтения. Время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|roleId|Строка| Идентификатор роли.|
|расписание|[microsoft.graph.governanceSchedule](governanceschedule.md)| Объект расписание запрос назначения ролей.|
|status|Строка| Состояние чтения only.The запрос назначения ролей. Значение может быть `NotStarted`,`Completed`,`RequestedApproval`,`Scheduled`,`Approved`,`ApprovalDenied`,`ApprovalAborted`,`Cancelling`,`Cancelled`,`Revoked`,`RequestExpired`.|
|ticketNumber|Строка| TicketNumber назначения роли. |
|ticketSystem|Строка| TicketSystem назначения роли.|
|type|Строка| Представляет тип операции в назначении ролей. Значение может быть `AdminAdd`: администраторам Добавление пользователей в роли. `UserAdd`: Добавление назначений ролей пользователей.|
|userId|String| Идентификатор пользователя.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|roleInfo|[privilegedRole](privilegedrole.md)| Объект roleInfo запрос назначения ролей.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
