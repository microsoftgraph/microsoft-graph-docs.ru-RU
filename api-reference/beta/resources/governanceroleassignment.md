---
title: Тип ресурса governanceRoleAssignment
description: Представляет назначение роли пользователю или группе.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 76aaa6e63b9c44e1bc3db1ccf6e8351a5796051f
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399462"
---
# <a name="governanceroleassignment-resource-type"></a>Тип ресурса governanceRoleAssignment

Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет назначение роли пользователю или группе.

управление привилегированными пользователями (PIM) поддерживает два типа назначений:

1. Активное назначение — представляет прямой или активированный доступ к ресурсам.
2. Допустимое назначение — представляет промежуточный этап привилегированного доступа к ресурсам между отсутствием доступа и прямым доступом. Администраторы могут назначать `eligible assignment` пользователей или группы заранее, и каждый раз, когда требуется доступ, `eligible assignment` `activation` требуется для получения мгновенного доступа к ресурсу в течение нескольких часов. После активации будет создано `active assignment` для пользователей или членов группы, чтобы указать состояние активации.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:------------|:--------|:--------|
|[Получение](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Чтение свойств и связей сущности назначения роли.|
|[Перечисление](../api/governanceroleassignment-list.md) | [Коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)|Перечисление коллекции назначений ролей для ресурса. |
|[Export](../api/governanceroleassignment-export.md) | octet-stream |Скачайте коллекцию назначений ролей для ресурса и сохраните ее в виде `.csv` файла.|

В `POST`наборе `PATCH``PUT`сущностей `DELETE` `roleAssignments` не поддерживаются операции, а также операции. Любые операции создания, обновления и удаления `governanceRoleAssignment` выполняются с помощью `governanceRoleAssignmentRequest`.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |Идентификатор назначения роли. Он имеет формат GUID.|
|resourceId |String     |Обязательный. Идентификатор ресурса, с которым связано назначение роли. |
|roleDefinitionId|String|Обязательный. Идентификатор определения роли, с которым связано назначение роли. |
|subjectId|String       |Обязательный. Идентификатор субъекта, с которым связано назначение роли. |
|linkedEligibleRoleAssignmentId|String|Если это действие создано `active assignment` из-за активации в объекте `eligible assignment`, он представляет его идентификатор `eligible assignment`; В противном случае значение равно `null`. |
|externalId   |String     |Внешний идентификатор ресурса, который используется для идентификации назначения роли в поставщике.|
|startDateTime|DateTimeOffset|Время начала назначения роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|endDateTime|DateTimeOffset|Для назначения неповратимых ролей это время, когда срок действия назначения роли истекает. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|assignmentState|String  |Состояние назначения. Это значение может быть предназначено `Eligible` `Active` `Active` для допустимого назначения или если оно напрямую назначено администраторами или активировано для допустимого назначения пользователями.|
|memberType|String      |Тип члена. Значение может быть: `Inherited` (если назначение роли наследуется от области родительского ресурса), `Group` (если назначение роли не наследуется, а происходит от членства в назначении группы) `User` или (если назначение роли не наследуется или не наследуется от назначения группы).|


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Ресурс, связанный с назначением роли. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, связанное с назначением роли. |
|subject|[governanceSubject](../resources/governancesubject.md)|Только для чтения. Тема, связанная с назначением роли. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Только для чтения. Если это объект, созданный `active assignment` из-за активации в объекте `eligible assignment`, он представляет его; `eligible assignment` В противном случае значение равно `null`. |

## <a name="json-representation"></a>Представление в формате JSON

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


