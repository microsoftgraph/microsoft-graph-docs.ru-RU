---
title: Тип ресурса plannerBucket
description: ) для задач в плане в Office 365. Он находится в plannerPlan и может иметь коллекцию перечисление plannertasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: eed92a62fed8077d2b7ee541feac7e0fa5c73483
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966016"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="f885f-104">Тип ресурса plannerBucket</span><span class="sxs-lookup"><span data-stu-id="f885f-104">plannerBucket resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f885f-105">Ресурс **plannerBucket** представляет сегмент (или "настраиваемый столбец") для задач в плане в Office 365.</span><span class="sxs-lookup"><span data-stu-id="f885f-105">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="f885f-106">Он находится в [plannerPlan](plannerplan.md) и может иметь коллекцию [перечисление plannertasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="f885f-106">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="f885f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f885f-107">Methods</span></span>

| <span data-ttu-id="f885f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f885f-108">Method</span></span>           | <span data-ttu-id="f885f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f885f-109">Return Type</span></span>    |<span data-ttu-id="f885f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f885f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f885f-111">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="f885f-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | <span data-ttu-id="f885f-112">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="f885f-112">[plannerBucket](plannerbucket.md)</span></span> |<span data-ttu-id="f885f-113">Чтение свойств и связей объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="f885f-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="f885f-114">Перечисление plannerTasks</span><span class="sxs-lookup"><span data-stu-id="f885f-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="f885f-115">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="f885f-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="f885f-116">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="f885f-116">Get a **plannerTask** object collection.</span></span>|
|<span data-ttu-id="f885f-117">[создание](../api/planner-post-buckets.md);</span><span class="sxs-lookup"><span data-stu-id="f885f-117">[Create](../api/planner-post-buckets.md)</span></span> | <span data-ttu-id="f885f-118">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="f885f-118">[plannerBucket](plannerbucket.md)</span></span>   | <span data-ttu-id="f885f-119">Создание нового объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="f885f-119">Create a new **plannerBucket** object.</span></span> |
|<span data-ttu-id="f885f-120">[обновление](../api/plannerbucket-update.md);</span><span class="sxs-lookup"><span data-stu-id="f885f-120">[Update](../api/plannerbucket-update.md)</span></span> | <span data-ttu-id="f885f-121">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="f885f-121">[plannerBucket](plannerbucket.md)</span></span>   |<span data-ttu-id="f885f-122">Обновление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="f885f-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="f885f-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="f885f-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="f885f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f885f-124">None</span></span> |<span data-ttu-id="f885f-125">Удаление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="f885f-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f885f-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="f885f-126">Properties</span></span>
| <span data-ttu-id="f885f-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="f885f-127">Property</span></span>     | <span data-ttu-id="f885f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f885f-128">Type</span></span>   |<span data-ttu-id="f885f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f885f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f885f-130">id</span><span class="sxs-lookup"><span data-stu-id="f885f-130">id</span></span>|<span data-ttu-id="f885f-131">String</span><span class="sxs-lookup"><span data-stu-id="f885f-131">String</span></span>| <span data-ttu-id="f885f-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f885f-132">Read-only.</span></span> <span data-ttu-id="f885f-133">Идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="f885f-133">ID of the bucket.</span></span> <span data-ttu-id="f885f-134">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f885f-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="f885f-135">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="f885f-135">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="f885f-136">name</span><span class="sxs-lookup"><span data-stu-id="f885f-136">name</span></span>|<span data-ttu-id="f885f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f885f-137">String</span></span>|<span data-ttu-id="f885f-138">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="f885f-138">Name of the bucket.</span></span>|
|<span data-ttu-id="f885f-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="f885f-139">orderHint</span></span>|<span data-ttu-id="f885f-140">String</span><span class="sxs-lookup"><span data-stu-id="f885f-140">String</span></span>|<span data-ttu-id="f885f-p104">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="f885f-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="f885f-143">planId</span><span class="sxs-lookup"><span data-stu-id="f885f-143">planId</span></span>|<span data-ttu-id="f885f-144">Строка</span><span class="sxs-lookup"><span data-stu-id="f885f-144">String</span></span>|<span data-ttu-id="f885f-145">ИДЕНТИФИКАТОР плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="f885f-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f885f-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="f885f-146">Relationships</span></span>
| <span data-ttu-id="f885f-147">Отношение</span><span class="sxs-lookup"><span data-stu-id="f885f-147">Relationship</span></span> | <span data-ttu-id="f885f-148">Тип</span><span class="sxs-lookup"><span data-stu-id="f885f-148">Type</span></span>   |<span data-ttu-id="f885f-149">Описание</span><span class="sxs-lookup"><span data-stu-id="f885f-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f885f-150">tasks</span><span class="sxs-lookup"><span data-stu-id="f885f-150">tasks</span></span>|<span data-ttu-id="f885f-151">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="f885f-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="f885f-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f885f-152">Read-only.</span></span> <span data-ttu-id="f885f-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f885f-153">Nullable.</span></span> <span data-ttu-id="f885f-154">Коллекция задач в сегменте.</span><span class="sxs-lookup"><span data-stu-id="f885f-154">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f885f-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f885f-155">JSON representation</span></span>
<span data-ttu-id="f885f-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f885f-156">Here is a JSON representation of the resource.</span></span>

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
