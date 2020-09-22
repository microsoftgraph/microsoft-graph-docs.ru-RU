---
title: Тип ресурса Планнерграуп
description: Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для группы. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6b4a282dcefe06ade0d4af1bb911449b168ac00c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067230"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="1859d-104">Тип ресурса Планнерграуп</span><span class="sxs-lookup"><span data-stu-id="1859d-104">plannerGroup resource type</span></span>

<span data-ttu-id="1859d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1859d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1859d-106">Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для [группы](group.md).</span><span class="sxs-lookup"><span data-stu-id="1859d-106">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="1859d-107">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="1859d-107">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="1859d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1859d-108">Methods</span></span>

| <span data-ttu-id="1859d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1859d-109">Method</span></span>           | <span data-ttu-id="1859d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1859d-110">Return Type</span></span>    |<span data-ttu-id="1859d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1859d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1859d-112">Список планов</span><span class="sxs-lookup"><span data-stu-id="1859d-112">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="1859d-113">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="1859d-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1859d-114">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="1859d-114">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="1859d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="1859d-115">Properties</span></span>
| <span data-ttu-id="1859d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="1859d-116">Property</span></span>     | <span data-ttu-id="1859d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1859d-117">Type</span></span>   |<span data-ttu-id="1859d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1859d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1859d-119">id</span><span class="sxs-lookup"><span data-stu-id="1859d-119">id</span></span>|<span data-ttu-id="1859d-120">String</span><span class="sxs-lookup"><span data-stu-id="1859d-120">String</span></span>| <span data-ttu-id="1859d-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1859d-121">Read-only.</span></span> <span data-ttu-id="1859d-122">Идентификатор объекта **планнерграуп**</span><span class="sxs-lookup"><span data-stu-id="1859d-122">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="1859d-123">Связи</span><span class="sxs-lookup"><span data-stu-id="1859d-123">Relationships</span></span>
| <span data-ttu-id="1859d-124">Связь</span><span class="sxs-lookup"><span data-stu-id="1859d-124">Relationship</span></span> | <span data-ttu-id="1859d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="1859d-125">Type</span></span>   |<span data-ttu-id="1859d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="1859d-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1859d-127">планирует</span><span class="sxs-lookup"><span data-stu-id="1859d-127">plans</span></span>|<span data-ttu-id="1859d-128">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="1859d-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1859d-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1859d-129">Read-only.</span></span> <span data-ttu-id="1859d-130">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1859d-130">Nullable.</span></span> <span data-ttu-id="1859d-131">Возвращает [планов](plannerplan.md) , принадлежащий группе.</span><span class="sxs-lookup"><span data-stu-id="1859d-131">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1859d-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1859d-132">JSON representation</span></span>
<span data-ttu-id="1859d-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1859d-133">Here is a JSON representation of the resource.</span></span>

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


