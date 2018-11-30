---
title: Тип ресурса plannerOrderHintsByAssignee
description: '**PlannerOrderHintsByAssignee** — это ресурс, который содержит упорядочения ссылки assignees в plannerTask ресурсов, чтобы указать порядок задач в представлении назначено панели задач.'
ms.openlocfilehash: b83abd3d3d08fc4d30f9f664af621bebad397b3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027032"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="42a0c-103">Тип ресурса plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="42a0c-103">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="42a0c-p101">**plannerOrderHintsByAssignee** — это ресурс, который содержит [указания в отношении порядка](planner-order-hint-format.md) расположения исполнителей задачи [plannerTask](plannertask.md) в представлении "Кому назначено" на доске задач. Это открытый тип. Свойства — это идентификаторы исполнителей, а значения — указания в отношении порядка расположения.</span><span class="sxs-lookup"><span data-stu-id="42a0c-p101">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="42a0c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="42a0c-107">Properties</span></span>
<span data-ttu-id="42a0c-p102">Свойства открытого типа может задавать клиент. Он должен указать идентификаторы исполнителей как имена свойств, а допустимое [указание в отношении порядка расположения](planner-order-hint-format.md) как значение. Свойства этого типа невозможно удалить. Служба будет автоматически удалять значения после обновления заданий в содержащем их объекте [plannerTask](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="42a0c-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="42a0c-112">Пример:</span><span class="sxs-lookup"><span data-stu-id="42a0c-112">Example:</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->