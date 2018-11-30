---
title: Тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом task связан один объект **plannerProgressTaskBoardTaskFormat**.
ms.openlocfilehash: 90ac4daa3d6b37f054c00df042de48d4c7706a96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027893"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="07e88-104">Тип ресурса plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="07e88-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="07e88-p102">Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом [task](plannertask.md) связан один объект **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="07e88-p102">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="07e88-107">Методы</span><span class="sxs-lookup"><span data-stu-id="07e88-107">Methods</span></span>

| <span data-ttu-id="07e88-108">Метод</span><span class="sxs-lookup"><span data-stu-id="07e88-108">Method</span></span>           | <span data-ttu-id="07e88-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="07e88-109">Return Type</span></span>    |<span data-ttu-id="07e88-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07e88-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07e88-111">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="07e88-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="07e88-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="07e88-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="07e88-113">Чтение свойств и отношений объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="07e88-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="07e88-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="07e88-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="07e88-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="07e88-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="07e88-116">Обновление объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="07e88-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="07e88-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="07e88-117">Properties</span></span>
| <span data-ttu-id="07e88-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="07e88-118">Property</span></span>     | <span data-ttu-id="07e88-119">Тип</span><span class="sxs-lookup"><span data-stu-id="07e88-119">Type</span></span>   |<span data-ttu-id="07e88-120">Описание</span><span class="sxs-lookup"><span data-stu-id="07e88-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07e88-121">id</span><span class="sxs-lookup"><span data-stu-id="07e88-121">id</span></span>|<span data-ttu-id="07e88-122">String</span><span class="sxs-lookup"><span data-stu-id="07e88-122">String</span></span>| <span data-ttu-id="07e88-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07e88-123">Read-only.</span></span> <span data-ttu-id="07e88-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="07e88-124">ID of the resource.</span></span> <span data-ttu-id="07e88-125">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="07e88-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="07e88-126">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="07e88-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="07e88-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="07e88-127">orderHint</span></span>|<span data-ttu-id="07e88-128">String</span><span class="sxs-lookup"><span data-stu-id="07e88-128">String</span></span>|<span data-ttu-id="07e88-p104">Указание, используемое для расположения задачи в представлении "Ход выполнения" на доске задач. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="07e88-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="07e88-131">Связи</span><span class="sxs-lookup"><span data-stu-id="07e88-131">Relationships</span></span>
<span data-ttu-id="07e88-132">Нет</span><span class="sxs-lookup"><span data-stu-id="07e88-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="07e88-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07e88-133">JSON representation</span></span>
<span data-ttu-id="07e88-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07e88-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->