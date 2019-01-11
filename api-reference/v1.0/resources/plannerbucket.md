---
title: Тип ресурса plannerBucket
description: ) для выполнения задач в плане в Office 365. Она содержится в plannerPlan и можно создать свою коллекцию plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: 592d0e24f527d7ae343bd29e71a3dfdf0247720f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831460"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="314c2-104">Тип ресурса plannerBucket</span><span class="sxs-lookup"><span data-stu-id="314c2-104">plannerBucket resource type</span></span>

<span data-ttu-id="314c2-p102">Ресурс **plannerBucket** представляет сегмент (или "специальный столбец") для задач плана в Office 365. Он содержится в объекте [plannerPlan](plannerplan.md) и может содержать коллекцию объектов [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="314c2-p102">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="314c2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="314c2-107">Methods</span></span>

| <span data-ttu-id="314c2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="314c2-108">Method</span></span>           | <span data-ttu-id="314c2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="314c2-109">Return Type</span></span>    |<span data-ttu-id="314c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="314c2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="314c2-111">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="314c2-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="314c2-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="314c2-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="314c2-113">Чтение свойств и отношений объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="314c2-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="314c2-114">Перечисление объектов plannerTasks</span><span class="sxs-lookup"><span data-stu-id="314c2-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="314c2-115">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="314c2-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="314c2-116">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="314c2-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="314c2-117">Создание</span><span class="sxs-lookup"><span data-stu-id="314c2-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="314c2-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="314c2-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="314c2-119">Создание объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="314c2-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="314c2-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="314c2-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="314c2-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="314c2-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="314c2-122">Обновление объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="314c2-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="314c2-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="314c2-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="314c2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="314c2-124">None</span></span> |<span data-ttu-id="314c2-125">Удаление объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="314c2-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="314c2-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="314c2-126">Properties</span></span>
| <span data-ttu-id="314c2-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="314c2-127">Property</span></span>     | <span data-ttu-id="314c2-128">Тип</span><span class="sxs-lookup"><span data-stu-id="314c2-128">Type</span></span>   |<span data-ttu-id="314c2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="314c2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="314c2-130">id</span><span class="sxs-lookup"><span data-stu-id="314c2-130">id</span></span>|<span data-ttu-id="314c2-131">Строка</span><span class="sxs-lookup"><span data-stu-id="314c2-131">String</span></span>| <span data-ttu-id="314c2-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="314c2-132">Read-only.</span></span> <span data-ttu-id="314c2-133">Идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="314c2-133">ID of the bucket.</span></span> <span data-ttu-id="314c2-134">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="314c2-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="314c2-135">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="314c2-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="314c2-136">name</span><span class="sxs-lookup"><span data-stu-id="314c2-136">name</span></span>|<span data-ttu-id="314c2-137">Строка</span><span class="sxs-lookup"><span data-stu-id="314c2-137">String</span></span>|<span data-ttu-id="314c2-138">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="314c2-138">Name of the bucket.</span></span>|
|<span data-ttu-id="314c2-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="314c2-139">orderHint</span></span>|<span data-ttu-id="314c2-140">Строка</span><span class="sxs-lookup"><span data-stu-id="314c2-140">String</span></span>|<span data-ttu-id="314c2-p104">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="314c2-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="314c2-143">planId</span><span class="sxs-lookup"><span data-stu-id="314c2-143">planId</span></span>|<span data-ttu-id="314c2-144">Строка</span><span class="sxs-lookup"><span data-stu-id="314c2-144">String</span></span>|<span data-ttu-id="314c2-145">Идентификатор плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="314c2-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="314c2-146">Связи</span><span class="sxs-lookup"><span data-stu-id="314c2-146">Relationships</span></span>
| <span data-ttu-id="314c2-147">Связь</span><span class="sxs-lookup"><span data-stu-id="314c2-147">Relationship</span></span> | <span data-ttu-id="314c2-148">Тип</span><span class="sxs-lookup"><span data-stu-id="314c2-148">Type</span></span>   |<span data-ttu-id="314c2-149">Описание</span><span class="sxs-lookup"><span data-stu-id="314c2-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="314c2-150">tasks</span><span class="sxs-lookup"><span data-stu-id="314c2-150">tasks</span></span>|<span data-ttu-id="314c2-151">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="314c2-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="314c2-p105">Только для чтения. Допускает значение null. Коллекция задач в сегменте.</span><span class="sxs-lookup"><span data-stu-id="314c2-p105">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="314c2-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="314c2-155">JSON representation</span></span>
<span data-ttu-id="314c2-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="314c2-156">Here is a JSON representation of the resource.</span></span>

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
