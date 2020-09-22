---
title: Тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "ход выполнения" доски задач (представление, организованное по состоянию поля PercentComplete в объекте Task со столбцами "не начато", "выполняется" и "завершено"). Каждой задаче будет назначен один объект **plannerProgressTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e52f98f6e84b39550288f49f9115bc3063556522
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064068"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="025a2-104">Тип ресурса plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="025a2-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="025a2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="025a2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="025a2-106">Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "ход выполнения" доски задач (представление, организованное по состоянию поля PercentComplete в объекте Task со столбцами "не начато", "выполняется" и "завершено").</span><span class="sxs-lookup"><span data-stu-id="025a2-106">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="025a2-107">Каждой [задаче](plannertask.md) будет назначен один объект **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="025a2-107">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="025a2-108">Методы</span><span class="sxs-lookup"><span data-stu-id="025a2-108">Methods</span></span>

| <span data-ttu-id="025a2-109">Метод</span><span class="sxs-lookup"><span data-stu-id="025a2-109">Method</span></span>           | <span data-ttu-id="025a2-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="025a2-110">Return Type</span></span>    |<span data-ttu-id="025a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="025a2-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="025a2-112">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="025a2-112">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | <span data-ttu-id="025a2-113">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).</span><span class="sxs-lookup"><span data-stu-id="025a2-113">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)</span></span> |<span data-ttu-id="025a2-114">Чтение свойств и связей объекта **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="025a2-114">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="025a2-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="025a2-115">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | <span data-ttu-id="025a2-116">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).</span><span class="sxs-lookup"><span data-stu-id="025a2-116">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)</span></span>    |<span data-ttu-id="025a2-117">Обновление объекта **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="025a2-117">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="025a2-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="025a2-118">Properties</span></span>
| <span data-ttu-id="025a2-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="025a2-119">Property</span></span>     | <span data-ttu-id="025a2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="025a2-120">Type</span></span>   |<span data-ttu-id="025a2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="025a2-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="025a2-122">id</span><span class="sxs-lookup"><span data-stu-id="025a2-122">id</span></span>|<span data-ttu-id="025a2-123">String</span><span class="sxs-lookup"><span data-stu-id="025a2-123">String</span></span>| <span data-ttu-id="025a2-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="025a2-124">Read-only.</span></span> <span data-ttu-id="025a2-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="025a2-125">ID of the resource.</span></span> <span data-ttu-id="025a2-126">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="025a2-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="025a2-127">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="025a2-127">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="025a2-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="025a2-128">orderHint</span></span>|<span data-ttu-id="025a2-129">String</span><span class="sxs-lookup"><span data-stu-id="025a2-129">String</span></span>|<span data-ttu-id="025a2-p104">Указание, используемое для расположения задачи в окне "Ход выполнения" доски задач. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="025a2-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="025a2-132">Связи</span><span class="sxs-lookup"><span data-stu-id="025a2-132">Relationships</span></span>
<span data-ttu-id="025a2-133">Нет</span><span class="sxs-lookup"><span data-stu-id="025a2-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="025a2-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="025a2-134">JSON representation</span></span>
<span data-ttu-id="025a2-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="025a2-135">Here is a JSON representation of the resource.</span></span>

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


