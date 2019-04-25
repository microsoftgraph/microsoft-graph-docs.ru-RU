---
title: Тип ресурса governanceRoleAssignment
description: Представляет назначение роли пользователю или группе.
localization_priority: Normal
ms.openlocfilehash: 77a5238aa337dd8d273d3156d285e081c4bc8875
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547452"
---
# <a name="governanceroleassignment-resource-type"></a>Тип ресурса governanceRoleAssignment
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначение роли пользователю или группе.

Привилегированное управление удостоверениями (PIM) поддерживает два типа назначений:

1. Активное назначение — представляет прямой/активированный доступ к ресурсам.
2. ПодХодящие назначения — представляет промежуточный этап привилегированного доступа к ресурсам, между отсутствием доступа и прямым доступом. Администраторы могут заранее назначать пользователей и группы `eligible assignment` , а при необходимости `activation` `eligible assignment` получить доступ к ресурсу в течение нескольких часов. После активации `active assignment` будет создана группа для пользователей и членов группы, указывающая состояние активации.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:------------|:--------|:--------|
|[Получение](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Чтение свойств и связей объекта назначения роли.|
|[List](../api/governanceroleassignment-list.md) | Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)|ПереЧисление коллекции назначений ролей для ресурса. |
|[Export](../api/governanceroleassignment-export.md) | поток в октетах |Скачайте коллекцию назначений ролей для ресурса и сохраните ее `.csv` в виде файла.|

`PUT` `POST` `roleAssignments` В наборе сущностей `DELETE` поддерживаются не поддерживаемые операции, а также операции. `PATCH` Все операции по `governanceRoleAssignment` созданию, обновлению и удалению выполняются `governanceRoleAssignmentRequest`.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |Идентификатор назначения роли. Он указан в формате GUID.|
|resourceId |String     |Обязательный. Идентификатор ресурса, с которым связано назначение роли. |
|Роледефинитионид|String|Обязательный. Идентификатор определения роли, с которым связано назначение роли. |
|Субжектид|String       |Обязательный. ИДЕНТИФИКАТОР субъекта, с которым связано назначение роли. |
|Линкеделигиблеролеассигнментид|String|Если он создан `active assignment` и создан в результате активации `eligible assignment`, он представляет идентификатор этого `eligible assignment`объекта; В противном случае — `null`значение. |
|externalId   |String     |Внешний идентификатор — ресурс, который используется для идентификации назначения роли в поставщике.|
|startDateTime|DateTimeOffset|Время начала назначения роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Для назначения непостоянных ролей это время истечения срока действия назначения роли. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Ассигнментстате|String  |Состояние назначения. Значение может быть <ul><li> `Eligible`для подходящего назначения</li><li> `Active`— Если он напрямую назначается `Active` администраторами или активирован в соответствии с подходящими пользователями.</li></ul>|
|Мембертипе|String      |Тип члена. Возможные значения: <ul><li>`Inherited`— назначение роли наследуется от родительской области ресурса</li><li>`Group`— назначение роли не наследуется, но поступает из группы назначения групп.</li><li>`User`— назначение роли не является ни унаследованным, ни назначением группы.</li></ul>|


## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Ресурс, связанный с назначением роли. |
|roleDefinition|[Говернанцероледефинитион](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, связанное с назначением роли. |
|subject|[Говернанцесубжект](../resources/governancesubject.md)|Только для чтения. Тема, связанная с назначением роли. |
|Линкеделигиблеролеассигнмент|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Только для чтения. Если он создан `active assignment` и создан в результате активации `eligible assignment`, он представляет объект этого `eligible assignment`объекта; В противном случае — `null`значение. |

## <a name="json-representation"></a>Представление в формате JSON

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
