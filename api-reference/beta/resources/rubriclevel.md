---
title: Тип ресурса Рубриклевел
description: Уровень Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dd8e67cbf4ba8994e03d683665928f9e62608d8e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173337"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="cafbb-103">Тип ресурса Рубриклевел</span><span class="sxs-lookup"><span data-stu-id="cafbb-103">rubricLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cafbb-104">Уровень Rubric.</span><span class="sxs-lookup"><span data-stu-id="cafbb-104">A level of a rubric.</span></span> <span data-ttu-id="cafbb-105">Описание связи между Rubric *качеством*, *уровнями*и критериями можно узнать в разделе \*\* [едукатионрубрик](educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="cafbb-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="cafbb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cafbb-106">Properties</span></span>

| <span data-ttu-id="cafbb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cafbb-107">Property</span></span>     | <span data-ttu-id="cafbb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cafbb-108">Type</span></span>        | <span data-ttu-id="cafbb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cafbb-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cafbb-110">description</span><span class="sxs-lookup"><span data-stu-id="cafbb-110">description</span></span>|[<span data-ttu-id="cafbb-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="cafbb-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="cafbb-112">Описание этого уровня Rubric.</span><span class="sxs-lookup"><span data-stu-id="cafbb-112">The description of this rubric level.</span></span>|
|<span data-ttu-id="cafbb-113">displayName</span><span class="sxs-lookup"><span data-stu-id="cafbb-113">displayName</span></span>|<span data-ttu-id="cafbb-114">String</span><span class="sxs-lookup"><span data-stu-id="cafbb-114">String</span></span>|<span data-ttu-id="cafbb-115">Имя этого уровня Rubric.</span><span class="sxs-lookup"><span data-stu-id="cafbb-115">The name of this rubric level.</span></span>|
|<span data-ttu-id="cafbb-116">снижения</span><span class="sxs-lookup"><span data-stu-id="cafbb-116">grading</span></span>|[<span data-ttu-id="cafbb-117">Едукатионассигнментградетипе</span><span class="sxs-lookup"><span data-stu-id="cafbb-117">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="cafbb-118">Значение null, если это неrubricная точка. [едукатионассигнментпоинтсградетипе](educationassignmentpointsgradetype.md) , если это точки Rubric.</span><span class="sxs-lookup"><span data-stu-id="cafbb-118">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="cafbb-119">Левелид</span><span class="sxs-lookup"><span data-stu-id="cafbb-119">levelId</span></span>|<span data-ttu-id="cafbb-120">String</span><span class="sxs-lookup"><span data-stu-id="cafbb-120">String</span></span>|<span data-ttu-id="cafbb-121">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="cafbb-121">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cafbb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cafbb-122">JSON representation</span></span>

<span data-ttu-id="cafbb-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cafbb-123">The following is a JSON representation of the resource.</span></span>

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