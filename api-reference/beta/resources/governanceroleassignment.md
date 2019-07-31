---
title: Тип ресурса governanceRoleAssignment
description: Представляет назначение роли пользователю или группе.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 518fbe18fcd09b1b4cc9730c6b7f0112adabfeae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971895"
---
# <a name="governanceroleassignment-resource-type"></a>Тип ресурса governanceRoleAssignment
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначение роли пользователю или группе.

Привилегированное управление удостоверениями (PIM) поддерживает два типа назначений:

1. Активное назначение — представляет прямой/активированный доступ к ресурсам.
2. Подходящие назначения — представляет промежуточный этап привилегированного доступа к ресурсам, между отсутствием доступа и прямым доступом. Администраторы могут заранее назначать пользователей и группы `eligible assignment` , а при необходимости `activation` `eligible assignment` получить доступ к ресурсу в течение нескольких часов. После активации `active assignment` будет создана группа для пользователей и членов группы, указывающая состояние активации.

## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:------------|:--------|:--------|
|[Получение](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Чтение свойств и связей объекта назначения роли.|
|[List](../api/governanceroleassignment-list.md) | Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)|Перечисление коллекции назначений ролей для ресурса. |
|[Экспорт](../api/governanceroleassignment-export.md) | поток в октетах |Скачайте коллекцию назначений ролей для ресурса и сохраните ее `.csv` в виде файла.|

`PUT` `POST` `roleAssignments` В наборе сущностей `DELETE` поддерживаются не поддерживаемые операции, а также операции. `PATCH` Все операции по `governanceRoleAssignment` созданию, обновлению и удалению выполняются `governanceRoleAssignmentRequest`.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |Строка     |Идентификатор назначения роли. Он указан в формате GUID.|
|resourceId |String     |Обязательный. Идентификатор ресурса, с которым связано назначение роли. |
|Роледефинитионид|String|Обязательный. Идентификатор определения роли, с которым связано назначение роли. |
|Субжектид|String       |Обязательный. ИДЕНТИФИКАТОР субъекта, с которым связано назначение роли. |
|Линкеделигиблеролеассигнментид|String|Если он создан `active assignment` и создан в результате активации `eligible assignment`, он представляет идентификатор этого `eligible assignment`объекта; В противном случае — `null`значение. |
|externalId   |String     |Внешний идентификатор — ресурс, который используется для идентификации назначения роли в поставщике.|
|startDateTime|DateTimeOffset|Время начала назначения роли. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|endDateTime|DateTimeOffset|Для назначения непостоянных ролей это время истечения срока действия назначения роли. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Ассигнментстате|String  |Состояние назначения. Значение может быть <ul><li> `Eligible`для подходящего назначения</li><li> `Active`— Если он напрямую назначается `Active` администраторами или активирован в соответствии с подходящими пользователями.</li></ul>|
|Мембертипе|String      |Тип члена. Возможные значения: <ul><li>`Inherited`— назначение роли наследуется от родительской области ресурса</li><li>`Group`— назначение роли не наследуется, но поступает из группы назначения групп.</li><li>`User`— назначение роли не является ни унаследованным, ни назначением группы.</li></ul>|


## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Ресурс, связанный с назначением роли. |
|roleDefinition|[Говернанцероледефинитион](../resources/governanceroledefinition.md)|Только для чтения. Определение роли, связанное с назначением роли. |
|subject|[Говернанцесубжект](../resources/governancesubject.md)|Только для чтения. Тема, связанная с назначением роли. |
|Линкеделигиблеролеассигнмент|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Только для чтения. Если он создан `active assignment` и создан в результате активации `eligible assignment`, он представляет объект этого `eligible assignment`объекта; В противном случае — `null`значение. |

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
