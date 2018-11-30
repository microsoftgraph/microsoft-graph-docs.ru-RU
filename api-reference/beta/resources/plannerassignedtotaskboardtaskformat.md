---
title: Тип ресурса plannerAssignedToTaskBoardTaskFormat
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой задачей будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.
ms.openlocfilehash: 8fc96d6fa7d4f05f6bc81f7030ebe766bf769e40
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078958"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="d41bf-104">Тип ресурса plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d41bf-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="d41bf-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d41bf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d41bf-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d41bf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d41bf-p103">Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой [задачей](plannertask.md) будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d41bf-p103">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="d41bf-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d41bf-109">Methods</span></span>

| <span data-ttu-id="d41bf-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d41bf-110">Method</span></span>           | <span data-ttu-id="d41bf-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d41bf-111">Return Type</span></span>    |<span data-ttu-id="d41bf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d41bf-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d41bf-113">Получение plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d41bf-113">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="d41bf-114">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d41bf-114">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="d41bf-115">Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d41bf-115">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="d41bf-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="d41bf-116">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="d41bf-117">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="d41bf-117">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="d41bf-118">Обновление объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="d41bf-118">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d41bf-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="d41bf-119">Properties</span></span>
| <span data-ttu-id="d41bf-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="d41bf-120">Property</span></span>     | <span data-ttu-id="d41bf-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d41bf-121">Type</span></span>   |<span data-ttu-id="d41bf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d41bf-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d41bf-123">id</span><span class="sxs-lookup"><span data-stu-id="d41bf-123">id</span></span>|<span data-ttu-id="d41bf-124">String</span><span class="sxs-lookup"><span data-stu-id="d41bf-124">String</span></span>| <span data-ttu-id="d41bf-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41bf-125">Read-only.</span></span> <span data-ttu-id="d41bf-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="d41bf-126">ID of the resource.</span></span> <span data-ttu-id="d41bf-127">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="d41bf-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d41bf-128">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="d41bf-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d41bf-129">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d41bf-129">orderHintsByAssignee</span></span>|[<span data-ttu-id="d41bf-130">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="d41bf-130">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="d41bf-p105">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d41bf-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="d41bf-134">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="d41bf-134">unassignedOrderHint</span></span>|<span data-ttu-id="d41bf-135">Строка</span><span class="sxs-lookup"><span data-stu-id="d41bf-135">String</span></span>|<span data-ttu-id="d41bf-p106">Значение указания, используемое для упорядочения задач в представлении AssignedTo доски задач, когда задача не назначена ни одному пользователю либо когда в словаре orderHintsByAssignee нет указания порядка для пользователя, которому назначена задача. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d41bf-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d41bf-138">Связи</span><span class="sxs-lookup"><span data-stu-id="d41bf-138">Relationships</span></span>
<span data-ttu-id="d41bf-139">Нет</span><span class="sxs-lookup"><span data-stu-id="d41bf-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d41bf-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d41bf-140">JSON representation</span></span>
<span data-ttu-id="d41bf-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d41bf-141">Here is a JSON representation of the resource.</span></span>

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