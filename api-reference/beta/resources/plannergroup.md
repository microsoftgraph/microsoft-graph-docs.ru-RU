---
title: Тип ресурса Планнерграуп
description: Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для группы. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 043cec9c3953f8c78a37e141a7b0f1259eb89d52
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344482"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="3e8c3-104">Тип ресурса Планнерграуп</span><span class="sxs-lookup"><span data-stu-id="3e8c3-104">plannerGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e8c3-105">Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для [группы](group.md).</span><span class="sxs-lookup"><span data-stu-id="3e8c3-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="3e8c3-106">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="3e8c3-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="3e8c3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3e8c3-107">Methods</span></span>

| <span data-ttu-id="3e8c3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3e8c3-108">Method</span></span>           | <span data-ttu-id="3e8c3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3e8c3-109">Return Type</span></span>    |<span data-ttu-id="3e8c3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e8c3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3e8c3-111">Список планов</span><span class="sxs-lookup"><span data-stu-id="3e8c3-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="3e8c3-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3e8c3-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3e8c3-113">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="3e8c3-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e8c3-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e8c3-114">Properties</span></span>
| <span data-ttu-id="3e8c3-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e8c3-115">Property</span></span>     | <span data-ttu-id="3e8c3-116">Тип</span><span class="sxs-lookup"><span data-stu-id="3e8c3-116">Type</span></span>   |<span data-ttu-id="3e8c3-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3e8c3-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e8c3-118">id</span><span class="sxs-lookup"><span data-stu-id="3e8c3-118">id</span></span>|<span data-ttu-id="3e8c3-119">String</span><span class="sxs-lookup"><span data-stu-id="3e8c3-119">String</span></span>| <span data-ttu-id="3e8c3-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e8c3-120">Read-only.</span></span> <span data-ttu-id="3e8c3-121">Идентификатор объекта **планнерграуп**</span><span class="sxs-lookup"><span data-stu-id="3e8c3-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e8c3-122">Связи</span><span class="sxs-lookup"><span data-stu-id="3e8c3-122">Relationships</span></span>
| <span data-ttu-id="3e8c3-123">Отношение</span><span class="sxs-lookup"><span data-stu-id="3e8c3-123">Relationship</span></span> | <span data-ttu-id="3e8c3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3e8c3-124">Type</span></span>   |<span data-ttu-id="3e8c3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3e8c3-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e8c3-126">планирует</span><span class="sxs-lookup"><span data-stu-id="3e8c3-126">plans</span></span>|<span data-ttu-id="3e8c3-127">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3e8c3-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3e8c3-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e8c3-128">Read-only.</span></span> <span data-ttu-id="3e8c3-129">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="3e8c3-129">Nullable.</span></span> <span data-ttu-id="3e8c3-130">Возвращает [планов](plannerplan.md) , принадлежащий группе.</span><span class="sxs-lookup"><span data-stu-id="3e8c3-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e8c3-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e8c3-131">JSON representation</span></span>
<span data-ttu-id="3e8c3-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e8c3-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
