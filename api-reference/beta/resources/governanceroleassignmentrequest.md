---
title: Тип ресурса governanceRoleAssignmentRequest
description: Представляет запрос для операций назначения роли управления удостоверениями Privilegd.
localization_priority: Normal
ms.openlocfilehash: 838d16455a2eaea2183d008800eaef72a0af2a15
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572103"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>Тип ресурса governanceRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос для операций назначения роли управления удостоверениями Privilegd.

`governanceRoleAssignmentRequest`смоделировать билетов сущности, используется для управления жизненным циклом назначения ролей. Он представляет намерения/решение для пользователей и администраторов, а также обеспечивает гибкость для внедрения повторяющаяся schduling, шлюзы утверждения и т. д. по сравнению с непосредственно предоставление `POST`, `PUT`, и `DELETE` операции на `governanceRoleAssignment`.

## <a name="methods"></a>Методы

| Метод          |Возвращаемый тип  |Описание|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignmentrequest-get.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Получите запрос назначения ролей, заданную идентификатором.  
|[List](../api/governanceroleassignmentrequest-list.md) | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) коллекции|Получите запросы назначений ролей для ресурса.|
|[Create](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Создание запроса для управления жизненным циклом существующего или нового назначения роли.|
|[Cancel](../api/governanceroleassignmentrequest-cancel.md)|  |Отмена назначения запроса ожидающие роли.|
|[Update](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Администраторы обновлять решения на запросы, если запросов в состояние `PendingAdminDecision`.|

## <a name="properties"></a>Свойства
| Свойство                  | Тип          |Описание|
|:--------------------------|:--------------|:----------|
|id                         |Строка         |Идентификатор запроса назначений ролей.|
|resourceId                 |Строка         |Обязательный. Идентификатор ресурса запрос назначения ролей, связанный с.|
|roleDefinitionId           |Строка         |Обязательный. Идентификатор запрос назначения ролей, связанный с определения роли.|
|subjectId                  |Строка         |Обязательный. Идентификатор субъекта, запрос назначения ролей, связанный с.|
|type                       |Строка         |Обязательный. Представляет тип операции в назначении ролей. Значение может быть <ul><li>`AdminAdd`: Администраторам назначение пользователей и групп для роли.</li><li>`UserAdd`: Пользователи активировать подходящими назначения;</li><li> `AdminUpdate`: Администраторам изменение существующего назначения ролей</li><li>`AdminRemove`: Администраторам удаление пользователей и групп из роли.<li>`UserRemove`: Пользователи отключение active назначения;<li>`UserExtend`: Пользователи запрос для расширения их истекающим сроком действия назначения;</li><li>`AdminExtend`: Администраторы расширение назначений с истекающим сроком действия.</li><li>`UserRenew`: Пользователи запроса на обновление назначений истекшим сроком действия;</li><li>`AdminRenew`: Администраторы расширение назначений с истекающим сроком действия.</li></ul>|
|assignmentState|Строка  |Обязательный. Состояние назначения. Значение может быть <ul><li> `Eligible`для подходящими назначения</li><li> `Active`-Если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей.</li></ul>|
|requestedDateTime          |DateTimeOffset |Только для чтения. Время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|расписание                   |[microsoft.graph.governanceSchedule](governanceschedule.md)|Объект расписание запрос назначения ролей.|
|Причина                     |Строка         |Сообщение, предоставляемые пользователями и администраторами при создании запроса о зачем он нужен.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |Состояние запроса назначений ролей.|
|linkedEligibleRoleAssignmentId|Строка        |Если запрос для активации роли, он представляет идентификатор `eligible assignment` ссылки; В противном случае — значение `null`. |



## <a name="relationships"></a>Связи
| Связь | Тип                                |Описание|
|:-------------|:----------------------------------|:----------|
|resource      |[governanceResource](../resources/governanceresource.md)            |Только для чтения. Ресурс, запрос имеет своей целью. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение ролей, запрос имеет своей целью. |
|subject       |[governanceSubject](../resources/governancesubject.md)|Только для чтения. Участника пользователя или группы.|

### <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
