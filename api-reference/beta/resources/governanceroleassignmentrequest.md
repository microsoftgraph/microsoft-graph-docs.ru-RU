---
title: Тип ресурса governanceRoleAssignmentRequest
description: Представляет запрос на операции назначения ролей в Priviledged Identity Management.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 4dd6c1c5911193306c6a0925bfec1d642a00a81c
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397588"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>Тип ресурса governanceRoleAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет запрос для операций назначения ролей в управление привилегированными пользователями.

`governanceRoleAssignmentRequest` — это сущность, с помощью модели билета, используемая для управления жизненным циклом назначений ролей. Он представляет намерение и решение пользователей и администраторов, а также обеспечивает гибкость для реализации повторяющихся схем, шлюзов утверждения и т. д., `POST``PUT``DELETE` `governanceRoleAssignment`по сравнению с предоставлением непосредственного доступа и операций с .

## <a name="methods"></a>Методы

| Метод          |Возвращаемый тип  |Описание|
|:------------|:--------|:--------|
|[Получение](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Получение запроса на назначение роли, указанного по идентификатору.  
|[Перечисление](../api/governanceroleassignmentrequest-list.md) | [Коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Получение запросов на назначение ролей для ресурса.|
|[Создание](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Создайте запрос для управления жизненным циклом существующего или нового назначения ролей.|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |Отмена ожидающего запроса на назначение роли.|
|[Обновление](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Администраторы обновляют решения по запросам, если запросы находятся в состоянии . `PendingAdminDecision`.|

## <a name="properties"></a>Свойства
| Свойство                  | Тип          |Описание|
|:--------------------------|:--------------|:----------|
|id                         |String         |Идентификатор запроса на назначение роли.|
|resourceId                 |String         |Обязательный. Уникальный идентификатор ресурса Azure, связанного с запросом на назначение роли. Ресурсы Azure могут включать подписки, группы ресурсов, виртуальные машины и базы данных SQL.|
|roleDefinitionId           |String         |Обязательный. Идентификатор определения роли Azure, с помощью которого связан запрос на назначение ролей.|
|subjectId                  |String         |Обязательный. Уникальный идентификатор субъекта или субъекта, с помощью которого связан запрос на назначение ролей. Субъектами могут быть пользователи, группы или субъекты-службы.|
|type                       |String        |Обязательный. Представляет тип операции назначения роли. Возможные значения: `AdminAdd` , , `UserAdd` , `AdminUpdate` , `AdminRemove` , `UserRemove` , `AdminRenew``UserExtend` `AdminExtend` `UserRenew` .|
|assignmentState|String  |Обязательный. Состояние назначения. Возможные значения: `Eligible` (для допустимого назначения),  `Active` (если оно назначено напрямую) `Active` (администраторами или активировано для допустимого назначения пользователями).|
|requestedDateTime          |DateTimeOffset |Только для чтения. Время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|schedule                   |[governanceSchedule](governanceschedule.md)|Объект расписания запроса на назначение роли.|
|reason                     |String         |Сообщение, предоставленное пользователями и администраторами при создании запроса о том, зачем он нужен.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |Состояние запроса на назначение роли.|
|linkedEligibleRoleAssignmentId|String        |Если это запрос на активацию роли, он представляет идентификатор `eligible assignment` ссылаемого; В противном случае значение равно `null`. |

|Member|Описание|
|:---|:---|
|AdminAdd|Администраторы назначают пользователям или группам роли.|
|UserAdd|Пользователи активируют допустимые назначения.|
|AdminUpdate|Администраторы изменяют существующие назначения ролей.|
|AdminRemove|Администраторы удаляют пользователей и группы из ролей.|
|UserRemove|Пользователи отключают активные назначения.|
|UserExtend|Пользователи запрашивают продление назначений с истекающим сроком действия.|
|AdminExtend|Администраторы расширяют назначения с истекающим сроком действия.|
|UserRenew|Пользователи запрашивают продление назначений с истекшим сроком действия.|
|AdminRenew|Администраторы расширяют назначения с истекающим сроком действия.|



## <a name="relationships"></a>Связи
| Связь | Тип                                |Описание|
|:-------------|:----------------------------------|:----------|
|resource      |[governanceResource](../resources/governanceresource.md)            |Только для чтения. Ресурс, на который нацелен запрос. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, на которое направлен запрос. |
|subject       |[governanceSubject](../resources/governancesubject.md)|Только для чтения. Пользователь или субъект группы.|

### <a name="json-representation"></a>Представление в формате JSON

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


