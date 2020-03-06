---
title: Тип ресурса Планнерграуп
description: Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для группы. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d7b495575eafbea877df79a6b8a5fb83b0ad2060
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533998"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="0b6f8-104">Тип ресурса Планнерграуп</span><span class="sxs-lookup"><span data-stu-id="0b6f8-104">plannerGroup resource type</span></span>

<span data-ttu-id="0b6f8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b6f8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b6f8-106">Ресурс **планнерграуп** предоставляет доступ к ресурсам планировщика для [группы](group.md).</span><span class="sxs-lookup"><span data-stu-id="0b6f8-106">The **plannerGroup** resource provides access to Planner resources for a [group](group.md).</span></span> <span data-ttu-id="0b6f8-107">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="0b6f8-107">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="0b6f8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0b6f8-108">Methods</span></span>

| <span data-ttu-id="0b6f8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0b6f8-109">Method</span></span>           | <span data-ttu-id="0b6f8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0b6f8-110">Return Type</span></span>    |<span data-ttu-id="0b6f8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0b6f8-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b6f8-112">Список планов</span><span class="sxs-lookup"><span data-stu-id="0b6f8-112">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="0b6f8-113">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="0b6f8-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="0b6f8-114">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="0b6f8-114">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b6f8-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b6f8-115">Properties</span></span>
| <span data-ttu-id="0b6f8-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b6f8-116">Property</span></span>     | <span data-ttu-id="0b6f8-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0b6f8-117">Type</span></span>   |<span data-ttu-id="0b6f8-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0b6f8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b6f8-119">id</span><span class="sxs-lookup"><span data-stu-id="0b6f8-119">id</span></span>|<span data-ttu-id="0b6f8-120">String</span><span class="sxs-lookup"><span data-stu-id="0b6f8-120">String</span></span>| <span data-ttu-id="0b6f8-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b6f8-121">Read-only.</span></span> <span data-ttu-id="0b6f8-122">Идентификатор объекта **планнерграуп**</span><span class="sxs-lookup"><span data-stu-id="0b6f8-122">Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b6f8-123">Связи</span><span class="sxs-lookup"><span data-stu-id="0b6f8-123">Relationships</span></span>
| <span data-ttu-id="0b6f8-124">Связь</span><span class="sxs-lookup"><span data-stu-id="0b6f8-124">Relationship</span></span> | <span data-ttu-id="0b6f8-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0b6f8-125">Type</span></span>   |<span data-ttu-id="0b6f8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0b6f8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b6f8-127">планирует</span><span class="sxs-lookup"><span data-stu-id="0b6f8-127">plans</span></span>|<span data-ttu-id="0b6f8-128">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="0b6f8-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="0b6f8-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b6f8-129">Read-only.</span></span> <span data-ttu-id="0b6f8-130">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0b6f8-130">Nullable.</span></span> <span data-ttu-id="0b6f8-131">Возвращает [планов](plannerplan.md) , принадлежащий группе.</span><span class="sxs-lookup"><span data-stu-id="0b6f8-131">Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b6f8-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b6f8-132">JSON representation</span></span>
<span data-ttu-id="0b6f8-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b6f8-133">Here is a JSON representation of the resource.</span></span>

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
