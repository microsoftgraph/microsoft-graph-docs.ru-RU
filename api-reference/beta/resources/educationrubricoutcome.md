---
title: Тип ресурса educationRubricOutcome
description: EducationOutcome, который предоставляет оградимую рубрику
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c8132159fa70c175a46a43a13ebce981299f2431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161917"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="b907f-103">Тип ресурса educationRubricOutcome</span><span class="sxs-lookup"><span data-stu-id="b907f-103">educationRubricOutcome resource type</span></span>

<span data-ttu-id="b907f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b907f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b907f-105">[EducationOutcome,](educationoutcome.md) который предоставляет оградимую рубрику.</span><span class="sxs-lookup"><span data-stu-id="b907f-105">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="b907f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b907f-106">Methods</span></span>

| <span data-ttu-id="b907f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b907f-107">Method</span></span>       | <span data-ttu-id="b907f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b907f-108">Return Type</span></span> | <span data-ttu-id="b907f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b907f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b907f-110">Обновление educationOutcome</span><span class="sxs-lookup"><span data-stu-id="b907f-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="b907f-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="b907f-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="b907f-112">Обновление объекта educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="b907f-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b907f-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="b907f-113">Properties</span></span>

| <span data-ttu-id="b907f-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="b907f-114">Property</span></span>     | <span data-ttu-id="b907f-115">Тип</span><span class="sxs-lookup"><span data-stu-id="b907f-115">Type</span></span>        | <span data-ttu-id="b907f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b907f-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b907f-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b907f-117">lastModifiedBy</span></span>|[<span data-ttu-id="b907f-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="b907f-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="b907f-119">Последний пользователь, который изменял ресурс.</span><span class="sxs-lookup"><span data-stu-id="b907f-119">The last user to modify the resource.</span></span>|
|<span data-ttu-id="b907f-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b907f-120">lastModifiedDateTime</span></span>|<span data-ttu-id="b907f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b907f-121">DateTimeOffset</span></span>|<span data-ttu-id="b907f-122">Время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="b907f-122">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="b907f-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b907f-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b907f-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b907f-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b907f-125">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="b907f-125">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="b907f-126">[Коллекция rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="b907f-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="b907f-127">Копия свойства rubricQualityFeedback, которая происходит, когда учащемуся отпущен класс.</span><span class="sxs-lookup"><span data-stu-id="b907f-127">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="b907f-128">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="b907f-128">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="b907f-129">[Коллекция rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="b907f-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="b907f-130">Копия свойства rubricQualitySelectedLevels, которая сделана, когда учащемуся был освобожден класс.</span><span class="sxs-lookup"><span data-stu-id="b907f-130">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="b907f-131">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="b907f-131">rubricQualityFeedback</span></span>|<span data-ttu-id="b907f-132">[Коллекция rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="b907f-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="b907f-133">Коллекция определенных отзывов для каждого качества этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="b907f-133">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="b907f-134">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="b907f-134">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="b907f-135">[Коллекция rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="b907f-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="b907f-136">Уровень, выбранный преподавателем для каждого качества при классификации этого задания.</span><span class="sxs-lookup"><span data-stu-id="b907f-136">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b907f-137">Связи</span><span class="sxs-lookup"><span data-stu-id="b907f-137">Relationships</span></span>

<span data-ttu-id="b907f-138">Нет</span><span class="sxs-lookup"><span data-stu-id="b907f-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b907f-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b907f-139">JSON representation</span></span>

<span data-ttu-id="b907f-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b907f-140">The following is a JSON representation of the resource.</span></span>

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

