---
title: Тип ресурса educationFeedback
description: Отзывы учитель студента. Это свойство представляет часть текста обратной связи, а также who.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0d08f3bc5c7b4882693cdcbba41b364734c6ccef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873565"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="93a22-104">Тип ресурса educationFeedback</span><span class="sxs-lookup"><span data-stu-id="93a22-104">educationFeedback resource type</span></span>

> <span data-ttu-id="93a22-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93a22-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93a22-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93a22-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93a22-107">Отзывы учитель студента.</span><span class="sxs-lookup"><span data-stu-id="93a22-107">Feedback from a teacher to a student.</span></span> <span data-ttu-id="93a22-108">Это свойство представляет часть текста обратной связи, а также who.</span><span class="sxs-lookup"><span data-stu-id="93a22-108">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="93a22-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="93a22-109">Properties</span></span>
| <span data-ttu-id="93a22-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="93a22-110">Property</span></span>     | <span data-ttu-id="93a22-111">Тип</span><span class="sxs-lookup"><span data-stu-id="93a22-111">Type</span></span>   |<span data-ttu-id="93a22-112">Описание</span><span class="sxs-lookup"><span data-stu-id="93a22-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93a22-113">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="93a22-113">feedbackBy</span></span>|[<span data-ttu-id="93a22-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="93a22-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="93a22-115">Пользователь, создавший свои отзывы и предложения.</span><span class="sxs-lookup"><span data-stu-id="93a22-115">User who created the feedback.</span></span>|
|<span data-ttu-id="93a22-116">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="93a22-116">feedbackDateTime</span></span>|<span data-ttu-id="93a22-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93a22-117">DateTimeOffset</span></span>|<span data-ttu-id="93a22-118">Момент времени, когда был задан свои отзывы и предложения.</span><span class="sxs-lookup"><span data-stu-id="93a22-118">Moment in time when the feedback was given.</span></span> <span data-ttu-id="93a22-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="93a22-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="93a22-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="93a22-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="93a22-121">text</span><span class="sxs-lookup"><span data-stu-id="93a22-121">text</span></span>|[<span data-ttu-id="93a22-122">itemBody</span><span class="sxs-lookup"><span data-stu-id="93a22-122">itemBody</span></span>](itembody.md)|<span data-ttu-id="93a22-123">Обратная связь.</span><span class="sxs-lookup"><span data-stu-id="93a22-123">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93a22-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93a22-124">JSON representation</span></span>

<span data-ttu-id="93a22-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93a22-125">The following is a JSON representation of the resource.</span></span>

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
