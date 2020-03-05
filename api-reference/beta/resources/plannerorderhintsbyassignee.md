---
title: Тип ресурса Планнерордерхинтсбяссигни
description: '**Планнерордерхинтсбяссигни** — это ресурс, который содержит подсказки упорядочения для уполномоченные в ресурсе plannerTask, чтобы указать порядок задачи, назначенный для представления доски задач.'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3fc3e8a67e92091b5e273d45c483751c63dbbf0a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521722"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="0c7e6-103">Тип ресурса Планнерордерхинтсбяссигни</span><span class="sxs-lookup"><span data-stu-id="0c7e6-103">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="0c7e6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0c7e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c7e6-105">**Планнерордерхинтсбяссигни** — это ресурс, который содержит [подсказки упорядочения](planner-order-hint-format.md) для уполномоченные в ресурсе [plannerTask](plannertask.md) , чтобы указать порядок задачи, назначенный для представления доски задач.</span><span class="sxs-lookup"><span data-stu-id="0c7e6-105">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board.</span></span>
<span data-ttu-id="0c7e6-106">Этот тип является открытым типом.</span><span class="sxs-lookup"><span data-stu-id="0c7e6-106">This type is an open type.</span></span> <span data-ttu-id="0c7e6-107">Свойства — это идентификаторы пользователей, назначенных задаче, а значения — подсказки порядка.</span><span class="sxs-lookup"><span data-stu-id="0c7e6-107">The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="0c7e6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c7e6-108">Properties</span></span>
<span data-ttu-id="0c7e6-109">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="0c7e6-109">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="0c7e6-110">В этом случае клиент должен предоставить идентификаторы пользователей, назначенных задаче, в качестве имен свойств и допустимую [подсказку порядка](planner-order-hint-format.md) в качестве значения.</span><span class="sxs-lookup"><span data-stu-id="0c7e6-110">In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value.</span></span>
<span data-ttu-id="0c7e6-111">Невозможно удалить свойства из этого типа.</span><span class="sxs-lookup"><span data-stu-id="0c7e6-111">Properties cannot be removed from this type.</span></span> <span data-ttu-id="0c7e6-112">Служба автоматически удалит значения, так как назначения для содержащегося [plannerTask](plannertask.md) будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="0c7e6-112">The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="0c7e6-113">Пример.</span><span class="sxs-lookup"><span data-stu-id="0c7e6-113">Example:</span></span>

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
  "suppressions": []
}
-->
