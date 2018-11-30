---
title: Тип ресурса plannerCategoryDescriptions
description: 'Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту сведений о плане. Можно задать до 6 категорий. '
ms.openlocfilehash: eb54a42cd3e86a9f2c39ff46d45c71fb04142dad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076680"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="9c033-105">Тип ресурса plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="9c033-105">plannerCategoryDescriptions resource type</span></span>

> <span data-ttu-id="9c033-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c033-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c033-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c033-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c033-p103">Ресурс **plannerCategoryDescriptions** представляет описательные метки категорий, заданных для плана. Он принадлежит объекту [сведений о плане](plannerplandetails.md). Можно задать до 6 категорий.</span><span class="sxs-lookup"><span data-stu-id="9c033-p103">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="9c033-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c033-111">Properties</span></span>
| <span data-ttu-id="9c033-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c033-112">Property</span></span>     | <span data-ttu-id="9c033-113">Тип</span><span class="sxs-lookup"><span data-stu-id="9c033-113">Type</span></span>   |<span data-ttu-id="9c033-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9c033-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c033-115">category1</span><span class="sxs-lookup"><span data-stu-id="9c033-115">category1</span></span>|<span data-ttu-id="9c033-116">String</span><span class="sxs-lookup"><span data-stu-id="9c033-116">String</span></span>|<span data-ttu-id="9c033-117">Метка, сопоставленная с категорией 1.</span><span class="sxs-lookup"><span data-stu-id="9c033-117">The label associated with Category 1</span></span>|
|<span data-ttu-id="9c033-118">category2</span><span class="sxs-lookup"><span data-stu-id="9c033-118">category2</span></span>|<span data-ttu-id="9c033-119">String</span><span class="sxs-lookup"><span data-stu-id="9c033-119">String</span></span>|<span data-ttu-id="9c033-120">Метка, сопоставленная с категорией 2.</span><span class="sxs-lookup"><span data-stu-id="9c033-120">The label associated with Category 2</span></span>|
|<span data-ttu-id="9c033-121">category3</span><span class="sxs-lookup"><span data-stu-id="9c033-121">category3</span></span>|<span data-ttu-id="9c033-122">String</span><span class="sxs-lookup"><span data-stu-id="9c033-122">String</span></span>|<span data-ttu-id="9c033-123">Метка, сопоставленная с категорией 3.</span><span class="sxs-lookup"><span data-stu-id="9c033-123">The label associated with Category 3</span></span>|
|<span data-ttu-id="9c033-124">category4</span><span class="sxs-lookup"><span data-stu-id="9c033-124">category4</span></span>|<span data-ttu-id="9c033-125">String</span><span class="sxs-lookup"><span data-stu-id="9c033-125">String</span></span>|<span data-ttu-id="9c033-126">Метка, сопоставленная с категорией 4.</span><span class="sxs-lookup"><span data-stu-id="9c033-126">The label associated with Category 4</span></span>|
|<span data-ttu-id="9c033-127">category5</span><span class="sxs-lookup"><span data-stu-id="9c033-127">category5</span></span>|<span data-ttu-id="9c033-128">String</span><span class="sxs-lookup"><span data-stu-id="9c033-128">String</span></span>|<span data-ttu-id="9c033-129">Метка, сопоставленная с категорией 5.</span><span class="sxs-lookup"><span data-stu-id="9c033-129">The label associated with Category 5</span></span>|
|<span data-ttu-id="9c033-130">category6</span><span class="sxs-lookup"><span data-stu-id="9c033-130">category6</span></span>|<span data-ttu-id="9c033-131">String</span><span class="sxs-lookup"><span data-stu-id="9c033-131">String</span></span>|<span data-ttu-id="9c033-132">Метка, сопоставленная с категорией 6.</span><span class="sxs-lookup"><span data-stu-id="9c033-132">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c033-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9c033-133">JSON representation</span></span>
<span data-ttu-id="9c033-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c033-134">Here is a JSON representation of the resource.</span></span>

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