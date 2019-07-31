---
title: Тип ресурса plannerAssignedToTaskBoardTaskFormat
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении AssignedTo доски задач (представление, упорядоченное пользователями, которым назначены задачи). Каждой задаче будет назначен один объект **plannerAssignedToTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a67f085b5e6a7984e1b73358defb28c783d2ec10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009141"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="5849c-104">Тип ресурса plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5849c-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5849c-105">Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении AssignedTo доски задач (представление, упорядоченное пользователями, которым назначены задачи).</span><span class="sxs-lookup"><span data-stu-id="5849c-105">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to).</span></span> <span data-ttu-id="5849c-106">Каждой [задаче](plannertask.md) будет назначен один объект **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="5849c-106">Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="5849c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5849c-107">Methods</span></span>

| <span data-ttu-id="5849c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5849c-108">Method</span></span>           | <span data-ttu-id="5849c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5849c-109">Return Type</span></span>    |<span data-ttu-id="5849c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5849c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5849c-111">Получение объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5849c-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | <span data-ttu-id="5849c-112">[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="5849c-112">[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)</span></span> |<span data-ttu-id="5849c-113">Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="5849c-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|<span data-ttu-id="5849c-114">[обновление](../api/plannerassignedtotaskboardtaskformat-update.md);</span><span class="sxs-lookup"><span data-stu-id="5849c-114">[Update](../api/plannerassignedtotaskboardtaskformat-update.md)</span></span> | <span data-ttu-id="5849c-115">[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="5849c-115">[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)</span></span>  |<span data-ttu-id="5849c-116">Обновление объекта **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="5849c-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5849c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5849c-117">Properties</span></span>
| <span data-ttu-id="5849c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5849c-118">Property</span></span>     | <span data-ttu-id="5849c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5849c-119">Type</span></span>   |<span data-ttu-id="5849c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5849c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5849c-121">id</span><span class="sxs-lookup"><span data-stu-id="5849c-121">id</span></span>|<span data-ttu-id="5849c-122">String</span><span class="sxs-lookup"><span data-stu-id="5849c-122">String</span></span>| <span data-ttu-id="5849c-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5849c-123">Read-only.</span></span> <span data-ttu-id="5849c-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="5849c-124">ID of the resource.</span></span> <span data-ttu-id="5849c-125">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5849c-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5849c-126">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="5849c-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5849c-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="5849c-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="5849c-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="5849c-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="5849c-p104">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="5849c-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5849c-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="5849c-132">unassignedOrderHint</span></span>|<span data-ttu-id="5849c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5849c-133">String</span></span>|<span data-ttu-id="5849c-p105">Указание, используемое для расположения задачи в окне "Кому назначено" доски задач, когда задача никому не назначена, или если в словаре orderHintsByAssignee нет указания order для пользователя, которому назначена задача. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="5849c-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5849c-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="5849c-136">Relationships</span></span>
<span data-ttu-id="5849c-137">Нет</span><span class="sxs-lookup"><span data-stu-id="5849c-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5849c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5849c-138">JSON representation</span></span>
<span data-ttu-id="5849c-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5849c-139">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
