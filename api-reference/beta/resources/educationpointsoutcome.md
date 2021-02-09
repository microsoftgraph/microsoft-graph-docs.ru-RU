---
title: Тип ресурса educationPointsOutcome
description: EducationOutcome, который дает числовую оценку
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ebf9a0bf12b7c4a78f28c9d75c93469afec2c34c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153632"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="16c86-103">Тип ресурса educationPointsOutcome</span><span class="sxs-lookup"><span data-stu-id="16c86-103">educationPointsOutcome resource type</span></span>

<span data-ttu-id="16c86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16c86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16c86-105">[EducationOutcome,](educationoutcome.md) который дает числовую оценку.</span><span class="sxs-lookup"><span data-stu-id="16c86-105">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="16c86-106">Методы</span><span class="sxs-lookup"><span data-stu-id="16c86-106">Methods</span></span>

| <span data-ttu-id="16c86-107">Метод</span><span class="sxs-lookup"><span data-stu-id="16c86-107">Method</span></span>       | <span data-ttu-id="16c86-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="16c86-108">Return Type</span></span> | <span data-ttu-id="16c86-109">Описание</span><span class="sxs-lookup"><span data-stu-id="16c86-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="16c86-110">Обновление educationOutcome</span><span class="sxs-lookup"><span data-stu-id="16c86-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="16c86-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="16c86-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="16c86-112">Обновление объекта educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="16c86-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="16c86-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="16c86-113">Properties</span></span>

| <span data-ttu-id="16c86-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="16c86-114">Property</span></span>     | <span data-ttu-id="16c86-115">Тип</span><span class="sxs-lookup"><span data-stu-id="16c86-115">Type</span></span>        | <span data-ttu-id="16c86-116">Описание</span><span class="sxs-lookup"><span data-stu-id="16c86-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16c86-117">points</span><span class="sxs-lookup"><span data-stu-id="16c86-117">points</span></span>|[<span data-ttu-id="16c86-118">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="16c86-118">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="16c86-119">Числовая оценка, присвоенная преподавателем для этого задания.</span><span class="sxs-lookup"><span data-stu-id="16c86-119">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="16c86-120">publishedPoints</span><span class="sxs-lookup"><span data-stu-id="16c86-120">publishedPoints</span></span>|[<span data-ttu-id="16c86-121">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="16c86-121">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="16c86-122">Копия свойства points, которая сделана при отписке оценки учащемуся.</span><span class="sxs-lookup"><span data-stu-id="16c86-122">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16c86-123">Связи</span><span class="sxs-lookup"><span data-stu-id="16c86-123">Relationships</span></span>

<span data-ttu-id="16c86-124">Нет</span><span class="sxs-lookup"><span data-stu-id="16c86-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16c86-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16c86-125">JSON representation</span></span>

<span data-ttu-id="16c86-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16c86-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "keyProperty": "id"
}-->

```json
{
  "points": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"},
  "publishedPoints": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPointsOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

