---
title: Тип ресурса Планнеркатегоридескриптионс
description: 'Ресурс **планнеркатегоридескриптионс** представляет описательные метки для категорий, определенных для плана. Он принадлежит объекту сведений о плане. Может быть определено до 6 категорий. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1cf1ee1c6e8ccc4e90f78985b352062fce37df88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462265"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="cc082-105">Тип ресурса Планнеркатегоридескриптионс</span><span class="sxs-lookup"><span data-stu-id="cc082-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc082-106">Ресурс **планнеркатегоридескриптионс** представляет описательные метки для категорий, определенных для плана.</span><span class="sxs-lookup"><span data-stu-id="cc082-106">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="cc082-107">Он принадлежит объекту [сведений о плане](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="cc082-107">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="cc082-108">Может быть определено до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="cc082-108">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="cc082-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc082-109">Properties</span></span>
| <span data-ttu-id="cc082-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc082-110">Property</span></span>     | <span data-ttu-id="cc082-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cc082-111">Type</span></span>   |<span data-ttu-id="cc082-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cc082-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc082-113">Category1</span><span class="sxs-lookup"><span data-stu-id="cc082-113">category1</span></span>|<span data-ttu-id="cc082-114">String</span><span class="sxs-lookup"><span data-stu-id="cc082-114">String</span></span>|<span data-ttu-id="cc082-115">Метка, связанная с категорией 1</span><span class="sxs-lookup"><span data-stu-id="cc082-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="cc082-116">category2</span><span class="sxs-lookup"><span data-stu-id="cc082-116">category2</span></span>|<span data-ttu-id="cc082-117">String</span><span class="sxs-lookup"><span data-stu-id="cc082-117">String</span></span>|<span data-ttu-id="cc082-118">Метка, сопоставленная с категорией 2</span><span class="sxs-lookup"><span data-stu-id="cc082-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="cc082-119">Category3</span><span class="sxs-lookup"><span data-stu-id="cc082-119">category3</span></span>|<span data-ttu-id="cc082-120">String</span><span class="sxs-lookup"><span data-stu-id="cc082-120">String</span></span>|<span data-ttu-id="cc082-121">Метка, связанная с категорией 3</span><span class="sxs-lookup"><span data-stu-id="cc082-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="cc082-122">category4</span><span class="sxs-lookup"><span data-stu-id="cc082-122">category4</span></span>|<span data-ttu-id="cc082-123">String</span><span class="sxs-lookup"><span data-stu-id="cc082-123">String</span></span>|<span data-ttu-id="cc082-124">Метка, сопоставленная с категорией 4</span><span class="sxs-lookup"><span data-stu-id="cc082-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="cc082-125">category5</span><span class="sxs-lookup"><span data-stu-id="cc082-125">category5</span></span>|<span data-ttu-id="cc082-126">String</span><span class="sxs-lookup"><span data-stu-id="cc082-126">String</span></span>|<span data-ttu-id="cc082-127">Метка, сопоставленная с категорией 5</span><span class="sxs-lookup"><span data-stu-id="cc082-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="cc082-128">category6</span><span class="sxs-lookup"><span data-stu-id="cc082-128">category6</span></span>|<span data-ttu-id="cc082-129">String</span><span class="sxs-lookup"><span data-stu-id="cc082-129">String</span></span>|<span data-ttu-id="cc082-130">Метка, сопоставленная с категорией 6</span><span class="sxs-lookup"><span data-stu-id="cc082-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc082-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc082-131">JSON representation</span></span>
<span data-ttu-id="cc082-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc082-132">Here is a JSON representation of the resource.</span></span>

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
