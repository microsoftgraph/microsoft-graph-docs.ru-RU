---
title: Тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для правильного отображения задачи в представлении "ход выполнения" доски задач (представление, организованное по состоянию поля PercentComplete в объекте Task со столбцами для Not started , Выполняется и завершено). Каждой задаче будет назначен один объект **plannerProgressTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ea1382d454a2167df40a37f0da7dbe9b08f867f1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344386"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="30513-104">Тип ресурса plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="30513-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30513-105">Ресурс **plannerProgressTaskBoardTaskFormat** представляет сведения, используемые для правильного отображения задачи в представлении "ход выполнения" доски задач (представление, организованное по состоянию поля PercentComplete в объекте Task со столбцами для Not started , Выполняется и завершено).</span><span class="sxs-lookup"><span data-stu-id="30513-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="30513-106">Каждой [задаче](plannertask.md) будет назначен один объект **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="30513-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="30513-107">Методы</span><span class="sxs-lookup"><span data-stu-id="30513-107">Methods</span></span>

| <span data-ttu-id="30513-108">Метод</span><span class="sxs-lookup"><span data-stu-id="30513-108">Method</span></span>           | <span data-ttu-id="30513-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="30513-109">Return Type</span></span>    |<span data-ttu-id="30513-110">Описание</span><span class="sxs-lookup"><span data-stu-id="30513-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30513-111">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="30513-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | <span data-ttu-id="30513-112">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).</span><span class="sxs-lookup"><span data-stu-id="30513-112">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)</span></span> |<span data-ttu-id="30513-113">Чтение свойств и связей объекта **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="30513-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="30513-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="30513-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | <span data-ttu-id="30513-115">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).</span><span class="sxs-lookup"><span data-stu-id="30513-115">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)</span></span>    |<span data-ttu-id="30513-116">Обновление объекта **plannerProgressTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="30513-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="30513-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="30513-117">Properties</span></span>
| <span data-ttu-id="30513-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="30513-118">Property</span></span>     | <span data-ttu-id="30513-119">Тип</span><span class="sxs-lookup"><span data-stu-id="30513-119">Type</span></span>   |<span data-ttu-id="30513-120">Описание</span><span class="sxs-lookup"><span data-stu-id="30513-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30513-121">id</span><span class="sxs-lookup"><span data-stu-id="30513-121">id</span></span>|<span data-ttu-id="30513-122">String</span><span class="sxs-lookup"><span data-stu-id="30513-122">String</span></span>| <span data-ttu-id="30513-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30513-123">Read-only.</span></span> <span data-ttu-id="30513-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="30513-124">ID of the resource.</span></span> <span data-ttu-id="30513-125">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="30513-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="30513-126">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="30513-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="30513-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="30513-127">orderHint</span></span>|<span data-ttu-id="30513-128">String</span><span class="sxs-lookup"><span data-stu-id="30513-128">String</span></span>|<span data-ttu-id="30513-p104">Указание, используемое для расположения задачи в окне "Ход выполнения" доски задач. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="30513-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="30513-131">Связи</span><span class="sxs-lookup"><span data-stu-id="30513-131">Relationships</span></span>
<span data-ttu-id="30513-132">Нет</span><span class="sxs-lookup"><span data-stu-id="30513-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="30513-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30513-133">JSON representation</span></span>
<span data-ttu-id="30513-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30513-134">Here is a JSON representation of the resource.</span></span>

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
