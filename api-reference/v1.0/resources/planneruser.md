---
title: Тип ресурса plannerUser
description: Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1bdf811e68e6a856d50621d063fe66daecf57748
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037367"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="20f6e-104">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="20f6e-104">plannerUser resource type</span></span>

<span data-ttu-id="20f6e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20f6e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20f6e-106">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="20f6e-106">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="20f6e-107">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="20f6e-107">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="20f6e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="20f6e-108">Methods</span></span>

| <span data-ttu-id="20f6e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="20f6e-109">Method</span></span>           | <span data-ttu-id="20f6e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="20f6e-110">Return Type</span></span>    |<span data-ttu-id="20f6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="20f6e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20f6e-112">Список планов</span><span class="sxs-lookup"><span data-stu-id="20f6e-112">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="20f6e-113">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="20f6e-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="20f6e-114">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="20f6e-114">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="20f6e-115">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="20f6e-115">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="20f6e-116">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="20f6e-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="20f6e-117">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="20f6e-117">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="20f6e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="20f6e-118">Properties</span></span>
| <span data-ttu-id="20f6e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="20f6e-119">Property</span></span>     | <span data-ttu-id="20f6e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="20f6e-120">Type</span></span>   |<span data-ttu-id="20f6e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="20f6e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20f6e-122">id</span><span class="sxs-lookup"><span data-stu-id="20f6e-122">id</span></span>|<span data-ttu-id="20f6e-123">String</span><span class="sxs-lookup"><span data-stu-id="20f6e-123">String</span></span>| <span data-ttu-id="20f6e-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20f6e-124">Read-only.</span></span> <span data-ttu-id="20f6e-125">Идентификатор объекта Планенрусер</span><span class="sxs-lookup"><span data-stu-id="20f6e-125">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="20f6e-126">Связи</span><span class="sxs-lookup"><span data-stu-id="20f6e-126">Relationships</span></span>
| <span data-ttu-id="20f6e-127">Связь</span><span class="sxs-lookup"><span data-stu-id="20f6e-127">Relationship</span></span> | <span data-ttu-id="20f6e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="20f6e-128">Type</span></span>   |<span data-ttu-id="20f6e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="20f6e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20f6e-130">планирует</span><span class="sxs-lookup"><span data-stu-id="20f6e-130">plans</span></span>|<span data-ttu-id="20f6e-131">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="20f6e-131">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="20f6e-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20f6e-132">Read-only.</span></span> <span data-ttu-id="20f6e-133">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="20f6e-133">Nullable.</span></span> <span data-ttu-id="20f6e-134">Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="20f6e-134">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="20f6e-135">tasks</span><span class="sxs-lookup"><span data-stu-id="20f6e-135">tasks</span></span>|<span data-ttu-id="20f6e-136">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="20f6e-136">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="20f6e-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20f6e-137">Read-only.</span></span> <span data-ttu-id="20f6e-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="20f6e-138">Nullable.</span></span> <span data-ttu-id="20f6e-139">Возвращает [планов](plannerplan.md) , предоставленный пользователю.</span><span class="sxs-lookup"><span data-stu-id="20f6e-139">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20f6e-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20f6e-140">JSON representation</span></span>
<span data-ttu-id="20f6e-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20f6e-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

