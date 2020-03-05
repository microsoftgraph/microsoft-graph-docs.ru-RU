---
title: Тип ресурса Рубриккуалити
description: Качество Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6f900056db140719ff5bc7902a6a7a9531cebe9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521007"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="c2955-103">Тип ресурса Рубриккуалити</span><span class="sxs-lookup"><span data-stu-id="c2955-103">rubricQuality resource type</span></span>

<span data-ttu-id="c2955-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c2955-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2955-105">Качество Rubric.</span><span class="sxs-lookup"><span data-stu-id="c2955-105">A quality of a rubric.</span></span> <span data-ttu-id="c2955-106">Описание связи между Rubric *качеством*, *уровнями*и *критериями*можно узнать в разделе [едукатионрубрик](educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="c2955-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="c2955-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2955-107">Properties</span></span>

| <span data-ttu-id="c2955-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2955-108">Property</span></span>     | <span data-ttu-id="c2955-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2955-109">Type</span></span>        | <span data-ttu-id="c2955-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2955-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c2955-111">criteria</span><span class="sxs-lookup"><span data-stu-id="c2955-111">criteria</span></span>|<span data-ttu-id="c2955-112">Коллекция [рубриккритерион](rubriccriterion.md)</span><span class="sxs-lookup"><span data-stu-id="c2955-112">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="c2955-113">Коллекция критериев для этого качества Rubric.</span><span class="sxs-lookup"><span data-stu-id="c2955-113">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="c2955-114">description</span><span class="sxs-lookup"><span data-stu-id="c2955-114">description</span></span>|[<span data-ttu-id="c2955-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="c2955-115">itemBody</span></span>](itembody.md)|<span data-ttu-id="c2955-116">Описание этого качества Rubric.</span><span class="sxs-lookup"><span data-stu-id="c2955-116">The description of this rubric quality.</span></span>|
|<span data-ttu-id="c2955-117">displayName</span><span class="sxs-lookup"><span data-stu-id="c2955-117">displayName</span></span>|<span data-ttu-id="c2955-118">String</span><span class="sxs-lookup"><span data-stu-id="c2955-118">String</span></span>|<span data-ttu-id="c2955-119">Имя этого rubricного качества.</span><span class="sxs-lookup"><span data-stu-id="c2955-119">The name of this rubric quality.</span></span>|
|<span data-ttu-id="c2955-120">куалитид</span><span class="sxs-lookup"><span data-stu-id="c2955-120">qualityId</span></span>|<span data-ttu-id="c2955-121">String</span><span class="sxs-lookup"><span data-stu-id="c2955-121">String</span></span>|<span data-ttu-id="c2955-122">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="c2955-122">The ID of this resource.</span></span>|
|<span data-ttu-id="c2955-123">weight</span><span class="sxs-lookup"><span data-stu-id="c2955-123">weight</span></span>|<span data-ttu-id="c2955-124">Одинарное</span><span class="sxs-lookup"><span data-stu-id="c2955-124">Single</span></span>|<span data-ttu-id="c2955-125">Если задано, числовой вес для этого качества.</span><span class="sxs-lookup"><span data-stu-id="c2955-125">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="c2955-126">Весовые значения должны добавим до 100.</span><span class="sxs-lookup"><span data-stu-id="c2955-126">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2955-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2955-127">JSON representation</span></span>

<span data-ttu-id="c2955-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2955-128">The following is a JSON representation of the resource.</span></span>

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