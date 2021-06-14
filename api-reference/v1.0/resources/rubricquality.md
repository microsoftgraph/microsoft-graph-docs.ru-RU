---
title: тип ресурса rubricQuality
description: Качество рубрики.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82fdb8fa226ab6eb2c38b1e49e12904ff26b6491
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911522"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="cb98f-103">тип ресурса rubricQuality</span><span class="sxs-lookup"><span data-stu-id="cb98f-103">rubricQuality resource type</span></span>

<span data-ttu-id="cb98f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb98f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb98f-105">Качество рубрики.</span><span class="sxs-lookup"><span data-stu-id="cb98f-105">A quality of a rubric.</span></span> 

<span data-ttu-id="cb98f-106">См. [в рубрике EducationRubric](educationrubric.md) описание взаимосвязи между качествами,  *уровнями* и критериями *рубрики.*</span><span class="sxs-lookup"><span data-stu-id="cb98f-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="cb98f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb98f-107">Properties</span></span>

| <span data-ttu-id="cb98f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb98f-108">Property</span></span>     | <span data-ttu-id="cb98f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cb98f-109">Type</span></span>        | <span data-ttu-id="cb98f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cb98f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb98f-111">criteria</span><span class="sxs-lookup"><span data-stu-id="cb98f-111">criteria</span></span>|<span data-ttu-id="cb98f-112">[rubricCriterion](rubriccriterion.md) collection</span><span class="sxs-lookup"><span data-stu-id="cb98f-112">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="cb98f-113">Набор критериев для этого качества рубрики.</span><span class="sxs-lookup"><span data-stu-id="cb98f-113">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="cb98f-114">description</span><span class="sxs-lookup"><span data-stu-id="cb98f-114">description</span></span>|[<span data-ttu-id="cb98f-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="cb98f-115">itemBody</span></span>](itembody.md)|<span data-ttu-id="cb98f-116">Описание этого качества рубрики.</span><span class="sxs-lookup"><span data-stu-id="cb98f-116">The description of this rubric quality.</span></span>|
|<span data-ttu-id="cb98f-117">displayName</span><span class="sxs-lookup"><span data-stu-id="cb98f-117">displayName</span></span>|<span data-ttu-id="cb98f-118">String</span><span class="sxs-lookup"><span data-stu-id="cb98f-118">String</span></span>|<span data-ttu-id="cb98f-119">Имя этого качества рубрики.</span><span class="sxs-lookup"><span data-stu-id="cb98f-119">The name of this rubric quality.</span></span>|
|<span data-ttu-id="cb98f-120">qualityId</span><span class="sxs-lookup"><span data-stu-id="cb98f-120">qualityId</span></span>|<span data-ttu-id="cb98f-121">String</span><span class="sxs-lookup"><span data-stu-id="cb98f-121">String</span></span>|<span data-ttu-id="cb98f-122">ID этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="cb98f-122">The ID of this resource.</span></span>|
|<span data-ttu-id="cb98f-123">weight</span><span class="sxs-lookup"><span data-stu-id="cb98f-123">weight</span></span>|<span data-ttu-id="cb98f-124">Одинарное</span><span class="sxs-lookup"><span data-stu-id="cb98f-124">Single</span></span>|<span data-ttu-id="cb98f-125">Если есть, то числовой вес для этого качества.</span><span class="sxs-lookup"><span data-stu-id="cb98f-125">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="cb98f-126">Весы должны добавить до 100.</span><span class="sxs-lookup"><span data-stu-id="cb98f-126">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb98f-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb98f-127">JSON representation</span></span>

<span data-ttu-id="cb98f-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb98f-128">The following is a JSON representation of the resource.</span></span>

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

