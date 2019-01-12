---
title: Тип ресурса plannerAssignedToTaskBoardTaskFormat
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой задачей будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d59c8c45c998012cacdf4616f1e31f490bec5791
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973253"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="d3d15-104">Тип ресурса plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d3d15-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="d3d15-p102">Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой [задачей](plannertask.md) будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d3d15-p102">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="d3d15-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d3d15-107">Methods</span></span>

| <span data-ttu-id="d3d15-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d3d15-108">Method</span></span>           | <span data-ttu-id="d3d15-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d3d15-109">Return Type</span></span>    |<span data-ttu-id="d3d15-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d15-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3d15-111">Получение plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d3d15-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="d3d15-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d3d15-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="d3d15-113">Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d3d15-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="d3d15-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="d3d15-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="d3d15-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d3d15-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="d3d15-116">Обновление объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d3d15-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d3d15-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3d15-117">Properties</span></span>
| <span data-ttu-id="d3d15-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3d15-118">Property</span></span>     | <span data-ttu-id="d3d15-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d3d15-119">Type</span></span>   |<span data-ttu-id="d3d15-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d15-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3d15-121">id</span><span class="sxs-lookup"><span data-stu-id="d3d15-121">id</span></span>|<span data-ttu-id="d3d15-122">String</span><span class="sxs-lookup"><span data-stu-id="d3d15-122">String</span></span>| <span data-ttu-id="d3d15-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d3d15-123">Read-only.</span></span> <span data-ttu-id="d3d15-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="d3d15-124">ID of the resource.</span></span> <span data-ttu-id="d3d15-125">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="d3d15-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d3d15-126">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="d3d15-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d3d15-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d3d15-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="d3d15-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d3d15-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="d3d15-p104">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d3d15-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="d3d15-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="d3d15-132">unassignedOrderHint</span></span>|<span data-ttu-id="d3d15-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d3d15-133">String</span></span>|<span data-ttu-id="d3d15-p105">Значение указания, используемое для упорядочения задач в представлении AssignedTo доски задач, когда задача не назначена ни одному пользователю либо когда в словаре orderHintsByAssignee нет указания порядка для пользователя, которому назначена задача. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d3d15-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3d15-136">Связи</span><span class="sxs-lookup"><span data-stu-id="d3d15-136">Relationships</span></span>
<span data-ttu-id="d3d15-137">Нет</span><span class="sxs-lookup"><span data-stu-id="d3d15-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d3d15-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3d15-138">JSON representation</span></span>
<span data-ttu-id="d3d15-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3d15-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
