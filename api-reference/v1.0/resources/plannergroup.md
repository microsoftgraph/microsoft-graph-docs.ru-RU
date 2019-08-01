---
title: Тип ресурса Планнерграуп
description: Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для группы. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 65d0e81eede4f5edf75a43eaa662e9c044674624
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035240"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="ea8b0-104">Тип ресурса Планнерграуп</span><span class="sxs-lookup"><span data-stu-id="ea8b0-104">plannerGroup resource type</span></span>

<span data-ttu-id="ea8b0-105">Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для [группы](group.md).</span><span class="sxs-lookup"><span data-stu-id="ea8b0-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="ea8b0-106">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="ea8b0-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="ea8b0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ea8b0-107">Methods</span></span>

| <span data-ttu-id="ea8b0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ea8b0-108">Method</span></span>           | <span data-ttu-id="ea8b0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ea8b0-109">Return Type</span></span>    |<span data-ttu-id="ea8b0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ea8b0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea8b0-111">Список планов</span><span class="sxs-lookup"><span data-stu-id="ea8b0-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="ea8b0-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ea8b0-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ea8b0-113">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="ea8b0-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea8b0-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea8b0-114">Properties</span></span>
| <span data-ttu-id="ea8b0-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea8b0-115">Property</span></span>     | <span data-ttu-id="ea8b0-116">Тип</span><span class="sxs-lookup"><span data-stu-id="ea8b0-116">Type</span></span>   |<span data-ttu-id="ea8b0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ea8b0-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea8b0-118">id</span><span class="sxs-lookup"><span data-stu-id="ea8b0-118">id</span></span>|<span data-ttu-id="ea8b0-119">String</span><span class="sxs-lookup"><span data-stu-id="ea8b0-119">String</span></span>| <span data-ttu-id="ea8b0-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea8b0-120">Read-only.</span></span> <span data-ttu-id="ea8b0-121">Идентификатор объекта **планнерграуп**</span><span class="sxs-lookup"><span data-stu-id="ea8b0-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea8b0-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="ea8b0-122">Relationships</span></span>
| <span data-ttu-id="ea8b0-123">Отношение</span><span class="sxs-lookup"><span data-stu-id="ea8b0-123">Relationship</span></span> | <span data-ttu-id="ea8b0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ea8b0-124">Type</span></span>   |<span data-ttu-id="ea8b0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ea8b0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea8b0-126">планирует</span><span class="sxs-lookup"><span data-stu-id="ea8b0-126">plans</span></span>|<span data-ttu-id="ea8b0-127">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="ea8b0-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="ea8b0-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea8b0-128">Read-only.</span></span> <span data-ttu-id="ea8b0-129">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ea8b0-129">Nullable.</span></span> <span data-ttu-id="ea8b0-130">Возвращает [планов](plannerplan.md) , принадлежащий группе.</span><span class="sxs-lookup"><span data-stu-id="ea8b0-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea8b0-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea8b0-131">JSON representation</span></span>
<span data-ttu-id="ea8b0-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea8b0-132">Here is a JSON representation of the resource.</span></span>

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
