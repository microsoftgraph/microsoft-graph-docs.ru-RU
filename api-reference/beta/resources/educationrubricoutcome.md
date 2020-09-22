---
title: Тип ресурса Едукатионрубрикауткоме
description: Едукатионауткоме, обеспечивающий высококачественный Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ade372d6bd5e669f0dcde1ac36e8ef06e473cd43
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071292"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="97487-103">Тип ресурса Едукатионрубрикауткоме</span><span class="sxs-lookup"><span data-stu-id="97487-103">educationRubricOutcome resource type</span></span>

<span data-ttu-id="97487-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97487-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97487-105">Объект [едукатионауткоме](educationoutcome.md) , обеспечивающий высококачественную Rubric.</span><span class="sxs-lookup"><span data-stu-id="97487-105">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="97487-106">Методы</span><span class="sxs-lookup"><span data-stu-id="97487-106">Methods</span></span>

| <span data-ttu-id="97487-107">Метод</span><span class="sxs-lookup"><span data-stu-id="97487-107">Method</span></span>       | <span data-ttu-id="97487-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="97487-108">Return Type</span></span> | <span data-ttu-id="97487-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97487-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="97487-110">Обновление Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="97487-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="97487-111">едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="97487-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="97487-112">Обновление объекта Едукатионауткоме.</span><span class="sxs-lookup"><span data-stu-id="97487-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="97487-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="97487-113">Properties</span></span>

| <span data-ttu-id="97487-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="97487-114">Property</span></span>     | <span data-ttu-id="97487-115">Тип</span><span class="sxs-lookup"><span data-stu-id="97487-115">Type</span></span>        | <span data-ttu-id="97487-116">Описание</span><span class="sxs-lookup"><span data-stu-id="97487-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97487-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="97487-117">lastModifiedBy</span></span>|[<span data-ttu-id="97487-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="97487-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="97487-119">Последний пользователь для изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="97487-119">The last user to modify the resource.</span></span>|
|<span data-ttu-id="97487-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97487-120">lastModifiedDateTime</span></span>|<span data-ttu-id="97487-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97487-121">DateTimeOffset</span></span>|<span data-ttu-id="97487-122">Момент времени последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="97487-122">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="97487-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="97487-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97487-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97487-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="97487-125">публишедрубриккуалитифидбакк</span><span class="sxs-lookup"><span data-stu-id="97487-125">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="97487-126">Коллекция [рубриккуалитифидбаккмодел](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="97487-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="97487-127">Копия свойства Рубриккуалитифидбакк, выполняемого при отпадении оценки на учащийся.</span><span class="sxs-lookup"><span data-stu-id="97487-127">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="97487-128">публишедрубриккуалитиселектедлевелс</span><span class="sxs-lookup"><span data-stu-id="97487-128">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="97487-129">Коллекция [рубриккуалитиселектедколумнмодел](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="97487-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="97487-130">Копия свойства Рубриккуалитиселектедлевелс, выполняемого при отпадении оценки на учащийся.</span><span class="sxs-lookup"><span data-stu-id="97487-130">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="97487-131">рубриккуалитифидбакк</span><span class="sxs-lookup"><span data-stu-id="97487-131">rubricQualityFeedback</span></span>|<span data-ttu-id="97487-132">Коллекция [рубриккуалитифидбаккмодел](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="97487-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="97487-133">Коллекция определенных отзывов для каждого качества этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="97487-133">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="97487-134">рубриккуалитиселектедлевелс</span><span class="sxs-lookup"><span data-stu-id="97487-134">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="97487-135">Коллекция [рубриккуалитиселектедколумнмодел](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="97487-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="97487-136">Уровень, который преподаватель выбрал для каждого качества при ступенчатом назначении.</span><span class="sxs-lookup"><span data-stu-id="97487-136">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97487-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="97487-137">Relationships</span></span>

<span data-ttu-id="97487-138">Нет</span><span class="sxs-lookup"><span data-stu-id="97487-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97487-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97487-139">JSON representation</span></span>

<span data-ttu-id="97487-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97487-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "baseType": "",
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

