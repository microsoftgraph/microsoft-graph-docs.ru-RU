---
title: Тип ресурса daylightTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.
localization_priority: Normal
ms.openlocfilehash: 37e08ec0e695fd245678510ac4a40bc978b1a93e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825608"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="0c4a7-103">Тип ресурса daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="0c4a7-103">daylightTimeZoneOffset resource type</span></span>

> <span data-ttu-id="0c4a7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c4a7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c4a7-106">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-106">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="0c4a7-107">Допустим, для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="0c4a7-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="0c4a7-108">**bias** — 300;</span><span class="sxs-lookup"><span data-stu-id="0c4a7-108">**bias** is 300</span></span>
- <span data-ttu-id="0c4a7-109">**daylightBias** — -100;</span><span class="sxs-lookup"><span data-stu-id="0c4a7-109">**daylightBias** is -100</span></span>
- <span data-ttu-id="0c4a7-110">**dayOccurrence** — 4;</span><span class="sxs-lookup"><span data-stu-id="0c4a7-110">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="0c4a7-111">**dayOfWeek** — "sunday";</span><span class="sxs-lookup"><span data-stu-id="0c4a7-111">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="0c4a7-112">**month** — 5;</span><span class="sxs-lookup"><span data-stu-id="0c4a7-112">**month** is 5</span></span>
- <span data-ttu-id="0c4a7-113">**time** — 02:00:00; **year** — 0. Это означает, что летнее время опережает время в формате UTC на +300-100=200 минут.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-113">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="0c4a7-114">Переход с летнего на стандартное время в этом часовом поясе осуществляется ежегодно в четвертое воскресенье мая в 2:00.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-114">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="0c4a7-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c4a7-115">Properties</span></span>
| <span data-ttu-id="0c4a7-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c4a7-116">Property</span></span>     | <span data-ttu-id="0c4a7-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0c4a7-117">Type</span></span>   |<span data-ttu-id="0c4a7-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4a7-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c4a7-119">daylightBias</span><span class="sxs-lookup"><span data-stu-id="0c4a7-119">daylightBias</span></span> | <span data-ttu-id="0c4a7-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0c4a7-120">Edm.Int32</span></span> | <span data-ttu-id="0c4a7-121">Смещение летнего времени относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-121">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="0c4a7-122">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-122">This value is in minutes.</span></span>  |
| <span data-ttu-id="0c4a7-123">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="0c4a7-123">dayOccurrence</span></span> | <span data-ttu-id="0c4a7-124">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0c4a7-124">Edm.Int32</span></span> | <span data-ttu-id="0c4a7-125">Представляет n-е повторение дня недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-125">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="0c4a7-126">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="0c4a7-126">dayOfWeek</span></span> | <span data-ttu-id="0c4a7-127">строка</span><span class="sxs-lookup"><span data-stu-id="0c4a7-127">string</span></span> | <span data-ttu-id="0c4a7-128">Представляет день недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-128">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="0c4a7-129">month</span><span class="sxs-lookup"><span data-stu-id="0c4a7-129">month</span></span> | <span data-ttu-id="0c4a7-130">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0c4a7-130">Edm.Int32</span></span> | <span data-ttu-id="0c4a7-131">Представляет месяц года, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-131">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="0c4a7-132">time</span><span class="sxs-lookup"><span data-stu-id="0c4a7-132">time</span></span> | <span data-ttu-id="0c4a7-133">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0c4a7-133">Edm.TimeOfDay</span></span> | <span data-ttu-id="0c4a7-134">Представляет время суток, когда происходит переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-134">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="0c4a7-135">year</span><span class="sxs-lookup"><span data-stu-id="0c4a7-135">year</span></span> | <span data-ttu-id="0c4a7-136">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0c4a7-136">Edm.Int32</span></span> | <span data-ttu-id="0c4a7-137">Указывает, как часто (в годах) осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-137">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="0c4a7-138">Например, значение 0 указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-138">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0c4a7-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c4a7-139">JSON representation</span></span>

<span data-ttu-id="0c4a7-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
