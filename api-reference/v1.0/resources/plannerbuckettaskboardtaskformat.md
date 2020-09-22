---
title: Тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены). Каждой задаче будет назначен один объект **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1bd9282a137640af0abc1fd590ac5a87c18ea94e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037502"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="66e90-104">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="66e90-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="66e90-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66e90-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66e90-106">Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены).</span><span class="sxs-lookup"><span data-stu-id="66e90-106">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="66e90-107">Каждой [задаче](plannertask.md) будет назначен один объект **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="66e90-107">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="66e90-108">Методы</span><span class="sxs-lookup"><span data-stu-id="66e90-108">Methods</span></span>

| <span data-ttu-id="66e90-109">Метод</span><span class="sxs-lookup"><span data-stu-id="66e90-109">Method</span></span>           | <span data-ttu-id="66e90-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="66e90-110">Return Type</span></span>    |<span data-ttu-id="66e90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66e90-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66e90-112">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="66e90-112">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | <span data-ttu-id="66e90-113">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="66e90-113">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span> |<span data-ttu-id="66e90-114">Чтение свойств и связей объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="66e90-114">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|<span data-ttu-id="66e90-115">[обновление](../api/plannerbuckettaskboardtaskformat-update.md).</span><span class="sxs-lookup"><span data-stu-id="66e90-115">[Update](../api/plannerbuckettaskboardtaskformat-update.md)</span></span> | <span data-ttu-id="66e90-116">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="66e90-116">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span>  |<span data-ttu-id="66e90-117">Обновление объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="66e90-117">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="66e90-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="66e90-118">Properties</span></span>
| <span data-ttu-id="66e90-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="66e90-119">Property</span></span>     | <span data-ttu-id="66e90-120">Тип</span><span class="sxs-lookup"><span data-stu-id="66e90-120">Type</span></span>   |<span data-ttu-id="66e90-121">Описание</span><span class="sxs-lookup"><span data-stu-id="66e90-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66e90-122">id</span><span class="sxs-lookup"><span data-stu-id="66e90-122">id</span></span>|<span data-ttu-id="66e90-123">String</span><span class="sxs-lookup"><span data-stu-id="66e90-123">String</span></span>| <span data-ttu-id="66e90-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66e90-124">Read-only.</span></span> <span data-ttu-id="66e90-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="66e90-125">ID of the resource.</span></span> <span data-ttu-id="66e90-126">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="66e90-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="66e90-127">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="66e90-127">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="66e90-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="66e90-128">orderHint</span></span>|<span data-ttu-id="66e90-129">String</span><span class="sxs-lookup"><span data-stu-id="66e90-129">String</span></span>|<span data-ttu-id="66e90-p104">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="66e90-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="66e90-132">Связи</span><span class="sxs-lookup"><span data-stu-id="66e90-132">Relationships</span></span>
<span data-ttu-id="66e90-133">Нет</span><span class="sxs-lookup"><span data-stu-id="66e90-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="66e90-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66e90-134">JSON representation</span></span>
<span data-ttu-id="66e90-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66e90-135">Here is a JSON representation of the resource.</span></span>

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

