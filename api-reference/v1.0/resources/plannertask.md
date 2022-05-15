---
title: Тип ресурса plannerTask
description: Ресурс **plannerTask** представляет задачу планировщика в Microsoft 365. Задача планировщика содержится в плане и может быть назначена сегменту в плане. Каждый объект задачи имеет объект details, который может содержать дополнительные сведения о ней. Дополнительную информацию об отношениях между группой, планом и задачей см. в обзоре.
ms.localizationpriority: high
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 079170c91bfa754f1f36dbef1404b7c92c0d1602
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420651"
---
# <a name="plannertask-resource-type"></a>Тип ресурса plannerTask

Пространство имен: microsoft.graph

Ресурс **plannerTask** представляет задачу планировщика в Microsoft 365. Задача планировщика содержится в [плане](plannerplan.md) и может быть назначена [сегменту](plannerbucket.md) в плане. Каждый объект задачи имеет объект [details](plannertaskdetails.md), который может содержать дополнительные сведения о ней. Дополнительную информацию об отношениях между группой, планом и задачей см. в [этом обзоре](planner-overview.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerTask](../api/plannertask-get.md) | [plannerTask](plannertask.md) |Чтение свойств и отношений объекта **plannerTask**.|
|[Обновление](../api/plannertask-update.md) | [plannerTask](plannertask.md) |Обновление объекта **plannerTask**. |
|[Удаление](../api/plannertask-delete.md) | Нет |Удаление объекта **plannerTask**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|activeChecklistItemCount|Int32|Количество элементов контрольного списка со значением `false`, указывающим, что задача не выполнена.|
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|Категории, к которым применена задача. Возможные значения см. [здесь](plannerappliedcategories.md).|
|assigneePriority|String|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).|
|assignments|[plannerAssignments](plannerassignments.md)|Список исполнителей, которым назначена задача.|
|bucketId|Строка|Идентификатор сегмента, к которому относится задача. Сегмент должен находиться в том же плане, что и задача. Идентификатор состоит из 28 символов и чувствителен к регистру. [Проверка формата](planner-identifiers-disclaimer.md) выполняется на службе. |
|checklistItemCount|Int32|Количество элементов контрольного списка, представленных в задаче.|
|completedBy|[identitySet](identityset.md)|Идентификатор пользователя, который выполнил задачу.|
|completedDateTime|DateTimeOffset|Только для чтения. Дата и время присвоения свойству задачи `'percentComplete'` значения `'100'`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`|
|conversationThreadId|Строка|Идентификатор разговора о задаче. Это идентификатор объекта разговора, созданного в группе.|
|createdBy|[identitySet](identityset.md)|Идентификатор пользователя, создавшего задачу.|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|dueDateTime|DateTimeOffset|Срок выполнения задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|hasDescription|Boolean|Только для чтения. Значение — `true`, если объект details задачи имеет описание. В противном случае — `false`.|
|id|String|Только для чтения. Идентификатор задачи. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.|
|orderHint|String|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).|
|percentComplete|Int32|Процент выполнения задачи. Если установлено значение `100`, задача считается выполненной. |
|priority|Int32|Приоритет задачи. Допустимый диапазон значений находится между `0` и `10`, при этом возрастающее значение имеет более низкий приоритет (`0` имеет самый высокий приоритет, а `10` имеет самый низкий приоритет).  В настоящее время Планировщик интерпретирует значения `0` и `1`как "срочно", `2`,`3` и `4` как "важно", `5`,`6` и `7` как "средние", а `8`,`9` и `10` как "низкие".  Кроме того, Планировщик задает значение `1` для "срочно", `3` для "важно", `5` для "средний" и `9` для "низкий".|
|planId|Строка|Идентификатор плана, к которому относится задача.|
|previewType|String|Устанавливает тип предварительного просмотра задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|referenceCount|Int32|Количество внешних ссылок на задачу.|
|startDateTime|DateTimeOffset|Дата и время начала выполнения задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|title|Строка|Название задачи.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md);| Только для чтения. Допускает значение null. Используется для правильного отображения задачи на доске задач при сортировке по свойству assignedTo.|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);| Только для чтения. Допускает значение null. Используется для правильного отображения задачи на доске задач при сортировке по сегменту.|
|подробности|[plannerTaskDetails](plannertaskdetails.md);| Только для чтения. Допускает значение null. Дополнительные сведения о задаче.|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).| Только для чтения. Допускает значение null. Используется для правильного отображения задачи на доске задач при сортировке по ходу выполнения.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": "Int32",
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": "Int32",
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": "Int32",
  "priority": "Int32",
  "planId": "String",
  "previewType": "String",
  "referenceCount": "Int32",
  "startDateTime": "String (timestamp)",
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

