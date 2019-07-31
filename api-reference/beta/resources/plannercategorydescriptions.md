---
title: Тип ресурса Планнеркатегоридескриптионс
description: 'Ресурс **планнеркатегоридескриптионс** представляет описательные метки для категорий, определенных для плана. Он принадлежит объекту сведений о плане. Может быть определено до 6 категорий. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a8d80be1768cae3383b07c6fbb7dac1e042cc0bd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966029"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="fce49-105">Тип ресурса Планнеркатегоридескриптионс</span><span class="sxs-lookup"><span data-stu-id="fce49-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fce49-106">Ресурс **планнеркатегоридескриптионс** представляет описательные метки для категорий, определенных для плана.</span><span class="sxs-lookup"><span data-stu-id="fce49-106">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="fce49-107">Он принадлежит объекту [сведений о плане](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="fce49-107">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="fce49-108">Может быть определено до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="fce49-108">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="fce49-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fce49-109">Properties</span></span>
| <span data-ttu-id="fce49-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fce49-110">Property</span></span>     | <span data-ttu-id="fce49-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fce49-111">Type</span></span>   |<span data-ttu-id="fce49-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fce49-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fce49-113">Category1</span><span class="sxs-lookup"><span data-stu-id="fce49-113">category1</span></span>|<span data-ttu-id="fce49-114">String</span><span class="sxs-lookup"><span data-stu-id="fce49-114">String</span></span>|<span data-ttu-id="fce49-115">Метка, связанная с категорией 1</span><span class="sxs-lookup"><span data-stu-id="fce49-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="fce49-116">category2</span><span class="sxs-lookup"><span data-stu-id="fce49-116">category2</span></span>|<span data-ttu-id="fce49-117">String</span><span class="sxs-lookup"><span data-stu-id="fce49-117">String</span></span>|<span data-ttu-id="fce49-118">Метка, сопоставленная с категорией 2</span><span class="sxs-lookup"><span data-stu-id="fce49-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="fce49-119">category3</span><span class="sxs-lookup"><span data-stu-id="fce49-119">category3</span></span>|<span data-ttu-id="fce49-120">String</span><span class="sxs-lookup"><span data-stu-id="fce49-120">String</span></span>|<span data-ttu-id="fce49-121">Метка, связанная с категорией 3</span><span class="sxs-lookup"><span data-stu-id="fce49-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="fce49-122">category4</span><span class="sxs-lookup"><span data-stu-id="fce49-122">category4</span></span>|<span data-ttu-id="fce49-123">String</span><span class="sxs-lookup"><span data-stu-id="fce49-123">String</span></span>|<span data-ttu-id="fce49-124">Метка, сопоставленная с категорией 4</span><span class="sxs-lookup"><span data-stu-id="fce49-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="fce49-125">category5</span><span class="sxs-lookup"><span data-stu-id="fce49-125">category5</span></span>|<span data-ttu-id="fce49-126">String</span><span class="sxs-lookup"><span data-stu-id="fce49-126">String</span></span>|<span data-ttu-id="fce49-127">Метка, сопоставленная с категорией 5</span><span class="sxs-lookup"><span data-stu-id="fce49-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="fce49-128">category6</span><span class="sxs-lookup"><span data-stu-id="fce49-128">category6</span></span>|<span data-ttu-id="fce49-129">String</span><span class="sxs-lookup"><span data-stu-id="fce49-129">String</span></span>|<span data-ttu-id="fce49-130">Метка, сопоставленная с категорией 6</span><span class="sxs-lookup"><span data-stu-id="fce49-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fce49-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fce49-131">JSON representation</span></span>
<span data-ttu-id="fce49-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fce49-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
