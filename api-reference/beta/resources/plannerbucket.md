---
title: Тип ресурса plannerBucket
description: ) для выполнения задач в плане в Office 365. Она содержится в plannerPlan и можно создать свою коллекцию plannerTasks.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 4ed1cbe51ca22fbabce6dfd030747e728299190f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929713"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="0a369-104">Тип ресурса plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0a369-104">plannerBucket resource type</span></span>

> <span data-ttu-id="0a369-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a369-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a369-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a369-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a369-p103">Ресурс **plannerBucket** представляет сегмент (или "специальный столбец") для задач плана в Office 365. Он содержится в объекте [plannerPlan](plannerplan.md) и может содержать коллекцию объектов [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="0a369-p103">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="0a369-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0a369-109">Methods</span></span>

| <span data-ttu-id="0a369-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0a369-110">Method</span></span>           | <span data-ttu-id="0a369-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0a369-111">Return Type</span></span>    |<span data-ttu-id="0a369-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0a369-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a369-113">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0a369-113">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="0a369-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0a369-114">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="0a369-115">Чтение свойств и отношений объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="0a369-115">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="0a369-116">Перечисление объектов plannerTasks</span><span class="sxs-lookup"><span data-stu-id="0a369-116">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="0a369-117">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="0a369-117">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="0a369-118">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="0a369-118">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="0a369-119">Создание</span><span class="sxs-lookup"><span data-stu-id="0a369-119">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="0a369-120">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0a369-120">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="0a369-121">Создание объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="0a369-121">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="0a369-122">Обновление</span><span class="sxs-lookup"><span data-stu-id="0a369-122">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="0a369-123">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0a369-123">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="0a369-124">Обновление объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="0a369-124">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="0a369-125">Удаление</span><span class="sxs-lookup"><span data-stu-id="0a369-125">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="0a369-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0a369-126">None</span></span> |<span data-ttu-id="0a369-127">Удаление объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="0a369-127">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0a369-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a369-128">Properties</span></span>
| <span data-ttu-id="0a369-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a369-129">Property</span></span>     | <span data-ttu-id="0a369-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0a369-130">Type</span></span>   |<span data-ttu-id="0a369-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0a369-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a369-132">id</span><span class="sxs-lookup"><span data-stu-id="0a369-132">id</span></span>|<span data-ttu-id="0a369-133">String</span><span class="sxs-lookup"><span data-stu-id="0a369-133">String</span></span>| <span data-ttu-id="0a369-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a369-134">Read-only.</span></span> <span data-ttu-id="0a369-135">Идентификатор сегмента.</span><span class="sxs-lookup"><span data-stu-id="0a369-135">ID of the bucket.</span></span> <span data-ttu-id="0a369-136">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="0a369-136">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0a369-137">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="0a369-137">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="0a369-138">name</span><span class="sxs-lookup"><span data-stu-id="0a369-138">name</span></span>|<span data-ttu-id="0a369-139">Строка</span><span class="sxs-lookup"><span data-stu-id="0a369-139">String</span></span>|<span data-ttu-id="0a369-140">Имя сегмента.</span><span class="sxs-lookup"><span data-stu-id="0a369-140">Name of the bucket.</span></span>|
|<span data-ttu-id="0a369-141">orderHint</span><span class="sxs-lookup"><span data-stu-id="0a369-141">orderHint</span></span>|<span data-ttu-id="0a369-142">String</span><span class="sxs-lookup"><span data-stu-id="0a369-142">String</span></span>|<span data-ttu-id="0a369-p105">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определяется, как описано [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="0a369-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="0a369-145">planId</span><span class="sxs-lookup"><span data-stu-id="0a369-145">planId</span></span>|<span data-ttu-id="0a369-146">Строка</span><span class="sxs-lookup"><span data-stu-id="0a369-146">String</span></span>|<span data-ttu-id="0a369-147">Идентификатор плана, к которому относится сегмент.</span><span class="sxs-lookup"><span data-stu-id="0a369-147">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a369-148">Связи</span><span class="sxs-lookup"><span data-stu-id="0a369-148">Relationships</span></span>
| <span data-ttu-id="0a369-149">Связь</span><span class="sxs-lookup"><span data-stu-id="0a369-149">Relationship</span></span> | <span data-ttu-id="0a369-150">Тип</span><span class="sxs-lookup"><span data-stu-id="0a369-150">Type</span></span>   |<span data-ttu-id="0a369-151">Описание</span><span class="sxs-lookup"><span data-stu-id="0a369-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a369-152">tasks</span><span class="sxs-lookup"><span data-stu-id="0a369-152">tasks</span></span>|<span data-ttu-id="0a369-153">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="0a369-153">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="0a369-p106">Только для чтения. Допускает значение null. Коллекция задач в сегменте.</span><span class="sxs-lookup"><span data-stu-id="0a369-p106">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a369-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0a369-157">JSON representation</span></span>
<span data-ttu-id="0a369-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a369-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
