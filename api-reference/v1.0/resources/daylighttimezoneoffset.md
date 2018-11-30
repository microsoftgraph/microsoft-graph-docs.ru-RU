---
title: Тип ресурса daylightTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.
ms.openlocfilehash: bab5be49e88de1c71c7d13f53c15158e4a253a6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024392"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="093ae-103">Тип ресурса daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="093ae-103">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="093ae-104">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="093ae-104">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="093ae-105">Допустим, для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="093ae-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="093ae-106">**bias** — 300;</span><span class="sxs-lookup"><span data-stu-id="093ae-106">**bias** is 300</span></span>
- <span data-ttu-id="093ae-107">**daylightBias** — -100;</span><span class="sxs-lookup"><span data-stu-id="093ae-107">**daylightBias** is -100</span></span>
- <span data-ttu-id="093ae-108">**dayOccurrence** — 4;</span><span class="sxs-lookup"><span data-stu-id="093ae-108">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="093ae-109">**dayOfWeek** — "sunday";</span><span class="sxs-lookup"><span data-stu-id="093ae-109">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="093ae-110">**month** — 5;</span><span class="sxs-lookup"><span data-stu-id="093ae-110">**month** is 5</span></span>
- <span data-ttu-id="093ae-111">**time** — 02:00:00; **year** — 0. Это означает, что летнее время опережает время в формате UTC на +300-100=200 минут.</span><span class="sxs-lookup"><span data-stu-id="093ae-111">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="093ae-112">Переход с летнего на стандартное время в этом часовом поясе осуществляется ежегодно в четвертое воскресенье мая в 2:00.</span><span class="sxs-lookup"><span data-stu-id="093ae-112">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="093ae-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="093ae-113">Properties</span></span>
| <span data-ttu-id="093ae-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="093ae-114">Property</span></span>     | <span data-ttu-id="093ae-115">Тип</span><span class="sxs-lookup"><span data-stu-id="093ae-115">Type</span></span>   |<span data-ttu-id="093ae-116">Описание</span><span class="sxs-lookup"><span data-stu-id="093ae-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="093ae-117">daylightBias</span><span class="sxs-lookup"><span data-stu-id="093ae-117">daylightBias</span></span> | <span data-ttu-id="093ae-118">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="093ae-118">Edm.Int32</span></span> | <span data-ttu-id="093ae-119">Смещение летнего времени относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="093ae-119">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="093ae-120">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="093ae-120">This value is in minutes.</span></span>  |
| <span data-ttu-id="093ae-121">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="093ae-121">dayOccurrence</span></span> | <span data-ttu-id="093ae-122">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="093ae-122">Edm.Int32</span></span> | <span data-ttu-id="093ae-123">Представляет n-е повторение дня недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="093ae-123">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="093ae-124">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="093ae-124">dayOfWeek</span></span> | <span data-ttu-id="093ae-125">строка</span><span class="sxs-lookup"><span data-stu-id="093ae-125">string</span></span> | <span data-ttu-id="093ae-126">Представляет день недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="093ae-126">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="093ae-127">month</span><span class="sxs-lookup"><span data-stu-id="093ae-127">month</span></span> | <span data-ttu-id="093ae-128">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="093ae-128">Edm.Int32</span></span> | <span data-ttu-id="093ae-129">Представляет месяц года, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="093ae-129">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="093ae-130">time</span><span class="sxs-lookup"><span data-stu-id="093ae-130">time</span></span> | <span data-ttu-id="093ae-131">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="093ae-131">Edm.TimeOfDay</span></span> | <span data-ttu-id="093ae-132">Представляет время суток, когда происходит переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="093ae-132">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="093ae-133">year</span><span class="sxs-lookup"><span data-stu-id="093ae-133">year</span></span> | <span data-ttu-id="093ae-134">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="093ae-134">Edm.Int32</span></span> | <span data-ttu-id="093ae-135">Указывает, как часто (в годах) осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="093ae-135">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="093ae-136">Например, значение 0 указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="093ae-136">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="093ae-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="093ae-137">JSON representation</span></span>

<span data-ttu-id="093ae-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="093ae-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.standardTimeZoneOffset",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
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
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->