---
title: Тип ресурса plannerBucket
description: ) для задач в плане в Office 365. Он находится в plannerPlan и может иметь коллекцию перечисление plannertasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: a9e6b3ac4a9bad8d7402dee28706b5200c623078
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344589"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="39ff6-104">Тип ресурса plannerBucket</span><span class="sxs-lookup"><span data-stu-id="39ff6-104">plannerBucket resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39ff6-105">Ресурс **plannerBucket** представляет сегмент (или "настраиваемый столбец") для задач в плане в Office 365.</span><span class="sxs-lookup"><span data-stu-id="39ff6-105">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="39ff6-106">Он находится в [plannerPlan](plannerplan.md) и может иметь коллекцию [перечисление plannertasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="39ff6-106">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="39ff6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="39ff6-107">Methods</span></span>

| <span data-ttu-id="39ff6-108">Метод</span><span class="sxs-lookup"><span data-stu-id="39ff6-108">Method</span></span>           | <span data-ttu-id="39ff6-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="39ff6-109">Return Type</span></span>    |<span data-ttu-id="39ff6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="39ff6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="39ff6-111">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="39ff6-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | <span data-ttu-id="39ff6-112">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="39ff6-112">[plannerBucket](plannerbucket.md)</span></span> |<span data-ttu-id="39ff6-113">Чтение свойств и связей объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="39ff6-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="39ff6-114">Перечисление plannerTasks</span><span class="sxs-lookup"><span data-stu-id="39ff6-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="39ff6-115">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="39ff6-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="39ff6-116">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="39ff6-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="39ff6-117">Создание</span><span class="sxs-lookup"><span data-stu-id="39ff6-117">Create</span></span>](../api/planner-post-buckets.md) | <span data-ttu-id="39ff6-118">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="39ff6-118">[plannerBucket](plannerbucket.md)</span></span>   | <span data-ttu-id="39ff6-119">Создание нового объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="39ff6-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="39ff6-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="39ff6-120">Update</span></span>](../api/plannerbucket-update.md) | <span data-ttu-id="39ff6-121">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="39ff6-121">[plannerBucket](plannerbucket.md)</span></span>   |<span data-ttu-id="39ff6-122">Обновление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="39ff6-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="39ff6-123">Delete</span><span class="sxs-lookup"><span data-stu-id="39ff6-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="39ff6-124">Нет</span><span class="sxs-lookup"><span data-stu-id="39ff6-124">None</span></span> |<span data-ttu-id="39ff6-125">Удаление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="39ff6-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="39ff6-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="39ff6-126">Properties</span></span>
| <span data-ttu-id="39ff6-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="39ff6-127">Property</span></span>     | <span data-ttu-id="39ff6-128">Тип</span><span class="sxs-lookup"><span data-stu-id="39ff6-128">Type</span></span>   |<span data-ttu-id="39ff6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="39ff6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39ff6-130">id</span><span class="sxs-lookup"><span data-stu-id="39ff6-130">id</span></span>|<span data-ttu-id="39ff6-131">String</span><span class="sxs-lookup"><span data-stu-id="39ff6-131">String</span></span>| <span data-ttu-id="39ff6-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ff6-132">Read-only.</span></span> <span data-ttu-id="39ff6-133">Идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="39ff6-133">ID of the bucket.</span></span> <span data-ttu-id="39ff6-134">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="39ff6-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="39ff6-135">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="39ff6-135">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="39ff6-136">name</span><span class="sxs-lookup"><span data-stu-id="39ff6-136">name</span></span>|<span data-ttu-id="39ff6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="39ff6-137">String</span></span>|<span data-ttu-id="39ff6-138">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="39ff6-138">Name of the bucket.</span></span>|
|<span data-ttu-id="39ff6-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="39ff6-139">orderHint</span></span>|<span data-ttu-id="39ff6-140">String</span><span class="sxs-lookup"><span data-stu-id="39ff6-140">String</span></span>|<span data-ttu-id="39ff6-p104">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="39ff6-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="39ff6-143">planId</span><span class="sxs-lookup"><span data-stu-id="39ff6-143">planId</span></span>|<span data-ttu-id="39ff6-144">Строка</span><span class="sxs-lookup"><span data-stu-id="39ff6-144">String</span></span>|<span data-ttu-id="39ff6-145">ИДЕНТИФИКАТОР плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="39ff6-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39ff6-146">Связи</span><span class="sxs-lookup"><span data-stu-id="39ff6-146">Relationships</span></span>
| <span data-ttu-id="39ff6-147">Отношение</span><span class="sxs-lookup"><span data-stu-id="39ff6-147">Relationship</span></span> | <span data-ttu-id="39ff6-148">Тип</span><span class="sxs-lookup"><span data-stu-id="39ff6-148">Type</span></span>   |<span data-ttu-id="39ff6-149">Описание</span><span class="sxs-lookup"><span data-stu-id="39ff6-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39ff6-150">tasks</span><span class="sxs-lookup"><span data-stu-id="39ff6-150">tasks</span></span>|<span data-ttu-id="39ff6-151">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="39ff6-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="39ff6-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ff6-152">Read-only.</span></span> <span data-ttu-id="39ff6-153">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="39ff6-153">Nullable.</span></span> <span data-ttu-id="39ff6-154">Коллекция задач в сегменте.</span><span class="sxs-lookup"><span data-stu-id="39ff6-154">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39ff6-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39ff6-155">JSON representation</span></span>
<span data-ttu-id="39ff6-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39ff6-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
