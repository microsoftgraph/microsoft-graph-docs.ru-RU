---
title: Тип ресурса plannerCategoryDescriptions
description: 'Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту сведений о плане. Можно задать до 6 категорий. '
ms.openlocfilehash: e71cbd1f41d23747691b3738b5a46ff302a72168
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025413"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="fb3b1-105">Тип ресурса plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="fb3b1-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="fb3b1-p102">Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту [сведений о плане](plannerplandetails.md). Можно задать до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="fb3b1-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="fb3b1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb3b1-109">Properties</span></span>
| <span data-ttu-id="fb3b1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb3b1-110">Property</span></span>     | <span data-ttu-id="fb3b1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fb3b1-111">Type</span></span>   |<span data-ttu-id="fb3b1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fb3b1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb3b1-113">category1</span><span class="sxs-lookup"><span data-stu-id="fb3b1-113">category1</span></span>|<span data-ttu-id="fb3b1-114">String</span><span class="sxs-lookup"><span data-stu-id="fb3b1-114">String</span></span>|<span data-ttu-id="fb3b1-115">Метка, сопоставленная с категорией 1.</span><span class="sxs-lookup"><span data-stu-id="fb3b1-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="fb3b1-116">category2</span><span class="sxs-lookup"><span data-stu-id="fb3b1-116">category2</span></span>|<span data-ttu-id="fb3b1-117">String</span><span class="sxs-lookup"><span data-stu-id="fb3b1-117">String</span></span>|<span data-ttu-id="fb3b1-118">Метка, сопоставленная с категорией 2.</span><span class="sxs-lookup"><span data-stu-id="fb3b1-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="fb3b1-119">category3</span><span class="sxs-lookup"><span data-stu-id="fb3b1-119">category3</span></span>|<span data-ttu-id="fb3b1-120">String</span><span class="sxs-lookup"><span data-stu-id="fb3b1-120">String</span></span>|<span data-ttu-id="fb3b1-121">Метка, сопоставленная с категорией 3.</span><span class="sxs-lookup"><span data-stu-id="fb3b1-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="fb3b1-122">category4</span><span class="sxs-lookup"><span data-stu-id="fb3b1-122">category4</span></span>|<span data-ttu-id="fb3b1-123">String</span><span class="sxs-lookup"><span data-stu-id="fb3b1-123">String</span></span>|<span data-ttu-id="fb3b1-124">Метка, сопоставленная с категорией 4.</span><span class="sxs-lookup"><span data-stu-id="fb3b1-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="fb3b1-125">category5</span><span class="sxs-lookup"><span data-stu-id="fb3b1-125">category5</span></span>|<span data-ttu-id="fb3b1-126">String</span><span class="sxs-lookup"><span data-stu-id="fb3b1-126">String</span></span>|<span data-ttu-id="fb3b1-127">Метка, сопоставленная с категорией 5.</span><span class="sxs-lookup"><span data-stu-id="fb3b1-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="fb3b1-128">category6</span><span class="sxs-lookup"><span data-stu-id="fb3b1-128">category6</span></span>|<span data-ttu-id="fb3b1-129">String</span><span class="sxs-lookup"><span data-stu-id="fb3b1-129">String</span></span>|<span data-ttu-id="fb3b1-130">Метка, сопоставленная с категорией 6.</span><span class="sxs-lookup"><span data-stu-id="fb3b1-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb3b1-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fb3b1-131">JSON representation</span></span>
<span data-ttu-id="fb3b1-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb3b1-132">Here is a JSON representation of the resource.</span></span>

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