---
title: Тип ресурса plannerUser
description: Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549827"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="bdc71-104">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="bdc71-104">plannerUser resource type</span></span>

<span data-ttu-id="bdc71-105">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="bdc71-105">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="bdc71-106">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="bdc71-106">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="bdc71-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bdc71-107">Methods</span></span>

| <span data-ttu-id="bdc71-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bdc71-108">Method</span></span>           | <span data-ttu-id="bdc71-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bdc71-109">Return Type</span></span>    |<span data-ttu-id="bdc71-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bdc71-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdc71-111">Список планов</span><span class="sxs-lookup"><span data-stu-id="bdc71-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="bdc71-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="bdc71-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="bdc71-113">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="bdc71-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="bdc71-114">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="bdc71-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="bdc71-115">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="bdc71-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="bdc71-116">Получение коллекции объектов **plannerTask** .</span><span class="sxs-lookup"><span data-stu-id="bdc71-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="bdc71-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="bdc71-117">Properties</span></span>
| <span data-ttu-id="bdc71-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdc71-118">Property</span></span>     | <span data-ttu-id="bdc71-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bdc71-119">Type</span></span>   |<span data-ttu-id="bdc71-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bdc71-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdc71-121">id</span><span class="sxs-lookup"><span data-stu-id="bdc71-121">id</span></span>|<span data-ttu-id="bdc71-122">String</span><span class="sxs-lookup"><span data-stu-id="bdc71-122">String</span></span>| <span data-ttu-id="bdc71-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdc71-123">Read-only.</span></span> <span data-ttu-id="bdc71-124">Идентификатор объекта Планенрусер</span><span class="sxs-lookup"><span data-stu-id="bdc71-124">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdc71-125">Связи</span><span class="sxs-lookup"><span data-stu-id="bdc71-125">Relationships</span></span>
| <span data-ttu-id="bdc71-126">Отношение</span><span class="sxs-lookup"><span data-stu-id="bdc71-126">Relationship</span></span> | <span data-ttu-id="bdc71-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bdc71-127">Type</span></span>   |<span data-ttu-id="bdc71-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bdc71-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdc71-129">планирует</span><span class="sxs-lookup"><span data-stu-id="bdc71-129">plans</span></span>|<span data-ttu-id="bdc71-130">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="bdc71-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="bdc71-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdc71-131">Read-only.</span></span> <span data-ttu-id="bdc71-132">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bdc71-132">Nullable.</span></span> <span data-ttu-id="bdc71-133">Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="bdc71-133">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="bdc71-134">tasks</span><span class="sxs-lookup"><span data-stu-id="bdc71-134">tasks</span></span>|<span data-ttu-id="bdc71-135">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="bdc71-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="bdc71-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdc71-136">Read-only.</span></span> <span data-ttu-id="bdc71-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bdc71-137">Nullable.</span></span> <span data-ttu-id="bdc71-138">Возвращает [планов](plannerplan.md) , предоставленный пользователю.</span><span class="sxs-lookup"><span data-stu-id="bdc71-138">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdc71-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bdc71-139">JSON representation</span></span>
<span data-ttu-id="bdc71-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdc71-140">Here is a JSON representation of the resource.</span></span>

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
