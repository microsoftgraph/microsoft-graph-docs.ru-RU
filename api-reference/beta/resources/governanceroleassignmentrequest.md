---
title: Тип ресурса governanceRoleAssignmentRequest
description: Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 91c4cf596ead6dac9a1cea58ecba2c04365e1279
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058398"
---
# <a name="governanceroleassignmentrequest-resource-type"></a>Тип ресурса governanceRoleAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос для операций назначения ролей в Привилегд управления удостоверениями.

`governanceRoleAssignmentRequest` — Это объект с моделированием билетов, используемый для управления жизненным циклом назначений ролей. Он представляет намерение/решение для пользователей и администраторов, а также обеспечивает гибкость, позволяющую включать реализацию перечисленных счдулинг, шлюзов утверждения и т. д., по сравнению с прямым предоставлением `POST` `PUT` и `DELETE` работой с `governanceRoleAssignment` .

## <a name="methods"></a>Методы

| Метод          |Возвращаемый тип  |Описание|
|:------------|:--------|:--------|
|[получение](../api/governanceroleassignmentrequest-get.md); | [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Получение запроса на назначение роли, указанного по ИДЕНТИФИКАТОРу.  
|[Список](../api/governanceroleassignmentrequest-list.md) | Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Получение запросов на назначение ролей ресурсу.|
|[Создание](../api/governanceroleassignmentrequest-post.md)|  [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Создание запроса на управление жизненным циклом существующего или нового назначения роли.|
|[Отмена](../api/governanceroleassignmentrequest-cancel.md)|  |Отмена ожидающего запроса на назначение роли.|
|[Обновление](../api/governanceroleassignmentrequest-update.md)| [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Администраторы обновляют решения в запросах, если запросы находятся в состоянии `PendingAdminDecision` .|

## <a name="properties"></a>Свойства
| Свойство                  | Тип          |Описание|
|:--------------------------|:--------------|:----------|
|id                         |String         |Идентификатор запроса на назначение роли.|
|resourceId                 |String         |Обязательный. Идентификатор ресурса, с которым связан запрос назначения роли.|
|роледефинитионид           |String         |Обязательный. Идентификатор определения роли, с которым связан запрос назначения роли.|
|субжектид                  |String         |Обязательный. Идентификатор субъекта, с которым связан запрос назначения роли.|
|type                       |String         |Обязательный. Представляет тип операции для назначения роли. Значение может быть <ul><li>`AdminAdd`: Администраторы назначают роли пользователям и группам.</li><li>`UserAdd`: Пользователи активируют подходящие назначения;</li><li> `AdminUpdate`: Администраторы изменяют существующие назначения ролей</li><li>`AdminRemove`: Администраторы удаляют пользователей и группы из ролей;<li>`UserRemove`: Пользователи деактивируют активные назначения;<li>`UserExtend`: Пользователи запрашивают, чтобы расширить их назначения с истекшим сроком действия;</li><li>`AdminExtend`: Администраторы расширяют назначения с истекающим сроком действия.</li><li>`UserRenew`: Пользователи запрашивают обновление назначений с истекшим сроком действия;</li><li>`AdminRenew`: Администраторы расширяют назначения с истекающим сроком действия.</li></ul>|
|ассигнментстате|String  |Обязательный. Состояние назначения. Значение может быть <ul><li> `Eligible` для подходящего назначения</li><li> `Active` — Если он напрямую назначается `Active` администраторами или активирован в соответствии с подходящими пользователями.</li></ul>|
|рекуестеддатетиме          |DateTimeOffset |Только для чтения. Время создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|schedule                   |[governanceSchedule](governanceschedule.md)|Объект расписания для запроса на назначение роли.|
|reason                     |String         |Сообщение, предоставленное пользователями и администраторами при создании запроса о том, почему это необходимо.|
|status                     |[governanceRoleAssignmentRequestStatus](governanceroleassignmentrequeststatus.md)         |Состояние запроса на назначение роли.|
|линкеделигиблеролеассигнментид|String        |Если это запрос на активацию роли, он представляет идентификатор, на который `eligible assignment` ссылается ссылка; В противном случае — значение `null` . |



## <a name="relationships"></a>Отношения
| Связь | Тип                                |Описание|
|:-------------|:----------------------------------|:----------|
|resource      |[governanceResource](../resources/governanceresource.md)            |Только для чтения. Ресурс, на который запрашивается запрос. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, которому назначен запрос. |
|subject       |[говернанцесубжект](../resources/governancesubject.md)|Только для чтения. Участник группы "пользователь/группа".|

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


