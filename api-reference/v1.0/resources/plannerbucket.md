---
title: Тип ресурса plannerBucket
description: ) для задач в плане в Office 365. Он находится в plannerPlan и может иметь коллекцию перечисление plannertasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b6810a62ecab5209ca1c17aa7f3ca9e4753a50a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035326"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="102fe-104">Тип ресурса plannerBucket</span><span class="sxs-lookup"><span data-stu-id="102fe-104">plannerBucket resource type</span></span>

<span data-ttu-id="102fe-105">Ресурс **plannerBucket** представляет сегмент (или "настраиваемый столбец") для задач в плане в Office 365.</span><span class="sxs-lookup"><span data-stu-id="102fe-105">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="102fe-106">Он находится в [plannerPlan](plannerplan.md) и может иметь коллекцию [перечисление plannertasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="102fe-106">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="102fe-107">Методы</span><span class="sxs-lookup"><span data-stu-id="102fe-107">Methods</span></span>

| <span data-ttu-id="102fe-108">Метод</span><span class="sxs-lookup"><span data-stu-id="102fe-108">Method</span></span>           | <span data-ttu-id="102fe-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="102fe-109">Return Type</span></span>    |<span data-ttu-id="102fe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="102fe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="102fe-111">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="102fe-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | <span data-ttu-id="102fe-112">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="102fe-112">[plannerBucket](plannerbucket.md)</span></span> |<span data-ttu-id="102fe-113">Чтение свойств и связей объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="102fe-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="102fe-114">Перечисление plannerTasks</span><span class="sxs-lookup"><span data-stu-id="102fe-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="102fe-115">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="102fe-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="102fe-116">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="102fe-116">Get a **plannerTask** object collection.</span></span>|
|<span data-ttu-id="102fe-117">[создание](../api/planner-post-buckets.md);</span><span class="sxs-lookup"><span data-stu-id="102fe-117">[Create](../api/planner-post-buckets.md)</span></span> | <span data-ttu-id="102fe-118">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="102fe-118">[plannerBucket](plannerbucket.md)</span></span>   | <span data-ttu-id="102fe-119">Создание нового объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="102fe-119">Create a new **plannerBucket** object.</span></span> |
|<span data-ttu-id="102fe-120">[обновление](../api/plannerbucket-update.md);</span><span class="sxs-lookup"><span data-stu-id="102fe-120">[Update](../api/plannerbucket-update.md)</span></span> | <span data-ttu-id="102fe-121">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="102fe-121">[plannerBucket](plannerbucket.md)</span></span>   |<span data-ttu-id="102fe-122">Обновление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="102fe-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="102fe-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="102fe-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="102fe-124">Нет</span><span class="sxs-lookup"><span data-stu-id="102fe-124">None</span></span> |<span data-ttu-id="102fe-125">Удаление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="102fe-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="102fe-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="102fe-126">Properties</span></span>
| <span data-ttu-id="102fe-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="102fe-127">Property</span></span>     | <span data-ttu-id="102fe-128">Тип</span><span class="sxs-lookup"><span data-stu-id="102fe-128">Type</span></span>   |<span data-ttu-id="102fe-129">Описание</span><span class="sxs-lookup"><span data-stu-id="102fe-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="102fe-130">id</span><span class="sxs-lookup"><span data-stu-id="102fe-130">id</span></span>|<span data-ttu-id="102fe-131">String</span><span class="sxs-lookup"><span data-stu-id="102fe-131">String</span></span>| <span data-ttu-id="102fe-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="102fe-132">Read-only.</span></span> <span data-ttu-id="102fe-133">Идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="102fe-133">ID of the bucket.</span></span> <span data-ttu-id="102fe-134">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="102fe-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="102fe-135">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="102fe-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="102fe-136">name</span><span class="sxs-lookup"><span data-stu-id="102fe-136">name</span></span>|<span data-ttu-id="102fe-137">Строка</span><span class="sxs-lookup"><span data-stu-id="102fe-137">String</span></span>|<span data-ttu-id="102fe-138">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="102fe-138">Name of the bucket.</span></span>|
|<span data-ttu-id="102fe-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="102fe-139">orderHint</span></span>|<span data-ttu-id="102fe-140">String</span><span class="sxs-lookup"><span data-stu-id="102fe-140">String</span></span>|<span data-ttu-id="102fe-p104">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="102fe-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="102fe-143">planId</span><span class="sxs-lookup"><span data-stu-id="102fe-143">planId</span></span>|<span data-ttu-id="102fe-144">Строка</span><span class="sxs-lookup"><span data-stu-id="102fe-144">String</span></span>|<span data-ttu-id="102fe-145">ИДЕНТИФИКАТОР плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="102fe-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="102fe-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="102fe-146">Relationships</span></span>
| <span data-ttu-id="102fe-147">Отношение</span><span class="sxs-lookup"><span data-stu-id="102fe-147">Relationship</span></span> | <span data-ttu-id="102fe-148">Тип</span><span class="sxs-lookup"><span data-stu-id="102fe-148">Type</span></span>   |<span data-ttu-id="102fe-149">Описание</span><span class="sxs-lookup"><span data-stu-id="102fe-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="102fe-150">tasks</span><span class="sxs-lookup"><span data-stu-id="102fe-150">tasks</span></span>|<span data-ttu-id="102fe-151">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="102fe-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="102fe-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="102fe-152">Read-only.</span></span> <span data-ttu-id="102fe-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="102fe-153">Nullable.</span></span> <span data-ttu-id="102fe-154">Коллекция задач в сегменте.</span><span class="sxs-lookup"><span data-stu-id="102fe-154">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="102fe-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="102fe-155">JSON representation</span></span>
<span data-ttu-id="102fe-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="102fe-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
