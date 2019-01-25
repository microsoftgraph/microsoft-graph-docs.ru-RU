---
title: Тип ресурса plannerTask
description: Ресурс **plannerTask** представляет задачу планировщика в Office 365. Задача планировщика содержится в плане и может быть назначена сегменту в плане. Каждый объект задачи имеет объект details, который может содержать дополнительные сведения о задаче. Дополнительные сведения об отношениях между группой, планом и задачей см. в этом обзоре.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2313b31e0a962f27fa728af8c8953b646210397a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511214"
---
# <a name="plannertask-resource-type"></a>Тип ресурса plannerTask

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerTask** представляет задачу планировщика в Office 365. Задача планировщика содержится в [плане](plannerplan.md) и может быть назначена [сегменту](plannerbucket.md) в плане. Каждый объект задачи имеет объект [details](plannertaskdetails.md), который может содержать дополнительные сведения о задаче. Дополнительные сведения об отношениях между группой, планом и задачей см. в [этом обзоре](planner-overview.md).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerTask](../api/plannertask-get.md) | [plannerTask](plannertask.md); |Чтение свойств и отношений объекта **plannerTask**.|
|[Обновление](../api/plannertask-update.md) | [plannerTask](plannertask.md) |Обновление объекта **plannerTask**. |
|[Удаление](../api/plannertask-delete.md) | Нет |Удаление объекта **plannerTask**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|activeChecklistItemCount|Int32|Количество элементов контрольного списка со значением false, указывающим, что задача не выполнена.|
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|Категории, к которым применена задача. Возможные значения см. [здесь](plannerappliedcategories.md).|
|assigneePriority|String|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).|
|assignments|[plannerAssignments](plannerassignments.md)|Список исполнителей, которым назначена задача.|
|bucketId|String|КОД сегмента, к которой принадлежит задачи. Должен быть в плане, задача находится в сегменте. Это 28 знаков без учета регистра. [Формат](tasks-identifiers-disclaimer.md) проверяются на службу. |
|checklistItemCount|Int32|Количество элементов контрольного списка, представленных в задаче.|
|completedBy|[identitySet](identityset.md)|Идентификатор пользователя, который выполнил задачу.|
|completedDateTime|DateTimeOffset|Только для чтения. Дата и время присвоения свойству задачи `'percentComplete'` значения `'100'`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`|
|conversationThreadId|String|Идентификатор разговора о задаче. Это идентификатор объекта разговора, созданного в группе.|
|createdBy|[identitySet](identityset.md)|Идентификатор пользователя, создавшего задачу.|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|dueDateTime|DateTimeOffset|Срок выполнения задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|hasDescription|Логический|Только для чтения. Значение — `true`, если объект details задачи имеет описание. В противном случае — `false`.|
|id|String|Только для чтения. Идентификатор задачи. Это 28 знаков без учета регистра. [Формат](tasks-identifiers-disclaimer.md) проверяются на службу.|
|orderHint|String|Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).|
|percentComplete|Int32|Процент выполнения задачи. Если установлено значение `100`, задача считается выполненной. |
|planId|String|Идентификатор плана, к которому относится задача.|
|previewType|строка|Устанавливает тип предварительного просмотра задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|referenceCount|Int32|Количество внешних ссылок на задачу.|
|startDateTime|DateTimeOffset|Дата и время начала задачи. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|title|String|Название задачи.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)| Только для чтения. Допускает значение null. Используется для правильного отображения задачи на доске задач при сортировке по свойству assignedTo.|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)| Только для чтения. Допускает значение null. Используется для правильного отображения задачи на доске задач при сортировке по сегменту.|
|details|[plannerTaskDetails](plannertaskdetails.md)| Только для чтения. Допускает значение null. Дополнительные сведения о задаче.|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)| Только для чтения. Допускает значение null. Используется для правильного отображения задачи на доске задач при сортировке по ходу выполнения.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": 1024,
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": 1024,
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": 1024,
  "planId": "String",
  "previewType": "string",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertask.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
