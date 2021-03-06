---
title: тип ресурса governanceRoleAssignment
description: Представляет назначение пользователя или группы роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6d9e1b56a503ffdf1bde6bde6a583b78f8a34851
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722309"
---
# <a name="governanceroleassignment-resource-type"></a>тип ресурса governanceRoleAssignment

Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначение пользователя или группы роли.

Привилегированное управление удостоверениями (PIM) поддерживает два типа назначений:

1. Активное назначение — представляет прямой или активированный доступ к ресурсам.
2. Право назначения — представляет промежуточный этап привилегированного доступа к ресурсам между отсутствием доступа и прямым доступом. Администраторы могут назначать пользователям или группам заранее, и всякий раз, когда необходим доступ, необходимо получить мгновенный доступ к ресурсу `eligible assignment` `activation` в течение нескольких `eligible assignment` часов. После активации будет создано для пользователей или членов группы, чтобы указать `active assignment` активированный статус.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:------------|:--------|:--------|
|[получение](../api/governanceroleassignment-get.md); |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Чтение свойств и связей объекта назначения ролей.|
|[List](../api/governanceroleassignment-list.md) | [коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)|Список набор назначений ролей на ресурсе. |
|[Экспорт](../api/governanceroleassignment-export.md) | octet-stream |Скачайте коллекцию назначений ролей на ресурсе и сохраните в качестве `.csv` файла.|

Нет `POST` , или операции `PUT` `PATCH` `DELETE` поддерживаются в `roleAssignments` наборе сущности. Любые операции по созданию, обновлению и удаляемой работе `governanceRoleAssignment` делаются `governanceRoleAssignmentRequest` путем .

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |ID назначения роли. Он находится в формате GUID.|
|resourceId |String     |Обязательный. ID ресурса, с которым связано назначение ролей. |
|roleDefinitionId|String|Обязательный. ID определения роли, с которым связано назначение ролей. |
|subjectId|String       |Обязательный. ID субъекта, с которым связано назначение ролей. |
|linkedEligibleRoleAssignmentId|String|Если это и создано из-за активации `active assignment` на , он представляет собой `eligible assignment` ID `eligible assignment` этого; В противном случае значение `null` . |
|externalId   |String     |Внешний ID ресурса, который используется для определения назначения роли в поставщике.|
|startDateTime|DateTimeOffset|Время начала назначения роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|endDateTime|DateTimeOffset|Для назначения непостоянных ролей это время, когда срок действия назначения роли истекает. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|assignmentState|String  |Состояние назначения. Значение может быть <ul><li> `Eligible` для назначения</li><li> `Active` - если оно непосредственно назначено администраторами или активировано при назначении, назначенное `Active` пользователями.</li></ul>|
|memberType|String      |Тип участника. Значение может быть: <ul><li>`Inherited` — назначение роли наследуется из области родительского ресурса</li><li>`Group`— назначение роли не наследуется, а происходит от членства в групповом назначении</li><li>`User` — назначение роли не наследуется или не наследуется групповым назначением.</li></ul>|


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Ресурс, связанный с назначением ролей. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, связанное с назначением роли. |
|subject|[governanceSubject](../resources/governancesubject.md)|Только для чтения. Тема, связанная с назначением ролей. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Только для чтения. Если это и `active assignment` создается из-за активации на объекте, он представляет `eligible assignment` объект `eligible assignment` этого; В противном случае значение `null` . |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


