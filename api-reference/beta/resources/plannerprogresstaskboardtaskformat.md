---
title: Тип ресурса plannerProgressTaskBoardTaskFormat
description: Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом **task** связан один объект plannerProgressTaskBoardTaskFormat.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 20a215b108ca1f1801702a532bda09eac67834c6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522072"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="59691-104">Тип ресурса plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="59691-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59691-p102">Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом [task](plannertask.md) связан один объект **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="59691-p102">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="59691-107">Методы</span><span class="sxs-lookup"><span data-stu-id="59691-107">Methods</span></span>

| <span data-ttu-id="59691-108">Метод</span><span class="sxs-lookup"><span data-stu-id="59691-108">Method</span></span>           | <span data-ttu-id="59691-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="59691-109">Return Type</span></span>    |<span data-ttu-id="59691-110">Описание</span><span class="sxs-lookup"><span data-stu-id="59691-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="59691-111">Получение объекта plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="59691-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | <span data-ttu-id="59691-112">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md).</span><span class="sxs-lookup"><span data-stu-id="59691-112">[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)</span></span> |<span data-ttu-id="59691-113">Чтение свойств и отношений объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="59691-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="59691-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="59691-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="59691-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="59691-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="59691-116">Обновление объекта **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="59691-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="59691-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="59691-117">Properties</span></span>
| <span data-ttu-id="59691-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="59691-118">Property</span></span>     | <span data-ttu-id="59691-119">Тип</span><span class="sxs-lookup"><span data-stu-id="59691-119">Type</span></span>   |<span data-ttu-id="59691-120">Описание</span><span class="sxs-lookup"><span data-stu-id="59691-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59691-121">id</span><span class="sxs-lookup"><span data-stu-id="59691-121">id</span></span>|<span data-ttu-id="59691-122">String</span><span class="sxs-lookup"><span data-stu-id="59691-122">String</span></span>| <span data-ttu-id="59691-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59691-123">Read-only.</span></span> <span data-ttu-id="59691-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="59691-124">ID of the resource.</span></span> <span data-ttu-id="59691-125">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="59691-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="59691-126">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="59691-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="59691-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="59691-127">orderHint</span></span>|<span data-ttu-id="59691-128">String</span><span class="sxs-lookup"><span data-stu-id="59691-128">String</span></span>|<span data-ttu-id="59691-p104">Указание, используемое для расположения задачи в представлении "Ход выполнения" на доске задач. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="59691-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="59691-131">Связи</span><span class="sxs-lookup"><span data-stu-id="59691-131">Relationships</span></span>
<span data-ttu-id="59691-132">Нет</span><span class="sxs-lookup"><span data-stu-id="59691-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="59691-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59691-133">JSON representation</span></span>
<span data-ttu-id="59691-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59691-134">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerprogresstaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
