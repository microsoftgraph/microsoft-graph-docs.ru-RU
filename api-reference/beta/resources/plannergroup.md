---
title: Тип ресурса Планнерграуп
description: Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для группы. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4d20a6d5c4918f729189e95a27bad18d9f872c8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521729"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="511f9-104">Тип ресурса Планнерграуп</span><span class="sxs-lookup"><span data-stu-id="511f9-104">plannerGroup resource type</span></span>

<span data-ttu-id="511f9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="511f9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="511f9-106">Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для [группы](group.md).</span><span class="sxs-lookup"><span data-stu-id="511f9-106">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="511f9-107">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="511f9-107">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="511f9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="511f9-108">Methods</span></span>

| <span data-ttu-id="511f9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="511f9-109">Method</span></span>           | <span data-ttu-id="511f9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="511f9-110">Return Type</span></span>    |<span data-ttu-id="511f9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="511f9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="511f9-112">Список планов</span><span class="sxs-lookup"><span data-stu-id="511f9-112">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="511f9-113">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="511f9-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="511f9-114">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="511f9-114">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="511f9-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="511f9-115">Properties</span></span>
| <span data-ttu-id="511f9-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="511f9-116">Property</span></span>     | <span data-ttu-id="511f9-117">Тип</span><span class="sxs-lookup"><span data-stu-id="511f9-117">Type</span></span>   |<span data-ttu-id="511f9-118">Описание</span><span class="sxs-lookup"><span data-stu-id="511f9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="511f9-119">id</span><span class="sxs-lookup"><span data-stu-id="511f9-119">id</span></span>|<span data-ttu-id="511f9-120">String</span><span class="sxs-lookup"><span data-stu-id="511f9-120">String</span></span>| <span data-ttu-id="511f9-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="511f9-121">Read-only.</span></span> <span data-ttu-id="511f9-122">Идентификатор объекта **планнерграуп**</span><span class="sxs-lookup"><span data-stu-id="511f9-122">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="511f9-123">Связи</span><span class="sxs-lookup"><span data-stu-id="511f9-123">Relationships</span></span>
| <span data-ttu-id="511f9-124">Связь</span><span class="sxs-lookup"><span data-stu-id="511f9-124">Relationship</span></span> | <span data-ttu-id="511f9-125">Тип</span><span class="sxs-lookup"><span data-stu-id="511f9-125">Type</span></span>   |<span data-ttu-id="511f9-126">Описание</span><span class="sxs-lookup"><span data-stu-id="511f9-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="511f9-127">планирует</span><span class="sxs-lookup"><span data-stu-id="511f9-127">plans</span></span>|<span data-ttu-id="511f9-128">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="511f9-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="511f9-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="511f9-129">Read-only.</span></span> <span data-ttu-id="511f9-130">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="511f9-130">Nullable.</span></span> <span data-ttu-id="511f9-131">Возвращает [планов](plannerplan.md) , принадлежащий группе.</span><span class="sxs-lookup"><span data-stu-id="511f9-131">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="511f9-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="511f9-132">JSON representation</span></span>
<span data-ttu-id="511f9-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="511f9-133">Here is a JSON representation of the resource.</span></span>

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
