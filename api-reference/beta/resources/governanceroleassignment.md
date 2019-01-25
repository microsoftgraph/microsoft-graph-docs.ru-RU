---
title: Тип ресурса governanceRoleAssignment
description: Представляет назначения пользователя или группы на роль.
localization_priority: Normal
ms.openlocfilehash: 77a5238aa337dd8d273d3156d285e081c4bc8875
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512684"
---
# <a name="governanceroleassignment-resource-type"></a>Тип ресурса governanceRoleAssignment
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначения пользователя или группы на роль.

Управление правами Identity (PIM) поддерживает два типа назначения.

1. Активное назначение — предоставляет доступ/активирован непосредственно к ресурсам.
2. Допустимость назначения — представляет промежуточного этапа привилегированный доступ к ресурсам между нет доступа и прямой доступ. Администраторы могут назначать пользователей и групп для `eligible assignment` заранее, а каждый раз, когда требуется доступ, `activation` на `eligible assignment` необходим для получения быстрого доступа к ресурсу для нескольких часов. После активации `active assignment` будут создаваться заинтересованных пользователей и групп для указания состояния активации.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Чтение свойства и связи объекта назначения ролей.|
|[List](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md) коллекции|Список коллекции назначения ролей для ресурса. |
|[Export](../api/governanceroleassignment-export.md) | потока октетов |Загрузите набор из назначения ролей для ресурса и сохранить как `.csv` файла.|

Не `POST`, `PUT`, `PATCH`, или `DELETE` поддерживается на `roleAssignments` набора сущностей. Любой создание, обновление и удаление операций на `governanceRoleAssignment` выполнить по `governanceRoleAssignmentRequest`.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |Строка     |Идентификатор назначения ролей. Это в формате GUID.|
|resourceId |Строка     |Обязательный. Идентификатор ресурса, назначения ролей, связанный с. |
|roleDefinitionId|Строка|Обязательный. Идентификатор определения роли, назначения ролей, связанный с. |
|subjectId|Строка       |Обязательный. Идентификатор субъекта, назначения ролей, связанный с. |
|linkedEligibleRoleAssignmentId|String|Если это `active assignment` и создано из-за активации на `eligible assignment`, представляющий идентификатор, который `eligible assignment`; В противном случае — значение `null`. |
|externalId   |String     |Внешний идентификатор ресурса, используемый для идентификации назначения роли в поставщик.|
|startDateTime|DateTimeOffset|Время начала назначения ролей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Назначение ролей не постоянная — это время, когда срока действия назначения ролей. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|assignmentState|String  |Состояние назначения. Значение может быть <ul><li> `Eligible`для подходящими назначения</li><li> `Active`-Если она назначена непосредственно `Active` администраторами, или активируемого на допустимость назначения для пользователей.</li></ul>|
|memberType|String      |Тип элемента. Значение может быть: <ul><li>`Inherited`-Назначение ролей наследуется от родительской области ресурсов</li><li>`Group`-назначения ролей не наследуется, но, поступающие из членства Назначение группы</li><li>`User`-не наследуется назначения ролей, ни из Назначение группы.</li></ul>|


## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Ресурс, связанный с назначения ролей. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, связанные с назначения ролей. |
|subject|[governanceSubject](../resources/governancesubject.md)|Только для чтения. Тема, связанная с назначения ролей. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Только для чтения. Если это `active assignment` и создано из-за активации на `eligible assignment`, представляющий объект, который `eligible assignment`; В противном случае — значение `null`. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
