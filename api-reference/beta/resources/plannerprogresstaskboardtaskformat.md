---
title: Тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "ход выполнения" доски задач (представление, организованное по состоянию поля PercentComplete в объекте Task со столбцами "не начато", "выполняется" и "завершено"). Каждой задаче будет назначен один объект **plannerProgressTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7be6483f127910224b05e05fdf885780d8767176
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521673"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="6d33f-104">Тип ресурса plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="6d33f-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="6d33f-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6d33f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d33f-106">Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "ход выполнения" доски задач (представление, организованное по состоянию поля PercentComplete в объекте Task со столбцами "не начато", "выполняется" и "завершено").</span><span class="sxs-lookup"><span data-stu-id="6d33f-106">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="6d33f-107">Каждой [задаче](plannertask.md) будет назначен один объект **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="6d33f-107">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="6d33f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6d33f-108">Methods</span></span>

| <span data-ttu-id="6d33f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6d33f-109">Method</span></span>           | <span data-ttu-id="6d33f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6d33f-110">Return Type</span></span>    |<span data-ttu-id="6d33f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6d33f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d33f-112">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="6d33f-112">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | <span data-ttu-id="6d33f-113">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).</span><span class="sxs-lookup"><span data-stu-id="6d33f-113">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)</span></span> |<span data-ttu-id="6d33f-114">Чтение свойств и связей объекта **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="6d33f-114">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|<span data-ttu-id="6d33f-115">[обновление](../api/plannerprogresstaskboardtaskformat-update.md).</span><span class="sxs-lookup"><span data-stu-id="6d33f-115">[Update](../api/plannerprogresstaskboardtaskformat-update.md)</span></span> | <span data-ttu-id="6d33f-116">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).</span><span class="sxs-lookup"><span data-stu-id="6d33f-116">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)</span></span>    |<span data-ttu-id="6d33f-117">Обновление объекта **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="6d33f-117">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6d33f-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d33f-118">Properties</span></span>
| <span data-ttu-id="6d33f-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d33f-119">Property</span></span>     | <span data-ttu-id="6d33f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6d33f-120">Type</span></span>   |<span data-ttu-id="6d33f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6d33f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d33f-122">id</span><span class="sxs-lookup"><span data-stu-id="6d33f-122">id</span></span>|<span data-ttu-id="6d33f-123">String</span><span class="sxs-lookup"><span data-stu-id="6d33f-123">String</span></span>| <span data-ttu-id="6d33f-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d33f-124">Read-only.</span></span> <span data-ttu-id="6d33f-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="6d33f-125">ID of the resource.</span></span> <span data-ttu-id="6d33f-126">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="6d33f-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="6d33f-127">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="6d33f-127">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6d33f-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="6d33f-128">orderHint</span></span>|<span data-ttu-id="6d33f-129">String</span><span class="sxs-lookup"><span data-stu-id="6d33f-129">String</span></span>|<span data-ttu-id="6d33f-p104">Указание, используемое для расположения задачи в окне "Ход выполнения" доски задач. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="6d33f-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d33f-132">Связи</span><span class="sxs-lookup"><span data-stu-id="6d33f-132">Relationships</span></span>
<span data-ttu-id="6d33f-133">Нет</span><span class="sxs-lookup"><span data-stu-id="6d33f-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6d33f-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d33f-134">JSON representation</span></span>
<span data-ttu-id="6d33f-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d33f-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
