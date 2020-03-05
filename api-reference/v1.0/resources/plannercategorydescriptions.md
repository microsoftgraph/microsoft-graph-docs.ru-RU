---
title: Тип ресурса Планнеркатегоридескриптионс
description: 'Ресурс **планнеркатегоридескриптионс** представляет описательные метки для категорий, определенных для плана. Он принадлежит объекту сведений о плане. Может быть определено до 6 категорий. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d0ef4c4f91c4b2f8017a7b7555785c9dd10d082a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447138"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="39983-105">Тип ресурса Планнеркатегоридескриптионс</span><span class="sxs-lookup"><span data-stu-id="39983-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="39983-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="39983-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39983-107">Ресурс **планнеркатегоридескриптионс** представляет описательные метки для категорий, определенных для плана.</span><span class="sxs-lookup"><span data-stu-id="39983-107">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="39983-108">Он принадлежит объекту [сведений о плане](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="39983-108">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="39983-109">Может быть определено до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="39983-109">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="39983-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="39983-110">Properties</span></span>
| <span data-ttu-id="39983-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="39983-111">Property</span></span>     | <span data-ttu-id="39983-112">Тип</span><span class="sxs-lookup"><span data-stu-id="39983-112">Type</span></span>   |<span data-ttu-id="39983-113">Описание</span><span class="sxs-lookup"><span data-stu-id="39983-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39983-114">Category1</span><span class="sxs-lookup"><span data-stu-id="39983-114">category1</span></span>|<span data-ttu-id="39983-115">String</span><span class="sxs-lookup"><span data-stu-id="39983-115">String</span></span>|<span data-ttu-id="39983-116">Метка, связанная с категорией 1</span><span class="sxs-lookup"><span data-stu-id="39983-116">The label associated with Category 1</span></span>|
|<span data-ttu-id="39983-117">category2</span><span class="sxs-lookup"><span data-stu-id="39983-117">category2</span></span>|<span data-ttu-id="39983-118">String</span><span class="sxs-lookup"><span data-stu-id="39983-118">String</span></span>|<span data-ttu-id="39983-119">Метка, сопоставленная с категорией 2</span><span class="sxs-lookup"><span data-stu-id="39983-119">The label associated with Category 2</span></span>|
|<span data-ttu-id="39983-120">category3</span><span class="sxs-lookup"><span data-stu-id="39983-120">category3</span></span>|<span data-ttu-id="39983-121">String</span><span class="sxs-lookup"><span data-stu-id="39983-121">String</span></span>|<span data-ttu-id="39983-122">Метка, связанная с категорией 3</span><span class="sxs-lookup"><span data-stu-id="39983-122">The label associated with Category 3</span></span>|
|<span data-ttu-id="39983-123">category4</span><span class="sxs-lookup"><span data-stu-id="39983-123">category4</span></span>|<span data-ttu-id="39983-124">String</span><span class="sxs-lookup"><span data-stu-id="39983-124">String</span></span>|<span data-ttu-id="39983-125">Метка, сопоставленная с категорией 4</span><span class="sxs-lookup"><span data-stu-id="39983-125">The label associated with Category 4</span></span>|
|<span data-ttu-id="39983-126">category5</span><span class="sxs-lookup"><span data-stu-id="39983-126">category5</span></span>|<span data-ttu-id="39983-127">String</span><span class="sxs-lookup"><span data-stu-id="39983-127">String</span></span>|<span data-ttu-id="39983-128">Метка, сопоставленная с категорией 5</span><span class="sxs-lookup"><span data-stu-id="39983-128">The label associated with Category 5</span></span>|
|<span data-ttu-id="39983-129">category6</span><span class="sxs-lookup"><span data-stu-id="39983-129">category6</span></span>|<span data-ttu-id="39983-130">String</span><span class="sxs-lookup"><span data-stu-id="39983-130">String</span></span>|<span data-ttu-id="39983-131">Метка, сопоставленная с категорией 6</span><span class="sxs-lookup"><span data-stu-id="39983-131">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39983-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39983-132">JSON representation</span></span>
<span data-ttu-id="39983-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39983-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
