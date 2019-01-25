---
title: Тип ресурса educationFeedback
description: Отзывы учитель студента. Это свойство представляет часть текста обратной связи, а также who.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 90e55b20b371d04bc3c6d45bb84fe6bf42157a2f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515638"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="57ae8-104">Тип ресурса educationFeedback</span><span class="sxs-lookup"><span data-stu-id="57ae8-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57ae8-105">Отзывы учитель студента.</span><span class="sxs-lookup"><span data-stu-id="57ae8-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="57ae8-106">Это свойство представляет часть текста обратной связи, а также who.</span><span class="sxs-lookup"><span data-stu-id="57ae8-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="57ae8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="57ae8-107">Properties</span></span>
| <span data-ttu-id="57ae8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="57ae8-108">Property</span></span>     | <span data-ttu-id="57ae8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="57ae8-109">Type</span></span>   |<span data-ttu-id="57ae8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="57ae8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57ae8-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="57ae8-111">feedbackBy</span></span>|[<span data-ttu-id="57ae8-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="57ae8-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="57ae8-113">Пользователь, создавший свои отзывы и предложения.</span><span class="sxs-lookup"><span data-stu-id="57ae8-113">User who created the feedback.</span></span>|
|<span data-ttu-id="57ae8-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="57ae8-114">feedbackDateTime</span></span>|<span data-ttu-id="57ae8-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57ae8-115">DateTimeOffset</span></span>|<span data-ttu-id="57ae8-116">Момент времени, когда был задан свои отзывы и предложения.</span><span class="sxs-lookup"><span data-stu-id="57ae8-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="57ae8-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="57ae8-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="57ae8-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="57ae8-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="57ae8-119">text</span><span class="sxs-lookup"><span data-stu-id="57ae8-119">text</span></span>|[<span data-ttu-id="57ae8-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="57ae8-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="57ae8-121">Отзывы</span><span class="sxs-lookup"><span data-stu-id="57ae8-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57ae8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57ae8-122">JSON representation</span></span>

<span data-ttu-id="57ae8-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57ae8-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfeedback.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
