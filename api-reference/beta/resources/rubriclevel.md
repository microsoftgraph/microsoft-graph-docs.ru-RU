---
title: Тип ресурса Рубриклевел
description: Уровень Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 14a7c084aad907ce2e5f90b06f17b64aca9c331e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016114"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="708b4-103">Тип ресурса Рубриклевел</span><span class="sxs-lookup"><span data-stu-id="708b4-103">rubricLevel resource type</span></span>

<span data-ttu-id="708b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="708b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="708b4-105">Уровень Rubric.</span><span class="sxs-lookup"><span data-stu-id="708b4-105">A level of a rubric.</span></span> <span data-ttu-id="708b4-106">Описание связи между Rubric *качеством*, *уровнями*и *критериями*можно узнать в разделе [едукатионрубрик](educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="708b4-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="708b4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="708b4-107">Properties</span></span>

| <span data-ttu-id="708b4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="708b4-108">Property</span></span>     | <span data-ttu-id="708b4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="708b4-109">Type</span></span>        | <span data-ttu-id="708b4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="708b4-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="708b4-111">description</span><span class="sxs-lookup"><span data-stu-id="708b4-111">description</span></span>|[<span data-ttu-id="708b4-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="708b4-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="708b4-113">Описание этого уровня Rubric.</span><span class="sxs-lookup"><span data-stu-id="708b4-113">The description of this rubric level.</span></span>|
|<span data-ttu-id="708b4-114">displayName</span><span class="sxs-lookup"><span data-stu-id="708b4-114">displayName</span></span>|<span data-ttu-id="708b4-115">String</span><span class="sxs-lookup"><span data-stu-id="708b4-115">String</span></span>|<span data-ttu-id="708b4-116">Имя этого уровня Rubric.</span><span class="sxs-lookup"><span data-stu-id="708b4-116">The name of this rubric level.</span></span>|
|<span data-ttu-id="708b4-117">снижения</span><span class="sxs-lookup"><span data-stu-id="708b4-117">grading</span></span>|[<span data-ttu-id="708b4-118">едукатионассигнментградетипе</span><span class="sxs-lookup"><span data-stu-id="708b4-118">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="708b4-119">Значение null, если это неrubricная точка. [едукатионассигнментпоинтсградетипе](educationassignmentpointsgradetype.md) , если это точки Rubric.</span><span class="sxs-lookup"><span data-stu-id="708b4-119">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="708b4-120">левелид</span><span class="sxs-lookup"><span data-stu-id="708b4-120">levelId</span></span>|<span data-ttu-id="708b4-121">String</span><span class="sxs-lookup"><span data-stu-id="708b4-121">String</span></span>|<span data-ttu-id="708b4-122">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="708b4-122">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="708b4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="708b4-123">JSON representation</span></span>

<span data-ttu-id="708b4-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="708b4-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricLevel",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "levelId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

