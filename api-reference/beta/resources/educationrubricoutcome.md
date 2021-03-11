---
title: тип ресурса educationRubricOutcome
description: EducationOutcome, в который содержится разрисовка рубрики
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 10863f6ce1271f132ad23fb3e0c62a625e012058
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721028"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="8092a-103">тип ресурса educationRubricOutcome</span><span class="sxs-lookup"><span data-stu-id="8092a-103">educationRubricOutcome resource type</span></span>

<span data-ttu-id="8092a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8092a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8092a-105">[EducationOutcome,](educationoutcome.md) который содержит градуарную рубрику.</span><span class="sxs-lookup"><span data-stu-id="8092a-105">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="8092a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8092a-106">Methods</span></span>

| <span data-ttu-id="8092a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8092a-107">Method</span></span>       | <span data-ttu-id="8092a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8092a-108">Return Type</span></span> | <span data-ttu-id="8092a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8092a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8092a-110">Обновление educationOutcome</span><span class="sxs-lookup"><span data-stu-id="8092a-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="8092a-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="8092a-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="8092a-112">Обновление объекта educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="8092a-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8092a-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="8092a-113">Properties</span></span>

| <span data-ttu-id="8092a-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="8092a-114">Property</span></span>     | <span data-ttu-id="8092a-115">Тип</span><span class="sxs-lookup"><span data-stu-id="8092a-115">Type</span></span>        | <span data-ttu-id="8092a-116">Описание</span><span class="sxs-lookup"><span data-stu-id="8092a-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8092a-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8092a-117">lastModifiedBy</span></span>|[<span data-ttu-id="8092a-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="8092a-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="8092a-119">Последний пользователь, который изменит ресурс.</span><span class="sxs-lookup"><span data-stu-id="8092a-119">The last user to modify the resource.</span></span>|
|<span data-ttu-id="8092a-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8092a-120">lastModifiedDateTime</span></span>|<span data-ttu-id="8092a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8092a-121">DateTimeOffset</span></span>|<span data-ttu-id="8092a-122">Время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="8092a-122">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="8092a-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8092a-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8092a-124">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8092a-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8092a-125">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="8092a-125">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="8092a-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span><span class="sxs-lookup"><span data-stu-id="8092a-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="8092a-127">Копия свойства rubricQualityFeedback, которое будет сделано после выпуска класса для учащегося.</span><span class="sxs-lookup"><span data-stu-id="8092a-127">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="8092a-128">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="8092a-128">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="8092a-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span><span class="sxs-lookup"><span data-stu-id="8092a-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="8092a-130">Копия свойства rubricQualitySelectedLevels, выполненного при отсвойке класса учащемуся.</span><span class="sxs-lookup"><span data-stu-id="8092a-130">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="8092a-131">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="8092a-131">rubricQualityFeedback</span></span>|<span data-ttu-id="8092a-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span><span class="sxs-lookup"><span data-stu-id="8092a-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="8092a-133">Коллекция конкретных отзывов для каждого качества этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="8092a-133">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="8092a-134">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="8092a-134">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="8092a-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span><span class="sxs-lookup"><span data-stu-id="8092a-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="8092a-136">Уровень, выбранный преподавателем для каждого качества при классификации этого назначения.</span><span class="sxs-lookup"><span data-stu-id="8092a-136">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8092a-137">Связи</span><span class="sxs-lookup"><span data-stu-id="8092a-137">Relationships</span></span>

<span data-ttu-id="8092a-138">Нет</span><span class="sxs-lookup"><span data-stu-id="8092a-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8092a-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8092a-139">JSON representation</span></span>

<span data-ttu-id="8092a-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8092a-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "keyProperty": "id"
}-->

```json
{
  "publishedRubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "publishedRubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}],
  "rubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "rubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubricOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

