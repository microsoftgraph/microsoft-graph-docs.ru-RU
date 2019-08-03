---
title: Тип ресурса Едукатионрубрикауткоме
description: Едукатионауткоме, обеспечивающий высококачественный Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4640daa1bb93945463cffc9dcf54d4db23b84da1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173260"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="66d08-103">Тип ресурса Едукатионрубрикауткоме</span><span class="sxs-lookup"><span data-stu-id="66d08-103">educationRubricOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66d08-104">Объект [едукатионауткоме](educationoutcome.md) , обеспечивающий высококачественную Rubric.</span><span class="sxs-lookup"><span data-stu-id="66d08-104">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="66d08-105">Методы</span><span class="sxs-lookup"><span data-stu-id="66d08-105">Methods</span></span>

| <span data-ttu-id="66d08-106">Метод</span><span class="sxs-lookup"><span data-stu-id="66d08-106">Method</span></span>       | <span data-ttu-id="66d08-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="66d08-107">Return Type</span></span> | <span data-ttu-id="66d08-108">Описание</span><span class="sxs-lookup"><span data-stu-id="66d08-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="66d08-109">Обновление Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="66d08-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="66d08-110">Едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="66d08-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="66d08-111">Обновление объекта Едукатионауткоме.</span><span class="sxs-lookup"><span data-stu-id="66d08-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="66d08-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="66d08-112">Properties</span></span>

| <span data-ttu-id="66d08-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="66d08-113">Property</span></span>     | <span data-ttu-id="66d08-114">Тип</span><span class="sxs-lookup"><span data-stu-id="66d08-114">Type</span></span>        | <span data-ttu-id="66d08-115">Описание</span><span class="sxs-lookup"><span data-stu-id="66d08-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66d08-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="66d08-116">lastModifiedBy</span></span>|[<span data-ttu-id="66d08-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="66d08-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="66d08-118">Последний пользователь для изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="66d08-118">The last user to modify the resource.</span></span>|
|<span data-ttu-id="66d08-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66d08-119">lastModifiedDateTime</span></span>|<span data-ttu-id="66d08-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d08-120">DateTimeOffset</span></span>|<span data-ttu-id="66d08-121">Момент времени последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="66d08-121">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="66d08-122">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="66d08-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66d08-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="66d08-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="66d08-124">Публишедрубриккуалитифидбакк</span><span class="sxs-lookup"><span data-stu-id="66d08-124">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="66d08-125">Коллекция [рубриккуалитифидбаккмодел](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="66d08-125">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="66d08-126">Копия свойства Рубриккуалитифидбакк, выполняемого при отпадении оценки на учащийся.</span><span class="sxs-lookup"><span data-stu-id="66d08-126">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="66d08-127">Публишедрубриккуалитиселектедлевелс</span><span class="sxs-lookup"><span data-stu-id="66d08-127">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="66d08-128">Коллекция [рубриккуалитиселектедколумнмодел](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="66d08-128">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="66d08-129">Копия свойства Рубриккуалитиселектедлевелс, выполняемого при отпадении оценки на учащийся.</span><span class="sxs-lookup"><span data-stu-id="66d08-129">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="66d08-130">Рубриккуалитифидбакк</span><span class="sxs-lookup"><span data-stu-id="66d08-130">rubricQualityFeedback</span></span>|<span data-ttu-id="66d08-131">Коллекция [рубриккуалитифидбаккмодел](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="66d08-131">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="66d08-132">Коллекция определенных отзывов для каждого качества этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="66d08-132">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="66d08-133">Рубриккуалитиселектедлевелс</span><span class="sxs-lookup"><span data-stu-id="66d08-133">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="66d08-134">Коллекция [рубриккуалитиселектедколумнмодел](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="66d08-134">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="66d08-135">Уровень, который преподаватель выбрал для каждого качества при ступенчатом назначении.</span><span class="sxs-lookup"><span data-stu-id="66d08-135">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66d08-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="66d08-136">Relationships</span></span>

<span data-ttu-id="66d08-137">Нет</span><span class="sxs-lookup"><span data-stu-id="66d08-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66d08-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66d08-138">JSON representation</span></span>

<span data-ttu-id="66d08-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66d08-139">The following is a JSON representation of the resource.</span></span>

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