---
title: Тип ресурса plannerBucket
description: ) для задач в плане в Office 365. Он находится в plannerPlan и может иметь коллекцию перечисление plannertasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 40dc49363e4214c044c408760007a46b8f65ea46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447152"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="35873-104">Тип ресурса plannerBucket</span><span class="sxs-lookup"><span data-stu-id="35873-104">plannerBucket resource type</span></span>

<span data-ttu-id="35873-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="35873-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35873-106">Ресурс **plannerBucket** представляет сегмент (или "настраиваемый столбец") для задач в плане в Office 365.</span><span class="sxs-lookup"><span data-stu-id="35873-106">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="35873-107">Он находится в [plannerPlan](plannerplan.md) и может иметь коллекцию [перечисление plannertasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="35873-107">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="35873-108">Методы</span><span class="sxs-lookup"><span data-stu-id="35873-108">Methods</span></span>

| <span data-ttu-id="35873-109">Метод</span><span class="sxs-lookup"><span data-stu-id="35873-109">Method</span></span>           | <span data-ttu-id="35873-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35873-110">Return Type</span></span>    |<span data-ttu-id="35873-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35873-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35873-112">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="35873-112">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | <span data-ttu-id="35873-113">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="35873-113">[plannerBucket](plannerbucket.md)</span></span> |<span data-ttu-id="35873-114">Чтение свойств и связей объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="35873-114">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="35873-115">Перечисление plannerTasks</span><span class="sxs-lookup"><span data-stu-id="35873-115">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="35873-116">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="35873-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="35873-117">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="35873-117">Get a **plannerTask** object collection.</span></span>|
|<span data-ttu-id="35873-118">[создание](../api/planner-post-buckets.md);</span><span class="sxs-lookup"><span data-stu-id="35873-118">[Create](../api/planner-post-buckets.md)</span></span> | <span data-ttu-id="35873-119">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="35873-119">[plannerBucket](plannerbucket.md)</span></span>   | <span data-ttu-id="35873-120">Создание нового объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="35873-120">Create a new **plannerBucket** object.</span></span> |
|<span data-ttu-id="35873-121">[обновление](../api/plannerbucket-update.md).</span><span class="sxs-lookup"><span data-stu-id="35873-121">[Update](../api/plannerbucket-update.md)</span></span> | <span data-ttu-id="35873-122">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="35873-122">[plannerBucket](plannerbucket.md)</span></span>   |<span data-ttu-id="35873-123">Обновление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="35873-123">Update **plannerBucket** object.</span></span> |
|<span data-ttu-id="35873-124">[удаление](../api/plannerbucket-delete.md);</span><span class="sxs-lookup"><span data-stu-id="35873-124">[Delete](../api/plannerbucket-delete.md)</span></span> | <span data-ttu-id="35873-125">Нет</span><span class="sxs-lookup"><span data-stu-id="35873-125">None</span></span> |<span data-ttu-id="35873-126">Удаление объекта **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="35873-126">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="35873-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="35873-127">Properties</span></span>
| <span data-ttu-id="35873-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="35873-128">Property</span></span>     | <span data-ttu-id="35873-129">Тип</span><span class="sxs-lookup"><span data-stu-id="35873-129">Type</span></span>   |<span data-ttu-id="35873-130">Описание</span><span class="sxs-lookup"><span data-stu-id="35873-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35873-131">id</span><span class="sxs-lookup"><span data-stu-id="35873-131">id</span></span>|<span data-ttu-id="35873-132">String</span><span class="sxs-lookup"><span data-stu-id="35873-132">String</span></span>| <span data-ttu-id="35873-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35873-133">Read-only.</span></span> <span data-ttu-id="35873-134">Идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="35873-134">ID of the bucket.</span></span> <span data-ttu-id="35873-135">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="35873-135">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="35873-136">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="35873-136">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="35873-137">name</span><span class="sxs-lookup"><span data-stu-id="35873-137">name</span></span>|<span data-ttu-id="35873-138">Строка</span><span class="sxs-lookup"><span data-stu-id="35873-138">String</span></span>|<span data-ttu-id="35873-139">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="35873-139">Name of the bucket.</span></span>|
|<span data-ttu-id="35873-140">orderHint</span><span class="sxs-lookup"><span data-stu-id="35873-140">orderHint</span></span>|<span data-ttu-id="35873-141">String</span><span class="sxs-lookup"><span data-stu-id="35873-141">String</span></span>|<span data-ttu-id="35873-p104">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="35873-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="35873-144">planId</span><span class="sxs-lookup"><span data-stu-id="35873-144">planId</span></span>|<span data-ttu-id="35873-145">Строка</span><span class="sxs-lookup"><span data-stu-id="35873-145">String</span></span>|<span data-ttu-id="35873-146">ИДЕНТИФИКАТОР плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="35873-146">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35873-147">Связи</span><span class="sxs-lookup"><span data-stu-id="35873-147">Relationships</span></span>
| <span data-ttu-id="35873-148">Связь</span><span class="sxs-lookup"><span data-stu-id="35873-148">Relationship</span></span> | <span data-ttu-id="35873-149">Тип</span><span class="sxs-lookup"><span data-stu-id="35873-149">Type</span></span>   |<span data-ttu-id="35873-150">Описание</span><span class="sxs-lookup"><span data-stu-id="35873-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35873-151">tasks</span><span class="sxs-lookup"><span data-stu-id="35873-151">tasks</span></span>|<span data-ttu-id="35873-152">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="35873-152">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="35873-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35873-153">Read-only.</span></span> <span data-ttu-id="35873-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="35873-154">Nullable.</span></span> <span data-ttu-id="35873-155">Коллекция задач в сегменте.</span><span class="sxs-lookup"><span data-stu-id="35873-155">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35873-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35873-156">JSON representation</span></span>
<span data-ttu-id="35873-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35873-157">Here is a JSON representation of the resource.</span></span>

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
