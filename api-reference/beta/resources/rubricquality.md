---
title: Тип ресурса Рубриккуалити
description: Качество Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e63fd8ad7aa7d0a19fe1774e18bba5d59af52140
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173309"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="082bd-103">Тип ресурса Рубриккуалити</span><span class="sxs-lookup"><span data-stu-id="082bd-103">rubricQuality resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="082bd-104">Качество Rubric.</span><span class="sxs-lookup"><span data-stu-id="082bd-104">A quality of a rubric.</span></span> <span data-ttu-id="082bd-105">Описание связи между Rubric *качеством*, *уровнями*и критериями можно узнать в разделе \*\* [едукатионрубрик](educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="082bd-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="082bd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="082bd-106">Properties</span></span>

| <span data-ttu-id="082bd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="082bd-107">Property</span></span>     | <span data-ttu-id="082bd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="082bd-108">Type</span></span>        | <span data-ttu-id="082bd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="082bd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="082bd-110">criteria</span><span class="sxs-lookup"><span data-stu-id="082bd-110">criteria</span></span>|<span data-ttu-id="082bd-111">Коллекция [рубриккритерион](rubriccriterion.md)</span><span class="sxs-lookup"><span data-stu-id="082bd-111">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="082bd-112">Коллекция критериев для этого качества Rubric.</span><span class="sxs-lookup"><span data-stu-id="082bd-112">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="082bd-113">description</span><span class="sxs-lookup"><span data-stu-id="082bd-113">description</span></span>|[<span data-ttu-id="082bd-114">itemBody</span><span class="sxs-lookup"><span data-stu-id="082bd-114">itemBody</span></span>](itembody.md)|<span data-ttu-id="082bd-115">Описание этого качества Rubric.</span><span class="sxs-lookup"><span data-stu-id="082bd-115">The description of this rubric quality.</span></span>|
|<span data-ttu-id="082bd-116">displayName</span><span class="sxs-lookup"><span data-stu-id="082bd-116">displayName</span></span>|<span data-ttu-id="082bd-117">String</span><span class="sxs-lookup"><span data-stu-id="082bd-117">String</span></span>|<span data-ttu-id="082bd-118">Имя этого rubricного качества.</span><span class="sxs-lookup"><span data-stu-id="082bd-118">The name of this rubric quality.</span></span>|
|<span data-ttu-id="082bd-119">Куалитид</span><span class="sxs-lookup"><span data-stu-id="082bd-119">qualityId</span></span>|<span data-ttu-id="082bd-120">String</span><span class="sxs-lookup"><span data-stu-id="082bd-120">String</span></span>|<span data-ttu-id="082bd-121">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="082bd-121">The ID of this resource.</span></span>|
|<span data-ttu-id="082bd-122">weight</span><span class="sxs-lookup"><span data-stu-id="082bd-122">weight</span></span>|<span data-ttu-id="082bd-123">Одинарное</span><span class="sxs-lookup"><span data-stu-id="082bd-123">Single</span></span>|<span data-ttu-id="082bd-124">Если задано, числовой вес для этого качества.</span><span class="sxs-lookup"><span data-stu-id="082bd-124">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="082bd-125">Весовые значения должны добавим до 100.</span><span class="sxs-lookup"><span data-stu-id="082bd-125">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="082bd-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="082bd-126">JSON representation</span></span>

<span data-ttu-id="082bd-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="082bd-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->