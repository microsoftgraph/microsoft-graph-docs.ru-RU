---
title: Тип ресурса plannerAssignedToTaskBoardTaskFormat
description: Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении AssignedTo доски задач (представление, упорядоченное пользователями, которым назначены задачи). Каждой задаче будет назначен один объект **plannerAssignedToTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 000797631f5f15b0d9128e4433512e8451975255
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534032"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="eed70-104">Тип ресурса plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="eed70-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="eed70-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eed70-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eed70-106">Ресурс **plannerAssignedToTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении AssignedTo доски задач (представление, упорядоченное пользователями, которым назначены задачи).</span><span class="sxs-lookup"><span data-stu-id="eed70-106">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to).</span></span> <span data-ttu-id="eed70-107">Каждой [задаче](plannertask.md) будет назначен один объект **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="eed70-107">Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="eed70-108">Методы</span><span class="sxs-lookup"><span data-stu-id="eed70-108">Methods</span></span>

| <span data-ttu-id="eed70-109">Метод</span><span class="sxs-lookup"><span data-stu-id="eed70-109">Method</span></span>           | <span data-ttu-id="eed70-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eed70-110">Return Type</span></span>    |<span data-ttu-id="eed70-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eed70-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eed70-112">Получение объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="eed70-112">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | <span data-ttu-id="eed70-113">[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="eed70-113">[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)</span></span> |<span data-ttu-id="eed70-114">Чтение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="eed70-114">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="eed70-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="eed70-115">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | <span data-ttu-id="eed70-116">[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="eed70-116">[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)</span></span>  |<span data-ttu-id="eed70-117">Обновление объекта **plannerAssignedToTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="eed70-117">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eed70-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="eed70-118">Properties</span></span>
| <span data-ttu-id="eed70-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="eed70-119">Property</span></span>     | <span data-ttu-id="eed70-120">Тип</span><span class="sxs-lookup"><span data-stu-id="eed70-120">Type</span></span>   |<span data-ttu-id="eed70-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eed70-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eed70-122">id</span><span class="sxs-lookup"><span data-stu-id="eed70-122">id</span></span>|<span data-ttu-id="eed70-123">String</span><span class="sxs-lookup"><span data-stu-id="eed70-123">String</span></span>| <span data-ttu-id="eed70-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eed70-124">Read-only.</span></span> <span data-ttu-id="eed70-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="eed70-125">ID of the resource.</span></span> <span data-ttu-id="eed70-126">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="eed70-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="eed70-127">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="eed70-127">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="eed70-128">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="eed70-128">orderHintsByAssignee</span></span>|[<span data-ttu-id="eed70-129">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="eed70-129">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="eed70-p104">Словарь указаний, используемых для упорядочения задач в представлении AssignedTo доски задач. Ключ каждой записи — один из пользователей, которому назначена задача, а значение — указание порядка. Формат каждого значения описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="eed70-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="eed70-133">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="eed70-133">unassignedOrderHint</span></span>|<span data-ttu-id="eed70-134">Строка</span><span class="sxs-lookup"><span data-stu-id="eed70-134">String</span></span>|<span data-ttu-id="eed70-p105">Указание, используемое для расположения задачи в окне "Кому назначено" доски задач, когда задача никому не назначена, или если в словаре orderHintsByAssignee нет указания order для пользователя, которому назначена задача. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="eed70-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="eed70-137">Связи</span><span class="sxs-lookup"><span data-stu-id="eed70-137">Relationships</span></span>
<span data-ttu-id="eed70-138">Нет</span><span class="sxs-lookup"><span data-stu-id="eed70-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="eed70-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eed70-139">JSON representation</span></span>
<span data-ttu-id="eed70-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eed70-140">Here is a JSON representation of the resource.</span></span>

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
