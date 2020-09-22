---
title: Тип ресурса Планнерордерхинтсбяссигни
description: '**Планнерордерхинтсбяссигни** — это ресурс, который содержит подсказки упорядочения для уполномоченные в ресурсе plannerTask, чтобы указать порядок задачи, назначенный для представления доски задач.'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e083f171b777b3223d698530b64539c86bb15139
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037474"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="61088-103">Тип ресурса Планнерордерхинтсбяссигни</span><span class="sxs-lookup"><span data-stu-id="61088-103">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="61088-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61088-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61088-105">**Планнерордерхинтсбяссигни** — это ресурс, который содержит [подсказки упорядочения](planner-order-hint-format.md) для уполномоченные в ресурсе [plannerTask](plannertask.md) , чтобы указать порядок задачи, назначенный для представления доски задач.</span><span class="sxs-lookup"><span data-stu-id="61088-105">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board.</span></span>
<span data-ttu-id="61088-106">Этот тип является открытым типом.</span><span class="sxs-lookup"><span data-stu-id="61088-106">This type is an open type.</span></span> <span data-ttu-id="61088-107">Свойства — это идентификаторы пользователей, назначенных задаче, а значения — подсказки порядка.</span><span class="sxs-lookup"><span data-stu-id="61088-107">The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="61088-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="61088-108">Properties</span></span>
<span data-ttu-id="61088-109">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="61088-109">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="61088-110">В этом случае клиент должен предоставить идентификаторы пользователей, назначенных задаче, в качестве имен свойств и допустимую [подсказку порядка](planner-order-hint-format.md) в качестве значения.</span><span class="sxs-lookup"><span data-stu-id="61088-110">In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value.</span></span>
<span data-ttu-id="61088-111">Невозможно удалить свойства из этого типа.</span><span class="sxs-lookup"><span data-stu-id="61088-111">Properties cannot be removed from this type.</span></span> <span data-ttu-id="61088-112">Служба автоматически удалит значения, так как назначения для содержащегося [plannerTask](plannertask.md) будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="61088-112">The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="61088-113">Пример:</span><span class="sxs-lookup"><span data-stu-id="61088-113">Example:</span></span>

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

