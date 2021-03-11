---
title: тип ресурса educationFeedback
description: Обратная связь от преподавателя к учащемуся. Это свойство представляет текстовую часть обратной связи вместе с who.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3ee5e30ddccc215fda7e08cfa4c8c9e7835f1139
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720916"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="917e5-104">тип ресурса educationFeedback</span><span class="sxs-lookup"><span data-stu-id="917e5-104">educationFeedback resource type</span></span>

<span data-ttu-id="917e5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="917e5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="917e5-106">Обратная связь от преподавателя к учащемуся.</span><span class="sxs-lookup"><span data-stu-id="917e5-106">Feedback from a teacher to a student.</span></span> <span data-ttu-id="917e5-107">Это свойство представляет текстовую часть обратной связи вместе с who.</span><span class="sxs-lookup"><span data-stu-id="917e5-107">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="917e5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="917e5-108">Properties</span></span>
| <span data-ttu-id="917e5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="917e5-109">Property</span></span>     | <span data-ttu-id="917e5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="917e5-110">Type</span></span>   |<span data-ttu-id="917e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="917e5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="917e5-112">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="917e5-112">feedbackBy</span></span>|[<span data-ttu-id="917e5-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="917e5-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="917e5-114">Пользователь, создавший отзыв.</span><span class="sxs-lookup"><span data-stu-id="917e5-114">User who created the feedback.</span></span>|
|<span data-ttu-id="917e5-115">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="917e5-115">feedbackDateTime</span></span>|<span data-ttu-id="917e5-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="917e5-116">DateTimeOffset</span></span>|<span data-ttu-id="917e5-117">Момент времени, когда была дана обратная связь.</span><span class="sxs-lookup"><span data-stu-id="917e5-117">Moment in time when the feedback was given.</span></span> <span data-ttu-id="917e5-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="917e5-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="917e5-119">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="917e5-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="917e5-120">текст</span><span class="sxs-lookup"><span data-stu-id="917e5-120">text</span></span>|[<span data-ttu-id="917e5-121">itemBody</span><span class="sxs-lookup"><span data-stu-id="917e5-121">itemBody</span></span>](itembody.md)|<span data-ttu-id="917e5-122">Обратная связь.</span><span class="sxs-lookup"><span data-stu-id="917e5-122">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="917e5-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="917e5-123">JSON representation</span></span>

<span data-ttu-id="917e5-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="917e5-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String (timestamp)",
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


