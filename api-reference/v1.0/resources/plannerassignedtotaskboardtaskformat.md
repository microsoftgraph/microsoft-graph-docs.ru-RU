---
title: Тип ресурса plannerAssignedToTaskBoardTaskFormat
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой задачей будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
ms.openlocfilehash: 0eee2ffaa08cb227ee1b9fa5fdab129d33ddd2ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846069"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="3a518-104">Тип ресурса plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3a518-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="3a518-p102">Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении AssignedTo на доске задач (представление, упорядоченное по пользователям, которым назначены задачи). C каждой [задачей](plannertask.md) будет сопоставлен один объект **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="3a518-p102">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="3a518-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3a518-107">Methods</span></span>

| <span data-ttu-id="3a518-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3a518-108">Method</span></span>           | <span data-ttu-id="3a518-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3a518-109">Return Type</span></span>    |<span data-ttu-id="3a518-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3a518-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3a518-111">Получение plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3a518-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="3a518-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3a518-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="3a518-113">Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="3a518-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="3a518-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="3a518-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="3a518-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="3a518-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="3a518-116">Обновление объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="3a518-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3a518-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a518-117">Properties</span></span>
| <span data-ttu-id="3a518-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a518-118">Property</span></span>     | <span data-ttu-id="3a518-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3a518-119">Type</span></span>   |<span data-ttu-id="3a518-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3a518-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a518-121">id</span><span class="sxs-lookup"><span data-stu-id="3a518-121">id</span></span>|<span data-ttu-id="3a518-122">Строка</span><span class="sxs-lookup"><span data-stu-id="3a518-122">String</span></span>| <span data-ttu-id="3a518-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3a518-123">Read-only.</span></span> <span data-ttu-id="3a518-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="3a518-124">ID of the resource.</span></span> <span data-ttu-id="3a518-125">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="3a518-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="3a518-126">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="3a518-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="3a518-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="3a518-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="3a518-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="3a518-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="3a518-p104">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="3a518-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="3a518-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="3a518-132">unassignedOrderHint</span></span>|<span data-ttu-id="3a518-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3a518-133">String</span></span>|<span data-ttu-id="3a518-p105">Значение указания, используемое для упорядочения задач в представлении AssignedTo доски задач, когда задача не назначена ни одному пользователю либо когда в словаре orderHintsByAssignee нет указания порядка для пользователя, которому назначена задача. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="3a518-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a518-136">Связи</span><span class="sxs-lookup"><span data-stu-id="3a518-136">Relationships</span></span>
<span data-ttu-id="3a518-137">Нет</span><span class="sxs-lookup"><span data-stu-id="3a518-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3a518-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a518-138">JSON representation</span></span>
<span data-ttu-id="3a518-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a518-139">Here is a JSON representation of the resource.</span></span>

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
