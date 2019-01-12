---
title: Тип ресурса plannerGroup
description: Ресурс **plannerGroup** предоставляет доступ к ресурсам планировщик работы группы. Он не содержит какие-либо можно использовать свойства.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6e60db0a3f33bc47d0ea63b7a773b7bb691cd5be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981422"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="f6ca7-104">Тип ресурса plannerGroup</span><span class="sxs-lookup"><span data-stu-id="f6ca7-104">plannerGroup resource type</span></span>

<span data-ttu-id="f6ca7-p102">Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для [группы](group.md). Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="f6ca7-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="f6ca7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f6ca7-107">Methods</span></span>

| <span data-ttu-id="f6ca7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f6ca7-108">Method</span></span>           | <span data-ttu-id="f6ca7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f6ca7-109">Return Type</span></span>    |<span data-ttu-id="f6ca7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ca7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f6ca7-111">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="f6ca7-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="f6ca7-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca7-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f6ca7-113">Получение коллекции объектов **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="f6ca7-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6ca7-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6ca7-114">Properties</span></span>
| <span data-ttu-id="f6ca7-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6ca7-115">Property</span></span>     | <span data-ttu-id="f6ca7-116">Тип</span><span class="sxs-lookup"><span data-stu-id="f6ca7-116">Type</span></span>   |<span data-ttu-id="f6ca7-117">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ca7-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6ca7-118">id</span><span class="sxs-lookup"><span data-stu-id="f6ca7-118">id</span></span>|<span data-ttu-id="f6ca7-119">String</span><span class="sxs-lookup"><span data-stu-id="f6ca7-119">String</span></span>| <span data-ttu-id="f6ca7-p103">Только для чтения. Идентификатор объекта **plannerGroup**.</span><span class="sxs-lookup"><span data-stu-id="f6ca7-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6ca7-122">Связи</span><span class="sxs-lookup"><span data-stu-id="f6ca7-122">Relationships</span></span>
| <span data-ttu-id="f6ca7-123">Связь</span><span class="sxs-lookup"><span data-stu-id="f6ca7-123">Relationship</span></span> | <span data-ttu-id="f6ca7-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f6ca7-124">Type</span></span>   |<span data-ttu-id="f6ca7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ca7-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6ca7-126">plans</span><span class="sxs-lookup"><span data-stu-id="f6ca7-126">plans</span></span>|<span data-ttu-id="f6ca7-127">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca7-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f6ca7-p104">Только для чтения. Допускает значение null. Возвращает экземпляры [plannerPlan](plannerplan.md), принадлежащие группе.</span><span class="sxs-lookup"><span data-stu-id="f6ca7-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6ca7-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f6ca7-131">JSON representation</span></span>
<span data-ttu-id="f6ca7-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6ca7-132">Here is a JSON representation of the resource.</span></span>

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
