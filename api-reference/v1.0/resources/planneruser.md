---
title: Тип ресурса plannerUser
description: Ресурс **plannerUser** предоставляют доступ к ресурсам планировщик работы для пользователя. Он не содержит какие-либо можно использовать свойства.
ms.openlocfilehash: 777886a61d702198ec03ea844fb9fced761047ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026494"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="13c0a-104">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="13c0a-104">plannerUser resource type</span></span>

<span data-ttu-id="13c0a-p102">Ресурс **plannerUser** предоставляют доступ к ресурсам Планировщика для [пользователя](user.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="13c0a-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="13c0a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="13c0a-107">Methods</span></span>

| <span data-ttu-id="13c0a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="13c0a-108">Method</span></span>           | <span data-ttu-id="13c0a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13c0a-109">Return Type</span></span>    |<span data-ttu-id="13c0a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="13c0a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13c0a-111">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="13c0a-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="13c0a-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="13c0a-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="13c0a-113">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="13c0a-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="13c0a-114">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="13c0a-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="13c0a-115">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="13c0a-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="13c0a-116">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="13c0a-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="13c0a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="13c0a-117">Properties</span></span>
| <span data-ttu-id="13c0a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="13c0a-118">Property</span></span>     | <span data-ttu-id="13c0a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="13c0a-119">Type</span></span>   |<span data-ttu-id="13c0a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="13c0a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13c0a-121">id</span><span class="sxs-lookup"><span data-stu-id="13c0a-121">id</span></span>|<span data-ttu-id="13c0a-122">String</span><span class="sxs-lookup"><span data-stu-id="13c0a-122">String</span></span>| <span data-ttu-id="13c0a-p103">Только для чтения. Идентификатор объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="13c0a-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="13c0a-125">Связи</span><span class="sxs-lookup"><span data-stu-id="13c0a-125">Relationships</span></span>
| <span data-ttu-id="13c0a-126">Связь</span><span class="sxs-lookup"><span data-stu-id="13c0a-126">Relationship</span></span> | <span data-ttu-id="13c0a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="13c0a-127">Type</span></span>   |<span data-ttu-id="13c0a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="13c0a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13c0a-129">plans</span><span class="sxs-lookup"><span data-stu-id="13c0a-129">plans</span></span>|<span data-ttu-id="13c0a-130">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="13c0a-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="13c0a-p104">Только для чтения. Допускает значение null. Возвращает объекты [plannerTask](plannertask.md), назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="13c0a-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="13c0a-134">tasks</span><span class="sxs-lookup"><span data-stu-id="13c0a-134">tasks</span></span>|<span data-ttu-id="13c0a-135">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="13c0a-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="13c0a-p105">Только для чтения. Допускает значение null. Возвращает объекты [plannerPlan](plannerplan.md), к которым у пользователя есть доступ.</span><span class="sxs-lookup"><span data-stu-id="13c0a-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13c0a-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="13c0a-139">JSON representation</span></span>
<span data-ttu-id="13c0a-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13c0a-140">Here is a JSON representation of the resource.</span></span>

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