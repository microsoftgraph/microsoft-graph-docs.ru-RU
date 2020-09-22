---
title: Тип ресурса Едукатионфидбакк
description: Обратная связь преподавателя с студентом. Это свойство представляет текстовую часть обратной связи вместе с тем, кто.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00514ce99860fa52d167465fb223dad2981c28db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095487"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="fb56d-104">Тип ресурса Едукатионфидбакк</span><span class="sxs-lookup"><span data-stu-id="fb56d-104">educationFeedback resource type</span></span>

<span data-ttu-id="fb56d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb56d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb56d-106">Обратная связь преподавателя с студентом.</span><span class="sxs-lookup"><span data-stu-id="fb56d-106">Feedback from a teacher to a student.</span></span> <span data-ttu-id="fb56d-107">Это свойство представляет текстовую часть обратной связи вместе с тем, кто.</span><span class="sxs-lookup"><span data-stu-id="fb56d-107">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="fb56d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb56d-108">Properties</span></span>
| <span data-ttu-id="fb56d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb56d-109">Property</span></span>     | <span data-ttu-id="fb56d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fb56d-110">Type</span></span>   |<span data-ttu-id="fb56d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fb56d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb56d-112">фидбаккби</span><span class="sxs-lookup"><span data-stu-id="fb56d-112">feedbackBy</span></span>|[<span data-ttu-id="fb56d-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="fb56d-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="fb56d-114">Пользователь, создавший отзыв.</span><span class="sxs-lookup"><span data-stu-id="fb56d-114">User who created the feedback.</span></span>|
|<span data-ttu-id="fb56d-115">фидбаккдатетиме</span><span class="sxs-lookup"><span data-stu-id="fb56d-115">feedbackDateTime</span></span>|<span data-ttu-id="fb56d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb56d-116">DateTimeOffset</span></span>|<span data-ttu-id="fb56d-117">Момент времени, когда была выдана обратная связь.</span><span class="sxs-lookup"><span data-stu-id="fb56d-117">Moment in time when the feedback was given.</span></span> <span data-ttu-id="fb56d-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fb56d-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fb56d-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fb56d-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fb56d-120">текст</span><span class="sxs-lookup"><span data-stu-id="fb56d-120">text</span></span>|[<span data-ttu-id="fb56d-121">itemBody</span><span class="sxs-lookup"><span data-stu-id="fb56d-121">itemBody</span></span>](itembody.md)|<span data-ttu-id="fb56d-122">Замечания.</span><span class="sxs-lookup"><span data-stu-id="fb56d-122">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb56d-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fb56d-123">JSON representation</span></span>

<span data-ttu-id="fb56d-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb56d-124">The following is a JSON representation of the resource.</span></span>

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


