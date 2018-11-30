---
title: Тип ресурса plannerGroup
description: Ресурс **plannerGroup** предоставляет доступ к ресурсам планировщик работы группы. Он не содержит какие-либо можно использовать свойства.
ms.openlocfilehash: 3a2bb9cfd90a36f6b0a2148e0d789ac97b2199fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026849"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="e9961-104">Тип ресурса plannerGroup</span><span class="sxs-lookup"><span data-stu-id="e9961-104">plannerGroup resource type</span></span>

<span data-ttu-id="e9961-p102">Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для [группы](group.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="e9961-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="e9961-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e9961-107">Methods</span></span>

| <span data-ttu-id="e9961-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e9961-108">Method</span></span>           | <span data-ttu-id="e9961-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e9961-109">Return Type</span></span>    |<span data-ttu-id="e9961-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e9961-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e9961-111">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="e9961-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="e9961-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="e9961-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="e9961-113">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="e9961-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e9961-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9961-114">Properties</span></span>
| <span data-ttu-id="e9961-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9961-115">Property</span></span>     | <span data-ttu-id="e9961-116">Тип</span><span class="sxs-lookup"><span data-stu-id="e9961-116">Type</span></span>   |<span data-ttu-id="e9961-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e9961-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9961-118">id</span><span class="sxs-lookup"><span data-stu-id="e9961-118">id</span></span>|<span data-ttu-id="e9961-119">String</span><span class="sxs-lookup"><span data-stu-id="e9961-119">String</span></span>| <span data-ttu-id="e9961-p103">Только для чтения. Идентификатор объекта **plannerGroup**.</span><span class="sxs-lookup"><span data-stu-id="e9961-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9961-122">Связи</span><span class="sxs-lookup"><span data-stu-id="e9961-122">Relationships</span></span>
| <span data-ttu-id="e9961-123">Связь</span><span class="sxs-lookup"><span data-stu-id="e9961-123">Relationship</span></span> | <span data-ttu-id="e9961-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e9961-124">Type</span></span>   |<span data-ttu-id="e9961-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e9961-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9961-126">plans</span><span class="sxs-lookup"><span data-stu-id="e9961-126">plans</span></span>|<span data-ttu-id="e9961-127">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="e9961-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="e9961-p104">Только для чтения. Допускает значение null. Возвращает экземпляры [plannerPlan](plannerplan.md), принадлежащие группе.</span><span class="sxs-lookup"><span data-stu-id="e9961-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9961-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e9961-131">JSON representation</span></span>
<span data-ttu-id="e9961-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9961-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->