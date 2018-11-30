---
title: Тип ресурса educationFeedback
description: Отзывы учитель студента. Это свойство представляет часть текста обратной связи, а также who.
ms.openlocfilehash: 4d9a08744ac818b4aadfac965a53655d498923ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074809"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="179c5-104">Тип ресурса educationFeedback</span><span class="sxs-lookup"><span data-stu-id="179c5-104">educationFeedback resource type</span></span>

> <span data-ttu-id="179c5-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="179c5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="179c5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="179c5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="179c5-107">Отзывы учитель студента.</span><span class="sxs-lookup"><span data-stu-id="179c5-107">Feedback from a teacher to a student.</span></span> <span data-ttu-id="179c5-108">Это свойство представляет часть текста обратной связи, а также who.</span><span class="sxs-lookup"><span data-stu-id="179c5-108">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="179c5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="179c5-109">Properties</span></span>
| <span data-ttu-id="179c5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="179c5-110">Property</span></span>     | <span data-ttu-id="179c5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="179c5-111">Type</span></span>   |<span data-ttu-id="179c5-112">Description</span><span class="sxs-lookup"><span data-stu-id="179c5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="179c5-113">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="179c5-113">feedbackBy</span></span>|[<span data-ttu-id="179c5-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="179c5-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="179c5-115">Пользователь, создавший свои отзывы и предложения.</span><span class="sxs-lookup"><span data-stu-id="179c5-115">User who created the feedback.</span></span>|
|<span data-ttu-id="179c5-116">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="179c5-116">feedbackDateTime</span></span>|<span data-ttu-id="179c5-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="179c5-117">DateTimeOffset</span></span>|<span data-ttu-id="179c5-118">Момент времени, когда был задан свои отзывы и предложения.</span><span class="sxs-lookup"><span data-stu-id="179c5-118">Moment in time when the feedback was given.</span></span> <span data-ttu-id="179c5-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="179c5-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="179c5-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="179c5-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="179c5-121">text</span><span class="sxs-lookup"><span data-stu-id="179c5-121">text</span></span>|[<span data-ttu-id="179c5-122">itemBody</span><span class="sxs-lookup"><span data-stu-id="179c5-122">itemBody</span></span>](itembody.md)|<span data-ttu-id="179c5-123">Обратная связь.</span><span class="sxs-lookup"><span data-stu-id="179c5-123">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="179c5-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="179c5-124">JSON representation</span></span>

<span data-ttu-id="179c5-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="179c5-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->