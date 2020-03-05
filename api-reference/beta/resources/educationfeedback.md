---
title: Тип ресурса Едукатионфидбакк
description: Обратная связь преподавателя с студентом. Это свойство представляет текстовую часть обратной связи вместе с тем, кто.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: aac921b1e9f70bc22db2b91833a6b6d348a935db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502146"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="ef7bd-104">Тип ресурса Едукатионфидбакк</span><span class="sxs-lookup"><span data-stu-id="ef7bd-104">educationFeedback resource type</span></span>

<span data-ttu-id="ef7bd-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ef7bd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef7bd-106">Обратная связь преподавателя с студентом.</span><span class="sxs-lookup"><span data-stu-id="ef7bd-106">Feedback from a teacher to a student.</span></span> <span data-ttu-id="ef7bd-107">Это свойство представляет текстовую часть обратной связи вместе с тем, кто.</span><span class="sxs-lookup"><span data-stu-id="ef7bd-107">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="ef7bd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef7bd-108">Properties</span></span>
| <span data-ttu-id="ef7bd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef7bd-109">Property</span></span>     | <span data-ttu-id="ef7bd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ef7bd-110">Type</span></span>   |<span data-ttu-id="ef7bd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ef7bd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef7bd-112">фидбаккби</span><span class="sxs-lookup"><span data-stu-id="ef7bd-112">feedbackBy</span></span>|[<span data-ttu-id="ef7bd-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="ef7bd-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="ef7bd-114">Пользователь, создавший отзыв.</span><span class="sxs-lookup"><span data-stu-id="ef7bd-114">User who created the feedback.</span></span>|
|<span data-ttu-id="ef7bd-115">фидбаккдатетиме</span><span class="sxs-lookup"><span data-stu-id="ef7bd-115">feedbackDateTime</span></span>|<span data-ttu-id="ef7bd-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef7bd-116">DateTimeOffset</span></span>|<span data-ttu-id="ef7bd-117">Момент времени, когда была выдана обратная связь.</span><span class="sxs-lookup"><span data-stu-id="ef7bd-117">Moment in time when the feedback was given.</span></span> <span data-ttu-id="ef7bd-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ef7bd-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ef7bd-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ef7bd-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ef7bd-120">текст</span><span class="sxs-lookup"><span data-stu-id="ef7bd-120">text</span></span>|[<span data-ttu-id="ef7bd-121">itemBody</span><span class="sxs-lookup"><span data-stu-id="ef7bd-121">itemBody</span></span>](itembody.md)|<span data-ttu-id="ef7bd-122">Замечания.</span><span class="sxs-lookup"><span data-stu-id="ef7bd-122">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef7bd-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef7bd-123">JSON representation</span></span>

<span data-ttu-id="ef7bd-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef7bd-124">The following is a JSON representation of the resource.</span></span>

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
