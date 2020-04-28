---
title: Тип ресурса Рубриклевел
description: Уровень Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 24af9e9be6dc9b63934a02193958e0267dde8dea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521014"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="ff99b-103">Тип ресурса Рубриклевел</span><span class="sxs-lookup"><span data-stu-id="ff99b-103">rubricLevel resource type</span></span>

<span data-ttu-id="ff99b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff99b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff99b-105">Уровень Rubric.</span><span class="sxs-lookup"><span data-stu-id="ff99b-105">A level of a rubric.</span></span> <span data-ttu-id="ff99b-106">Описание связи между Rubric *качеством*, *уровнями*и *критериями*можно узнать в разделе [едукатионрубрик](educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="ff99b-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="ff99b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff99b-107">Properties</span></span>

| <span data-ttu-id="ff99b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff99b-108">Property</span></span>     | <span data-ttu-id="ff99b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ff99b-109">Type</span></span>        | <span data-ttu-id="ff99b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff99b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff99b-111">description</span><span class="sxs-lookup"><span data-stu-id="ff99b-111">description</span></span>|[<span data-ttu-id="ff99b-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="ff99b-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="ff99b-113">Описание этого уровня Rubric.</span><span class="sxs-lookup"><span data-stu-id="ff99b-113">The description of this rubric level.</span></span>|
|<span data-ttu-id="ff99b-114">displayName</span><span class="sxs-lookup"><span data-stu-id="ff99b-114">displayName</span></span>|<span data-ttu-id="ff99b-115">String</span><span class="sxs-lookup"><span data-stu-id="ff99b-115">String</span></span>|<span data-ttu-id="ff99b-116">Имя этого уровня Rubric.</span><span class="sxs-lookup"><span data-stu-id="ff99b-116">The name of this rubric level.</span></span>|
|<span data-ttu-id="ff99b-117">снижения</span><span class="sxs-lookup"><span data-stu-id="ff99b-117">grading</span></span>|[<span data-ttu-id="ff99b-118">едукатионассигнментградетипе</span><span class="sxs-lookup"><span data-stu-id="ff99b-118">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="ff99b-119">Значение null, если это неrubricная точка. [едукатионассигнментпоинтсградетипе](educationassignmentpointsgradetype.md) , если это точки Rubric.</span><span class="sxs-lookup"><span data-stu-id="ff99b-119">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="ff99b-120">левелид</span><span class="sxs-lookup"><span data-stu-id="ff99b-120">levelId</span></span>|<span data-ttu-id="ff99b-121">String</span><span class="sxs-lookup"><span data-stu-id="ff99b-121">String</span></span>|<span data-ttu-id="ff99b-122">ИДЕНТИФИКАТОР этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="ff99b-122">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff99b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff99b-123">JSON representation</span></span>

<span data-ttu-id="ff99b-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff99b-124">The following is a JSON representation of the resource.</span></span>

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