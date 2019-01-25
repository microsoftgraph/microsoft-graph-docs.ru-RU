---
title: Тип ресурса plannerOrderHintsByAssignee
description: '**PlannerOrderHintsByAssignee** — это ресурс, который содержит упорядочения ссылки assignees в plannerTask ресурсов, чтобы указать порядок задач в представлении назначено панели задач.'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 27ef2c796c636e39ed6408c373cf0ac66c5572dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520909"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>Тип ресурса plannerOrderHintsByAssignee

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerOrderHintsByAssignee** — это ресурс, который содержит [указания в отношении порядка](planner-order-hint-format.md) расположения исполнителей задачи [plannerTask](plannertask.md) в представлении "Кому назначено" на доске задач. Это открытый тип. Свойства — это идентификаторы исполнителей, а значения — указания в отношении порядка расположения.

## <a name="properties"></a>Свойства
Свойства открытого типа может задавать клиент. Он должен указать идентификаторы исполнителей как имена свойств, а допустимое [указание в отношении порядка расположения](planner-order-hint-format.md) как значение. Свойства этого типа невозможно удалить. Служба будет автоматически удалять значения после обновления заданий в содержащем их объекте [plannerTask](plannertask.md).

Пример:

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerorderhintsbyassignee.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
