---
title: Тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом task связан один объект **plannerProgressTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 58e1b80c61dcb0c58996f65c1fa03c48c4edafbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955928"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="1b5a7-104">Тип ресурса plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1b5a7-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="1b5a7-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b5a7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b5a7-p103">Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом [task](plannertask.md) связан один объект **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-p103">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="1b5a7-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1b5a7-109">Methods</span></span>

| <span data-ttu-id="1b5a7-110">Метод</span><span class="sxs-lookup"><span data-stu-id="1b5a7-110">Method</span></span>           | <span data-ttu-id="1b5a7-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1b5a7-111">Return Type</span></span>    |<span data-ttu-id="1b5a7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1b5a7-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b5a7-113">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1b5a7-113">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="1b5a7-114">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1b5a7-114">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="1b5a7-115">Чтение свойств и отношений объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-115">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="1b5a7-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="1b5a7-116">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="1b5a7-117">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1b5a7-117">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="1b5a7-118">Обновление объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-118">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b5a7-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b5a7-119">Properties</span></span>
| <span data-ttu-id="1b5a7-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b5a7-120">Property</span></span>     | <span data-ttu-id="1b5a7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1b5a7-121">Type</span></span>   |<span data-ttu-id="1b5a7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1b5a7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b5a7-123">id</span><span class="sxs-lookup"><span data-stu-id="1b5a7-123">id</span></span>|<span data-ttu-id="1b5a7-124">Строка</span><span class="sxs-lookup"><span data-stu-id="1b5a7-124">String</span></span>| <span data-ttu-id="1b5a7-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-125">Read-only.</span></span> <span data-ttu-id="1b5a7-126">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-126">ID of the resource.</span></span> <span data-ttu-id="1b5a7-127">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1b5a7-128">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1b5a7-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="1b5a7-129">orderHint</span></span>|<span data-ttu-id="1b5a7-130">Строка</span><span class="sxs-lookup"><span data-stu-id="1b5a7-130">String</span></span>|<span data-ttu-id="1b5a7-p105">Указание, используемое для расположения задачи в представлении "Ход выполнения" на доске задач. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="1b5a7-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b5a7-133">Связи</span><span class="sxs-lookup"><span data-stu-id="1b5a7-133">Relationships</span></span>
<span data-ttu-id="1b5a7-134">Нет</span><span class="sxs-lookup"><span data-stu-id="1b5a7-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1b5a7-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b5a7-135">JSON representation</span></span>
<span data-ttu-id="1b5a7-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b5a7-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
