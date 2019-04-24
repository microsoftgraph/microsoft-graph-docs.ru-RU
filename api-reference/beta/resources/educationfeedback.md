---
title: Тип ресурса Едукатионфидбакк
description: Обратная связь преподавателя с студентом. Это свойство представляет текстовую часть обратной связи вместе с тем, кто.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 90e55b20b371d04bc3c6d45bb84fe6bf42157a2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507142"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="c2eac-104">Тип ресурса Едукатионфидбакк</span><span class="sxs-lookup"><span data-stu-id="c2eac-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2eac-105">Обратная связь преподавателя с студентом.</span><span class="sxs-lookup"><span data-stu-id="c2eac-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="c2eac-106">Это свойство представляет текстовую часть обратной связи вместе с тем, кто.</span><span class="sxs-lookup"><span data-stu-id="c2eac-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="c2eac-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2eac-107">Properties</span></span>
| <span data-ttu-id="c2eac-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2eac-108">Property</span></span>     | <span data-ttu-id="c2eac-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2eac-109">Type</span></span>   |<span data-ttu-id="c2eac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2eac-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2eac-111">Фидбаккби</span><span class="sxs-lookup"><span data-stu-id="c2eac-111">feedbackBy</span></span>|[<span data-ttu-id="c2eac-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="c2eac-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="c2eac-113">Пользователь, создавший отзыв.</span><span class="sxs-lookup"><span data-stu-id="c2eac-113">User who created the feedback.</span></span>|
|<span data-ttu-id="c2eac-114">Фидбаккдатетиме</span><span class="sxs-lookup"><span data-stu-id="c2eac-114">feedbackDateTime</span></span>|<span data-ttu-id="c2eac-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2eac-115">DateTimeOffset</span></span>|<span data-ttu-id="c2eac-116">Момент времени, когда была выдана обратная связь.</span><span class="sxs-lookup"><span data-stu-id="c2eac-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="c2eac-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c2eac-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c2eac-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c2eac-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c2eac-119">text</span><span class="sxs-lookup"><span data-stu-id="c2eac-119">text</span></span>|[<span data-ttu-id="c2eac-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="c2eac-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="c2eac-121">Замечания.</span><span class="sxs-lookup"><span data-stu-id="c2eac-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2eac-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2eac-122">JSON representation</span></span>

<span data-ttu-id="c2eac-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2eac-123">The following is a JSON representation of the resource.</span></span>

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
