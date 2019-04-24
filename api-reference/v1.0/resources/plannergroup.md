---
title: Тип ресурса Планнерграуп
description: Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для группы. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6e60db0a3f33bc47d0ea63b7a773b7bb691cd5be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462377"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="7450f-104">Тип ресурса Планнерграуп</span><span class="sxs-lookup"><span data-stu-id="7450f-104">plannerGroup resource type</span></span>

<span data-ttu-id="7450f-105">Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для [группы](group.md).</span><span class="sxs-lookup"><span data-stu-id="7450f-105">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="7450f-106">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="7450f-106">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="7450f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7450f-107">Methods</span></span>

| <span data-ttu-id="7450f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7450f-108">Method</span></span>           | <span data-ttu-id="7450f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7450f-109">Return Type</span></span>    |<span data-ttu-id="7450f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7450f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7450f-111">Список планов</span><span class="sxs-lookup"><span data-stu-id="7450f-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="7450f-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="7450f-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="7450f-113">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="7450f-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="7450f-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="7450f-114">Properties</span></span>
| <span data-ttu-id="7450f-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="7450f-115">Property</span></span>     | <span data-ttu-id="7450f-116">Тип</span><span class="sxs-lookup"><span data-stu-id="7450f-116">Type</span></span>   |<span data-ttu-id="7450f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="7450f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7450f-118">id</span><span class="sxs-lookup"><span data-stu-id="7450f-118">id</span></span>|<span data-ttu-id="7450f-119">String</span><span class="sxs-lookup"><span data-stu-id="7450f-119">String</span></span>| <span data-ttu-id="7450f-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7450f-120">Read-only.</span></span> <span data-ttu-id="7450f-121">Идентификатор объекта **планнерграуп**</span><span class="sxs-lookup"><span data-stu-id="7450f-121">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="7450f-122">Связи</span><span class="sxs-lookup"><span data-stu-id="7450f-122">Relationships</span></span>
| <span data-ttu-id="7450f-123">Отношение</span><span class="sxs-lookup"><span data-stu-id="7450f-123">Relationship</span></span> | <span data-ttu-id="7450f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7450f-124">Type</span></span>   |<span data-ttu-id="7450f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7450f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7450f-126">планирует</span><span class="sxs-lookup"><span data-stu-id="7450f-126">plans</span></span>|<span data-ttu-id="7450f-127">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="7450f-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="7450f-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7450f-128">Read-only.</span></span> <span data-ttu-id="7450f-129">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7450f-129">Nullable.</span></span> <span data-ttu-id="7450f-130">Возвращает [планов](plannerplan.md) , принадлежащий группе.</span><span class="sxs-lookup"><span data-stu-id="7450f-130">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7450f-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7450f-131">JSON representation</span></span>
<span data-ttu-id="7450f-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7450f-132">Here is a JSON representation of the resource.</span></span>

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
