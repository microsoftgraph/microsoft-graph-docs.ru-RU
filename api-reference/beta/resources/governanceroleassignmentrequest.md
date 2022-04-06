---
title: тип ресурса governanceRoleAssignmentRequest
description: Представляет запрос на операции назначения ролей в Priviledged Identity Management.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: e96babfcc2510ae3a942618ff0346d833e4e6fca
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510311"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>тип ресурса governanceRoleAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет запрос на операции назначения ролей в управление привилегированными пользователями.

`governanceRoleAssignmentRequest` — это объект, моделируемый билетами, используемый для управления жизненным циклом назначений ролей. Он представляет намерения и решения пользователей и администраторов, а также обеспечивает гибкость, чтобы включить реализацию повторяющихся schduling, ворота утверждения и так далее, `POST`по сравнению с непосредственной разоблачения , `PUT`и `DELETE` `governanceRoleAssignment`операций на .

## <a name="methods"></a>Методы

| Метод          |Возвращаемый тип  |Описание|
|:------------|:--------|:--------|
|[Получение](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Получите запрос на назначение ролей, указанный в ID.  
|[перечисление](../api/governanceroleassignmentrequest-list.md); | [коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Получить запросы на назначение ролей на ресурсе.|
|[Создание](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Создайте запрос для управления жизненным циклом существующего или нового назначения ролей.|
|[Отмена](../api/governanceroleassignmentrequest-cancel.md)|  |Отмена ожидающих запросов на назначение ролей.|
|[обновление](../api/governanceroleassignmentrequest-update.md);| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Администраторы обновляют решения по запросам, если запросы находятся в состоянии `PendingAdminDecision`.|

## <a name="properties"></a>Свойства
| Свойство                  | Тип          |Описание|
|:--------------------------|:--------------|:----------|
|id                         |Строка         |Идентификатор запроса на назначение ролей.|
|resourceId                 |String         |Обязательный. Уникальный идентификатор ресурса Azure, связанный с запросом на назначение ролей. Ресурсы Azure могут включать подписки, группы ресурсов, виртуальные машины и SQL базы данных.|
|roleDefinitionId           |String         |Обязательный. Идентификатор определения роли Azure, с котором связан запрос на назначение ролей.|
|subjectId                  |String         |Обязательный. Уникальный идентификатор основного или субъекта, с который связан запрос на назначение ролей. Директорами могут быть пользователи, группы или директора службы.|
|type                       |Строка        |Обязательный. Представление типа операции при назначении ролей. Возможные значения: `AdminAdd` , , `AdminUpdate` `UserAdd` , , `AdminRemove` , `UserRemove` , `AdminRenew``UserExtend` `AdminExtend` `UserRenew` .|
|assignmentState|String  |Обязательный. Состояние назначения. Возможные значения: `Eligible` (для назначения, назначенного по назначению),  `Active` (если оно непосредственно назначено) `Active` (администраторами или активировано при назначении, назначенное пользователями).|
|requestedDateTime          |DateTimeOffset |Только для чтения. Время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|schedule                   |[governanceSchedule](governanceschedule.md)|Объект расписания запроса назначения ролей.|
|reason                     |Строка         |Сообщение, предоставленное пользователями и администраторами при создании запроса о необходимости.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |Состояние запроса на назначение ролей.|
|linkedEligibleRoleAssignmentId|String        |Если это запрос на активацию роли, он представляет id `eligible assignment` переданного; В противном случае значение `null`. |

|Member|Описание|
|:---|:---|
|AdminAdd|Администраторы назначают пользователям/группам роли.|
|UserAdd|Пользователи активируют подходящие назначения.|
|AdminUpdate|Администраторы изменяют существующие назначения ролей.|
|AdminRemove|Администраторы удаляют пользователей и группы из ролей.|
|UserRemove|Пользователи отключат активные назначения.|
|UserExtend|Пользователи просят продлить срок действия назначений.|
|AdminExtend|Администраторы расширяют назначения по истечении срока действия.|
|UserRenew|Пользователи просят продлить истекаемы назначения.|
|AdminRenew|Администраторы расширяют назначения по истечении срока действия.|



## <a name="relationships"></a>Связи
| Связь | Тип                                |Описание|
|:-------------|:----------------------------------|:----------|
|resource      |[governanceResource](../resources/governanceresource.md)            |Только для чтения. Ресурс, на который направлен запрос. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, на которое направлен запрос. |
|subject       |[governanceSubject](../resources/governancesubject.md)|Только для чтения. Основной пользователь/группа.|

### <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "type": "String",
  "assignmentState": "String",
  "reason": "String",
  "requestedDateTime": "String (timestamp)",
  "schedule": {"@odata.type": "microsoft.graph.governanceSchedule"},
  "status": {"@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"},
  "linkedEligibleRoleAssignmentId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


