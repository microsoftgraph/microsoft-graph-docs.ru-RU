---
title: Тип ресурса Привилежедролеассигнментрекуест
description: Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.
localization_priority: Normal
ms.openlocfilehash: c0e0bbfa76b7ffb4e122d381d45dd4092f0843c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563361"
---
# <a name="privilegedroleassignmentrequest-resource-type"></a>Тип ресурса Привилежедролеассигнментрекуест

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.

`privilegedRoleAssignmentRequest`— Это объект с моделированием билетов, используемый для управления жизненным циклом назначений ролей. Он представляет намерение/решение для пользователей и администраторов, а также обеспечивает гибкость, позволяющую включать реализацию перечисленных счдулинг, шлюзов утверждения и т. д., в отличие от прямого предоставления `POST` и `LIST` операций, а также `MY` и `Cancel` функции On `governanceRoleAssignment`.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[List](../api/privilegedroleassignmentrequest-list.md) | Коллекция [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md)|Список запросов на назначение ролей.|
|[Создание](../api/privilegedroleassignmentrequest-post.md)|  [привилежедролеассигнментрекуест](../resources/privilegedroleassignmentrequest.md)|Создание запроса на управление жизненным циклом существующего или нового назначения роли.|
|[Отмена](../api/privilegedroleassignmentrequest-cancel.md)|  |Отмена ожидающего запроса на назначение роли.|
|[My](../api/privilegedroleassignmentrequest-my.md)|  |Получение запроса на назначение роли для текущего рекустор.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения. Идентификатор запроса на назначение роли.|
|Ассигнментстате|String| Состояние назначения. Значение может быть `Eligible` для правого назначения `Active` , если оно напрямую назначено `Active` администраторами или активировано в соответствии с подходящими пользователями.|
|duration|String| Продолжительность назначения роли.|
|причиной|String| Причина назначения роли.|
|Рекуестеддатетиме|DateTimeOffset| Только для чтения. Время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|roleId|String| Идентификатор роли.|
|Диспетчер|[governanceSchedule](governanceschedule.md)| Объект расписания для запроса на назначение роли.|
|status|Строка| Только для чтения. состояние запроса на назначение роли. Возможные значения `NotStarted``Completed`:,`RequestedApproval``Scheduled``Approved``Revoked``RequestExpired`,,,,,,,,,.`ApprovalDenied``ApprovalAborted``Cancelling``Cancelled`|
|Тиккетнумбер|String| Тиккетнумбер для назначения роли. |
|Тиккетсистем|String| Тиккетсистем для назначения роли.|
|type|String| Представляет тип операции для назначения роли. Возможные значения `AdminAdd`: Администраторы Add Users to Roles; `UserAdd`: Пользователи добавляют назначения ролей.|
|userId|String| Идентификатор пользователя.|

## <a name="relationships"></a>Связи
| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|Ролеинфо|[privilegedRole](privilegedrole.md)| Объект Ролеинфо запроса назначения роли.|

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
