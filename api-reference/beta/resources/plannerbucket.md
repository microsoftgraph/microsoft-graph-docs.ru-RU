---
title: Тип ресурса plannerBucket
description: ) для задач в плане в Microsoft 365. Он находится в plannerPlan и может иметь коллекцию перечисление plannertasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 33ce6a6be827510b522359ac93a77d1f0b74b477
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897052"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="1375d-104">Тип ресурса plannerBucket</span><span class="sxs-lookup"><span data-stu-id="1375d-104">plannerBucket resource type</span></span>

<span data-ttu-id="1375d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1375d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1375d-106">Ресурс **plannerBucket** представляет сегмент (или "настраиваемый столбец") для задач в плане в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1375d-106">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Microsoft 365.</span></span> <span data-ttu-id="1375d-107">Он находится в [plannerPlan](plannerplan.md) и может иметь коллекцию [перечисление plannertasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="1375d-107">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="1375d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1375d-108">Methods</span></span>

| <span data-ttu-id="1375d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1375d-109">Method</span></span>           | <span data-ttu-id="1375d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1375d-110">Return Type</span></span>    |<span data-ttu-id="1375d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1375d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1375d-112">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="1375d-112">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | <span data-ttu-id="1375d-113">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="1375d-113">[plannerBucket](plannerbucket.md)</span></span> |<span data-ttu-id="1375d-114">Чтение свойств и связей объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="1375d-114">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="1375d-115">Перечисление plannerTasks</span><span class="sxs-lookup"><span data-stu-id="1375d-115">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="1375d-116">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="1375d-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1375d-117">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="1375d-117">Get a **plannerTask** object collection.</span></span>|
|<span data-ttu-id="1375d-118">[Создание](../api/planner-post-buckets.md);</span><span class="sxs-lookup"><span data-stu-id="1375d-118">[Create](../api/planner-post-buckets.md)</span></span> | <span data-ttu-id="1375d-119">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="1375d-119">[plannerBucket](plannerbucket.md)</span></span>   | <span data-ttu-id="1375d-120">Создание нового объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="1375d-120">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="1375d-121">Update</span><span class="sxs-lookup"><span data-stu-id="1375d-121">Update</span></span>](../api/plannerbucket-update.md) | <span data-ttu-id="1375d-122">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="1375d-122">[plannerBucket](plannerbucket.md)</span></span>   |<span data-ttu-id="1375d-123">Обновление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="1375d-123">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="1375d-124">Delete</span><span class="sxs-lookup"><span data-stu-id="1375d-124">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="1375d-125">Нет</span><span class="sxs-lookup"><span data-stu-id="1375d-125">None</span></span> |<span data-ttu-id="1375d-126">Удаление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="1375d-126">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1375d-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="1375d-127">Properties</span></span>
| <span data-ttu-id="1375d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1375d-128">Property</span></span>     | <span data-ttu-id="1375d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1375d-129">Type</span></span>   |<span data-ttu-id="1375d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1375d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1375d-131">id</span><span class="sxs-lookup"><span data-stu-id="1375d-131">id</span></span>|<span data-ttu-id="1375d-132">String</span><span class="sxs-lookup"><span data-stu-id="1375d-132">String</span></span>| <span data-ttu-id="1375d-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1375d-133">Read-only.</span></span> <span data-ttu-id="1375d-134">Идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="1375d-134">ID of the bucket.</span></span> <span data-ttu-id="1375d-135">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="1375d-135">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1375d-136">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="1375d-136">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1375d-137">name</span><span class="sxs-lookup"><span data-stu-id="1375d-137">name</span></span>|<span data-ttu-id="1375d-138">Строка</span><span class="sxs-lookup"><span data-stu-id="1375d-138">String</span></span>|<span data-ttu-id="1375d-139">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="1375d-139">Name of the bucket.</span></span>|
|<span data-ttu-id="1375d-140">orderHint</span><span class="sxs-lookup"><span data-stu-id="1375d-140">orderHint</span></span>|<span data-ttu-id="1375d-141">String</span><span class="sxs-lookup"><span data-stu-id="1375d-141">String</span></span>|<span data-ttu-id="1375d-p104">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="1375d-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="1375d-144">planId</span><span class="sxs-lookup"><span data-stu-id="1375d-144">planId</span></span>|<span data-ttu-id="1375d-145">Строка</span><span class="sxs-lookup"><span data-stu-id="1375d-145">String</span></span>|<span data-ttu-id="1375d-146">ИДЕНТИФИКАТОР плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="1375d-146">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1375d-147">Связи</span><span class="sxs-lookup"><span data-stu-id="1375d-147">Relationships</span></span>
| <span data-ttu-id="1375d-148">Связь</span><span class="sxs-lookup"><span data-stu-id="1375d-148">Relationship</span></span> | <span data-ttu-id="1375d-149">Тип</span><span class="sxs-lookup"><span data-stu-id="1375d-149">Type</span></span>   |<span data-ttu-id="1375d-150">Описание</span><span class="sxs-lookup"><span data-stu-id="1375d-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1375d-151">tasks</span><span class="sxs-lookup"><span data-stu-id="1375d-151">tasks</span></span>|<span data-ttu-id="1375d-152">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="1375d-152">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1375d-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1375d-153">Read-only.</span></span> <span data-ttu-id="1375d-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1375d-154">Nullable.</span></span> <span data-ttu-id="1375d-155">Коллекция задач в сегменте.</span><span class="sxs-lookup"><span data-stu-id="1375d-155">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1375d-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1375d-156">JSON representation</span></span>
<span data-ttu-id="1375d-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1375d-157">Here is a JSON representation of the resource.</span></span>

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
