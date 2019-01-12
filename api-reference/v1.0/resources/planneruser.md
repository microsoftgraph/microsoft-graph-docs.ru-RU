---
title: Тип ресурса plannerUser
description: Ресурс **plannerUser** предоставляют доступ к ресурсам планировщик работы для пользователя. Он не содержит какие-либо можно использовать свойства.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953567"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="df619-104">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="df619-104">plannerUser resource type</span></span>

<span data-ttu-id="df619-p102">Ресурс **plannerUser** предоставляют доступ к ресурсам Планировщика для [пользователя](user.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="df619-p102">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="df619-107">Методы</span><span class="sxs-lookup"><span data-stu-id="df619-107">Methods</span></span>

| <span data-ttu-id="df619-108">Метод</span><span class="sxs-lookup"><span data-stu-id="df619-108">Method</span></span>           | <span data-ttu-id="df619-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="df619-109">Return Type</span></span>    |<span data-ttu-id="df619-110">Описание</span><span class="sxs-lookup"><span data-stu-id="df619-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df619-111">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="df619-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="df619-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="df619-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="df619-113">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="df619-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="df619-114">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="df619-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="df619-115">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="df619-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="df619-116">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="df619-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="df619-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="df619-117">Properties</span></span>
| <span data-ttu-id="df619-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="df619-118">Property</span></span>     | <span data-ttu-id="df619-119">Тип</span><span class="sxs-lookup"><span data-stu-id="df619-119">Type</span></span>   |<span data-ttu-id="df619-120">Описание</span><span class="sxs-lookup"><span data-stu-id="df619-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df619-121">id</span><span class="sxs-lookup"><span data-stu-id="df619-121">id</span></span>|<span data-ttu-id="df619-122">String</span><span class="sxs-lookup"><span data-stu-id="df619-122">String</span></span>| <span data-ttu-id="df619-p103">Только для чтения. Идентификатор объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="df619-p103">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="df619-125">Связи</span><span class="sxs-lookup"><span data-stu-id="df619-125">Relationships</span></span>
| <span data-ttu-id="df619-126">Связь</span><span class="sxs-lookup"><span data-stu-id="df619-126">Relationship</span></span> | <span data-ttu-id="df619-127">Тип</span><span class="sxs-lookup"><span data-stu-id="df619-127">Type</span></span>   |<span data-ttu-id="df619-128">Описание</span><span class="sxs-lookup"><span data-stu-id="df619-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df619-129">plans</span><span class="sxs-lookup"><span data-stu-id="df619-129">plans</span></span>|<span data-ttu-id="df619-130">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="df619-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="df619-p104">Только для чтения. Допускает значение null. Возвращает объекты [plannerTask](plannertask.md), назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="df619-p104">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="df619-134">tasks</span><span class="sxs-lookup"><span data-stu-id="df619-134">tasks</span></span>|<span data-ttu-id="df619-135">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="df619-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="df619-p105">Только для чтения. Допускает значение null. Возвращает объекты [plannerPlan](plannerplan.md), к которым у пользователя есть доступ.</span><span class="sxs-lookup"><span data-stu-id="df619-p105">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df619-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="df619-139">JSON representation</span></span>
<span data-ttu-id="df619-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df619-140">Here is a JSON representation of the resource.</span></span>

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
