---
title: Тип ресурса standardTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.
ms.openlocfilehash: 167ff45f4ccf1615c1560c3f2ba130cdc7747043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078158"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="c9a79-103">Тип ресурса standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="c9a79-103">standardTimeZoneOffset resource type</span></span>

> <span data-ttu-id="c9a79-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9a79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9a79-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9a79-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9a79-106">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="c9a79-106">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="c9a79-107">Например, если для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="c9a79-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="c9a79-108">**dayOccurrence** — 3</span><span class="sxs-lookup"><span data-stu-id="c9a79-108">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="c9a79-109">**dayOfWeek** — "Sunday"</span><span class="sxs-lookup"><span data-stu-id="c9a79-109">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="c9a79-110">**month** — 10</span><span class="sxs-lookup"><span data-stu-id="c9a79-110">**month** is 10</span></span>
- <span data-ttu-id="c9a79-111">**time** — 02:00:00 _ **year** — 0, это означает, что переход с летнего на стандартное время осуществляется ежегодно в третье воскресенье октября в 02:00.</span><span class="sxs-lookup"><span data-stu-id="c9a79-111">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="c9a79-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9a79-112">Properties</span></span>
| <span data-ttu-id="c9a79-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9a79-113">Property</span></span>     | <span data-ttu-id="c9a79-114">Тип</span><span class="sxs-lookup"><span data-stu-id="c9a79-114">Type</span></span>   |<span data-ttu-id="c9a79-115">Описание</span><span class="sxs-lookup"><span data-stu-id="c9a79-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c9a79-116">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="c9a79-116">dayOccurrence</span></span> | <span data-ttu-id="c9a79-117">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c9a79-117">Edm.Int32</span></span> | <span data-ttu-id="c9a79-118">Представляет n-е повторение дня недели, в который происходит переход с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="c9a79-118">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c9a79-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="c9a79-119">dayOfWeek</span></span> | <span data-ttu-id="c9a79-120">строка</span><span class="sxs-lookup"><span data-stu-id="c9a79-120">string</span></span> | <span data-ttu-id="c9a79-121">Представляет день недели, в который осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="c9a79-121">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="c9a79-122">month</span><span class="sxs-lookup"><span data-stu-id="c9a79-122">month</span></span> | <span data-ttu-id="c9a79-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c9a79-123">Edm.Int32</span></span> | <span data-ttu-id="c9a79-124">Представляет месяц, когда осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="c9a79-124">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c9a79-125">time</span><span class="sxs-lookup"><span data-stu-id="c9a79-125">time</span></span> | <span data-ttu-id="c9a79-126">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c9a79-126">Edm.TimeOfDay</span></span> | <span data-ttu-id="c9a79-127">Представляет время суток, когда происходит переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="c9a79-127">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="c9a79-128">year</span><span class="sxs-lookup"><span data-stu-id="c9a79-128">year</span></span> | <span data-ttu-id="c9a79-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="c9a79-129">Edm.Int32</span></span> | <span data-ttu-id="c9a79-130">Указывает периодичность перехода с летнего времени на стандартное (в годах).</span><span class="sxs-lookup"><span data-stu-id="c9a79-130">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="c9a79-131">Например, значение "0" указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="c9a79-131">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c9a79-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9a79-132">JSON representation</span></span>

<span data-ttu-id="c9a79-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9a79-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->