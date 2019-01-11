---
title: Тип ресурса plannerUser
description: Ресурс **plannerUser** предоставляют доступ к ресурсам планировщик работы для пользователя. Он не содержит какие-либо можно использовать свойства.
localization_priority: Normal
ms.openlocfilehash: 733c20d45e1c0b1e0e454b2c5ae03105a9ab5d24
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805945"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="ae109-104">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="ae109-104">plannerUser resource type</span></span>

<span data-ttu-id="ae109-p102">Ресурс **plannerUser** предоставляют доступ к ресурсам Планировщика для [пользователя](user.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="ae109-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="ae109-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ae109-107">Methods</span></span>

| <span data-ttu-id="ae109-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ae109-108">Method</span></span>           | <span data-ttu-id="ae109-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ae109-109">Return Type</span></span>    |<span data-ttu-id="ae109-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ae109-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae109-111">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="ae109-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="ae109-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ae109-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ae109-113">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="ae109-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="ae109-114">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="ae109-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="ae109-115">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ae109-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ae109-116">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="ae109-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae109-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae109-117">Properties</span></span>
| <span data-ttu-id="ae109-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae109-118">Property</span></span>     | <span data-ttu-id="ae109-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ae109-119">Type</span></span>   |<span data-ttu-id="ae109-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae109-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae109-121">id</span><span class="sxs-lookup"><span data-stu-id="ae109-121">id</span></span>|<span data-ttu-id="ae109-122">String</span><span class="sxs-lookup"><span data-stu-id="ae109-122">String</span></span>| <span data-ttu-id="ae109-p103">Только для чтения. Идентификатор объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="ae109-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae109-125">Связи</span><span class="sxs-lookup"><span data-stu-id="ae109-125">Relationships</span></span>
| <span data-ttu-id="ae109-126">Связь</span><span class="sxs-lookup"><span data-stu-id="ae109-126">Relationship</span></span> | <span data-ttu-id="ae109-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ae109-127">Type</span></span>   |<span data-ttu-id="ae109-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ae109-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae109-129">plans</span><span class="sxs-lookup"><span data-stu-id="ae109-129">plans</span></span>|<span data-ttu-id="ae109-130">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ae109-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ae109-p104">Только для чтения. Допускает значение null. Возвращает объекты [plannerTask](plannertask.md), назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="ae109-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="ae109-134">tasks</span><span class="sxs-lookup"><span data-stu-id="ae109-134">tasks</span></span>|<span data-ttu-id="ae109-135">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="ae109-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="ae109-p105">Только для чтения. Допускает значение null. Возвращает объекты [plannerPlan](plannerplan.md), к которым у пользователя есть доступ.</span><span class="sxs-lookup"><span data-stu-id="ae109-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae109-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ae109-139">JSON representation</span></span>
<span data-ttu-id="ae109-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae109-140">Here is a JSON representation of the resource.</span></span>

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
