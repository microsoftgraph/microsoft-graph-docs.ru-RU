---
title: Тип ресурса plannerCategoryDescriptions
description: 'Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту сведений о плане. Можно задать до 6 категорий. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 33031dc3c688e1fefb34109cb0a4a303dbe1c183
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521238"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="85866-105">Тип ресурса plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="85866-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85866-p102">Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту [сведений о плане](plannerplandetails.md). Можно задать до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="85866-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="85866-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="85866-109">Properties</span></span>
| <span data-ttu-id="85866-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="85866-110">Property</span></span>     | <span data-ttu-id="85866-111">Тип</span><span class="sxs-lookup"><span data-stu-id="85866-111">Type</span></span>   |<span data-ttu-id="85866-112">Описание</span><span class="sxs-lookup"><span data-stu-id="85866-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85866-113">category1</span><span class="sxs-lookup"><span data-stu-id="85866-113">category1</span></span>|<span data-ttu-id="85866-114">String</span><span class="sxs-lookup"><span data-stu-id="85866-114">String</span></span>|<span data-ttu-id="85866-115">Метка, сопоставленная с категорией 1.</span><span class="sxs-lookup"><span data-stu-id="85866-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="85866-116">category2</span><span class="sxs-lookup"><span data-stu-id="85866-116">category2</span></span>|<span data-ttu-id="85866-117">String</span><span class="sxs-lookup"><span data-stu-id="85866-117">String</span></span>|<span data-ttu-id="85866-118">Метка, сопоставленная с категорией 2.</span><span class="sxs-lookup"><span data-stu-id="85866-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="85866-119">category3</span><span class="sxs-lookup"><span data-stu-id="85866-119">category3</span></span>|<span data-ttu-id="85866-120">String</span><span class="sxs-lookup"><span data-stu-id="85866-120">String</span></span>|<span data-ttu-id="85866-121">Метка, сопоставленная с категорией 3.</span><span class="sxs-lookup"><span data-stu-id="85866-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="85866-122">category4</span><span class="sxs-lookup"><span data-stu-id="85866-122">category4</span></span>|<span data-ttu-id="85866-123">String</span><span class="sxs-lookup"><span data-stu-id="85866-123">String</span></span>|<span data-ttu-id="85866-124">Метка, сопоставленная с категорией 4.</span><span class="sxs-lookup"><span data-stu-id="85866-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="85866-125">category5</span><span class="sxs-lookup"><span data-stu-id="85866-125">category5</span></span>|<span data-ttu-id="85866-126">String</span><span class="sxs-lookup"><span data-stu-id="85866-126">String</span></span>|<span data-ttu-id="85866-127">Метка, сопоставленная с категорией 5.</span><span class="sxs-lookup"><span data-stu-id="85866-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="85866-128">category6</span><span class="sxs-lookup"><span data-stu-id="85866-128">category6</span></span>|<span data-ttu-id="85866-129">String</span><span class="sxs-lookup"><span data-stu-id="85866-129">String</span></span>|<span data-ttu-id="85866-130">Метка, сопоставленная с категорией 6.</span><span class="sxs-lookup"><span data-stu-id="85866-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85866-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="85866-131">JSON representation</span></span>
<span data-ttu-id="85866-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85866-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannercategorydescriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
