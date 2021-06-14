---
title: тип ресурса rubricLevel
description: Уровень рубрики.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b4cbd952d8c5bed366d6cfbbda5920d7eddba97d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911525"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="8acab-103">тип ресурса rubricLevel</span><span class="sxs-lookup"><span data-stu-id="8acab-103">rubricLevel resource type</span></span>

<span data-ttu-id="8acab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8acab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8acab-105">Уровень рубрики.</span><span class="sxs-lookup"><span data-stu-id="8acab-105">A level of a rubric.</span></span> 

<span data-ttu-id="8acab-106">См. [в рубрике EducationRubric](educationrubric.md) описание взаимосвязи между качествами,  *уровнями* и критериями *рубрики.*</span><span class="sxs-lookup"><span data-stu-id="8acab-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="8acab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8acab-107">Properties</span></span>

| <span data-ttu-id="8acab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8acab-108">Property</span></span>     | <span data-ttu-id="8acab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8acab-109">Type</span></span>        | <span data-ttu-id="8acab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8acab-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8acab-111">description</span><span class="sxs-lookup"><span data-stu-id="8acab-111">description</span></span>|[<span data-ttu-id="8acab-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="8acab-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="8acab-113">Описание этого уровня рубрики.</span><span class="sxs-lookup"><span data-stu-id="8acab-113">The description of this rubric level.</span></span>|
|<span data-ttu-id="8acab-114">displayName</span><span class="sxs-lookup"><span data-stu-id="8acab-114">displayName</span></span>|<span data-ttu-id="8acab-115">String</span><span class="sxs-lookup"><span data-stu-id="8acab-115">String</span></span>|<span data-ttu-id="8acab-116">Имя этого уровня рубрики.</span><span class="sxs-lookup"><span data-stu-id="8acab-116">The name of this rubric level.</span></span>|
|<span data-ttu-id="8acab-117">классификация</span><span class="sxs-lookup"><span data-stu-id="8acab-117">grading</span></span>|[<span data-ttu-id="8acab-118">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="8acab-118">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="8acab-119">Null, если это не пункты рубрики; [educationAssignmentPointsGradeType,](educationassignmentpointsgradetype.md) если это точки рубрики.</span><span class="sxs-lookup"><span data-stu-id="8acab-119">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="8acab-120">levelId</span><span class="sxs-lookup"><span data-stu-id="8acab-120">levelId</span></span>|<span data-ttu-id="8acab-121">String</span><span class="sxs-lookup"><span data-stu-id="8acab-121">String</span></span>|<span data-ttu-id="8acab-122">ID этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="8acab-122">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8acab-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8acab-123">JSON representation</span></span>

<span data-ttu-id="8acab-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8acab-124">The following is a JSON representation of the resource.</span></span>

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

