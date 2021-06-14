---
title: тип ресурса educationFeedback
description: Обратная связь от преподавателя к учащемуся.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 471c55668e7849f55d5a7623f86bc1f07fc6e537
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912624"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="3fcf6-103">тип ресурса educationFeedback</span><span class="sxs-lookup"><span data-stu-id="3fcf6-103">educationFeedback resource type</span></span>

<span data-ttu-id="3fcf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fcf6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fcf6-105">Обратная связь от преподавателя к учащемуся.</span><span class="sxs-lookup"><span data-stu-id="3fcf6-105">Feedback from a teacher to a student.</span></span> 

<span data-ttu-id="3fcf6-106">Это свойство представляет как текстовую часть отзывов, так и тех, кто предоставил обратную связь.</span><span class="sxs-lookup"><span data-stu-id="3fcf6-106">This property represents both the text part of the feedback along with who provided the feedback.</span></span>


## <a name="properties"></a><span data-ttu-id="3fcf6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fcf6-107">Properties</span></span>
| <span data-ttu-id="3fcf6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fcf6-108">Property</span></span>     | <span data-ttu-id="3fcf6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3fcf6-109">Type</span></span>   |<span data-ttu-id="3fcf6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3fcf6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fcf6-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="3fcf6-111">feedbackBy</span></span>|[<span data-ttu-id="3fcf6-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="3fcf6-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="3fcf6-113">Пользователь, создавший отзыв.</span><span class="sxs-lookup"><span data-stu-id="3fcf6-113">User who created the feedback.</span></span>|
|<span data-ttu-id="3fcf6-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="3fcf6-114">feedbackDateTime</span></span>|<span data-ttu-id="3fcf6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fcf6-115">DateTimeOffset</span></span>|<span data-ttu-id="3fcf6-116">Момент времени, когда была дана обратная связь.</span><span class="sxs-lookup"><span data-stu-id="3fcf6-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="3fcf6-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3fcf6-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3fcf6-118">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3fcf6-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="3fcf6-119">текст</span><span class="sxs-lookup"><span data-stu-id="3fcf6-119">text</span></span>|[<span data-ttu-id="3fcf6-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="3fcf6-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="3fcf6-121">Обратная связь.</span><span class="sxs-lookup"><span data-stu-id="3fcf6-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fcf6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fcf6-122">JSON representation</span></span>

<span data-ttu-id="3fcf6-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fcf6-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


