---
title: Тип ресурса plannerBucketTaskBoardTaskFormat
description: Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены). Каждой задаче будет назначен один объект **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6815209c4a87ee348cb3c37f5b318a5022e4c5b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521785"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="cbe0d-104">Тип ресурса plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="cbe0d-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="cbe0d-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cbe0d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbe0d-106">Ресурс **plannerBucketTaskBoardTaskFormat** представляет сведения, используемые для корректной визуализации задачи в представлении "сегменты" доски задач (представление, упорядоченное по задачам в сегментах, которым они назначены).</span><span class="sxs-lookup"><span data-stu-id="cbe0d-106">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to).</span></span> <span data-ttu-id="cbe0d-107">Каждой [задаче](plannertask.md) будет назначен один объект **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="cbe0d-107">Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="cbe0d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cbe0d-108">Methods</span></span>

| <span data-ttu-id="cbe0d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cbe0d-109">Method</span></span>           | <span data-ttu-id="cbe0d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cbe0d-110">Return Type</span></span>    |<span data-ttu-id="cbe0d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cbe0d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbe0d-112">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="cbe0d-112">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | <span data-ttu-id="cbe0d-113">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="cbe0d-113">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span> |<span data-ttu-id="cbe0d-114">Чтение свойств и связей объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="cbe0d-114">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|<span data-ttu-id="cbe0d-115">[обновление](../api/plannerbuckettaskboardtaskformat-update.md).</span><span class="sxs-lookup"><span data-stu-id="cbe0d-115">[Update](../api/plannerbuckettaskboardtaskformat-update.md)</span></span> | <span data-ttu-id="cbe0d-116">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md);</span><span class="sxs-lookup"><span data-stu-id="cbe0d-116">[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)</span></span>  |<span data-ttu-id="cbe0d-117">Обновление объекта **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="cbe0d-117">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cbe0d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbe0d-118">Properties</span></span>
| <span data-ttu-id="cbe0d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbe0d-119">Property</span></span>     | <span data-ttu-id="cbe0d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cbe0d-120">Type</span></span>   |<span data-ttu-id="cbe0d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cbe0d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbe0d-122">id</span><span class="sxs-lookup"><span data-stu-id="cbe0d-122">id</span></span>|<span data-ttu-id="cbe0d-123">String</span><span class="sxs-lookup"><span data-stu-id="cbe0d-123">String</span></span>| <span data-ttu-id="cbe0d-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cbe0d-124">Read-only.</span></span> <span data-ttu-id="cbe0d-125">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="cbe0d-125">ID of the resource.</span></span> <span data-ttu-id="cbe0d-126">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="cbe0d-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="cbe0d-127">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="cbe0d-127">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="cbe0d-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="cbe0d-128">orderHint</span></span>|<span data-ttu-id="cbe0d-129">String</span><span class="sxs-lookup"><span data-stu-id="cbe0d-129">String</span></span>|<span data-ttu-id="cbe0d-p104">Указание, используемое для расположения задач в окне "Сегмент" доски задачи. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="cbe0d-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbe0d-132">Связи</span><span class="sxs-lookup"><span data-stu-id="cbe0d-132">Relationships</span></span>
<span data-ttu-id="cbe0d-133">Нет</span><span class="sxs-lookup"><span data-stu-id="cbe0d-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cbe0d-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbe0d-134">JSON representation</span></span>
<span data-ttu-id="cbe0d-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbe0d-135">Here is a JSON representation of the resource.</span></span>

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
