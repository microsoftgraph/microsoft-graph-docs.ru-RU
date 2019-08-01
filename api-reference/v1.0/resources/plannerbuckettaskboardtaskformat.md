---
title: Тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены). Каждой задаче будет назначен один объект **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: dcc78f60decaa50f0ac1a2051b84e2f651e11521
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035331"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="c3b23-104">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c3b23-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="c3b23-105">Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены).</span><span class="sxs-lookup"><span data-stu-id="c3b23-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="c3b23-106">Каждой [задаче](plannertask.md) будет назначен один объект **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="c3b23-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="c3b23-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c3b23-107">Methods</span></span>

| <span data-ttu-id="c3b23-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c3b23-108">Method</span></span>           | <span data-ttu-id="c3b23-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3b23-109">Return Type</span></span>    |<span data-ttu-id="c3b23-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c3b23-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3b23-111">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c3b23-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | <span data-ttu-id="c3b23-112">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="c3b23-112">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span> |<span data-ttu-id="c3b23-113">Чтение свойств и связей объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="c3b23-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|<span data-ttu-id="c3b23-114">[обновление](../api/plannerbuckettaskboardtaskformat-update.md);</span><span class="sxs-lookup"><span data-stu-id="c3b23-114">[Update](../api/plannerbuckettaskboardtaskformat-update.md)</span></span> | <span data-ttu-id="c3b23-115">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="c3b23-115">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span>  |<span data-ttu-id="c3b23-116">Обновление объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="c3b23-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3b23-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3b23-117">Properties</span></span>
| <span data-ttu-id="c3b23-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3b23-118">Property</span></span>     | <span data-ttu-id="c3b23-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c3b23-119">Type</span></span>   |<span data-ttu-id="c3b23-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c3b23-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3b23-121">id</span><span class="sxs-lookup"><span data-stu-id="c3b23-121">id</span></span>|<span data-ttu-id="c3b23-122">String</span><span class="sxs-lookup"><span data-stu-id="c3b23-122">String</span></span>| <span data-ttu-id="c3b23-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3b23-123">Read-only.</span></span> <span data-ttu-id="c3b23-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="c3b23-124">ID of the resource.</span></span> <span data-ttu-id="c3b23-125">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c3b23-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c3b23-126">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="c3b23-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c3b23-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="c3b23-127">orderHint</span></span>|<span data-ttu-id="c3b23-128">String</span><span class="sxs-lookup"><span data-stu-id="c3b23-128">String</span></span>|<span data-ttu-id="c3b23-p104">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c3b23-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3b23-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="c3b23-131">Relationships</span></span>
<span data-ttu-id="c3b23-132">Нет</span><span class="sxs-lookup"><span data-stu-id="c3b23-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c3b23-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3b23-133">JSON representation</span></span>
<span data-ttu-id="c3b23-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3b23-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
