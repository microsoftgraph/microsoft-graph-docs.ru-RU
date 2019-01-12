---
title: Тип ресурса plannerAssignedToTaskBoardTaskFormat
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой задачей будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e86517f2b90cf1c76ca975b3a31a8766b7e86bd7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955795"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="f64ed-104">Тип ресурса plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f64ed-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="f64ed-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f64ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f64ed-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f64ed-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f64ed-p103">Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой [задачей](plannertask.md) будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="f64ed-p103">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="f64ed-109">Методы</span><span class="sxs-lookup"><span data-stu-id="f64ed-109">Methods</span></span>

| <span data-ttu-id="f64ed-110">Метод</span><span class="sxs-lookup"><span data-stu-id="f64ed-110">Method</span></span>           | <span data-ttu-id="f64ed-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f64ed-111">Return Type</span></span>    |<span data-ttu-id="f64ed-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f64ed-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f64ed-113">Получение plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f64ed-113">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="f64ed-114">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f64ed-114">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="f64ed-115">Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="f64ed-115">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="f64ed-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="f64ed-116">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="f64ed-117">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="f64ed-117">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="f64ed-118">Обновление объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="f64ed-118">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f64ed-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f64ed-119">Properties</span></span>
| <span data-ttu-id="f64ed-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f64ed-120">Property</span></span>     | <span data-ttu-id="f64ed-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f64ed-121">Type</span></span>   |<span data-ttu-id="f64ed-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f64ed-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f64ed-123">id</span><span class="sxs-lookup"><span data-stu-id="f64ed-123">id</span></span>|<span data-ttu-id="f64ed-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f64ed-124">String</span></span>| <span data-ttu-id="f64ed-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f64ed-125">Read-only.</span></span> <span data-ttu-id="f64ed-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="f64ed-126">ID of the resource.</span></span> <span data-ttu-id="f64ed-127">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="f64ed-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="f64ed-128">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="f64ed-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="f64ed-129">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="f64ed-129">orderHintsByAssignee</span></span>|[<span data-ttu-id="f64ed-130">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="f64ed-130">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="f64ed-p105">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="f64ed-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="f64ed-134">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="f64ed-134">unassignedOrderHint</span></span>|<span data-ttu-id="f64ed-135">Строка</span><span class="sxs-lookup"><span data-stu-id="f64ed-135">String</span></span>|<span data-ttu-id="f64ed-p106">Значение указания, используемое для упорядочения задач в представлении AssignedTo доски задач, когда задача не назначена ни одному пользователю либо когда в словаре orderHintsByAssignee нет указания порядка для пользователя, которому назначена задача. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="f64ed-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f64ed-138">Связи</span><span class="sxs-lookup"><span data-stu-id="f64ed-138">Relationships</span></span>
<span data-ttu-id="f64ed-139">Нет</span><span class="sxs-lookup"><span data-stu-id="f64ed-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f64ed-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f64ed-140">JSON representation</span></span>
<span data-ttu-id="f64ed-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f64ed-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
