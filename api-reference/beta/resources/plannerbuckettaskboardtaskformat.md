---
title: Тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены). Каждой задаче будет назначен один объект **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d40234fd729b849fee9fa789b9ae410eb0147f45
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344598"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="5daf8-104">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5daf8-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5daf8-105">Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены).</span><span class="sxs-lookup"><span data-stu-id="5daf8-105">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="5daf8-106">Каждой [задаче](plannertask.md) будет назначен один объект **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="5daf8-106">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="5daf8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5daf8-107">Methods</span></span>

| <span data-ttu-id="5daf8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5daf8-108">Method</span></span>           | <span data-ttu-id="5daf8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5daf8-109">Return Type</span></span>    |<span data-ttu-id="5daf8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5daf8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5daf8-111">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5daf8-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | <span data-ttu-id="5daf8-112">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="5daf8-112">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span> |<span data-ttu-id="5daf8-113">Чтение свойств и связей объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="5daf8-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="5daf8-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="5daf8-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | <span data-ttu-id="5daf8-115">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="5daf8-115">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span>  |<span data-ttu-id="5daf8-116">Обновление объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="5daf8-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5daf8-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5daf8-117">Properties</span></span>
| <span data-ttu-id="5daf8-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5daf8-118">Property</span></span>     | <span data-ttu-id="5daf8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5daf8-119">Type</span></span>   |<span data-ttu-id="5daf8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5daf8-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5daf8-121">id</span><span class="sxs-lookup"><span data-stu-id="5daf8-121">id</span></span>|<span data-ttu-id="5daf8-122">String</span><span class="sxs-lookup"><span data-stu-id="5daf8-122">String</span></span>| <span data-ttu-id="5daf8-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5daf8-123">Read-only.</span></span> <span data-ttu-id="5daf8-124">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="5daf8-124">ID of the resource.</span></span> <span data-ttu-id="5daf8-125">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5daf8-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5daf8-126">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="5daf8-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5daf8-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="5daf8-127">orderHint</span></span>|<span data-ttu-id="5daf8-128">String</span><span class="sxs-lookup"><span data-stu-id="5daf8-128">String</span></span>|<span data-ttu-id="5daf8-p104">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="5daf8-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5daf8-131">Связи</span><span class="sxs-lookup"><span data-stu-id="5daf8-131">Relationships</span></span>
<span data-ttu-id="5daf8-132">Нет</span><span class="sxs-lookup"><span data-stu-id="5daf8-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5daf8-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5daf8-133">JSON representation</span></span>
<span data-ttu-id="5daf8-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5daf8-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
