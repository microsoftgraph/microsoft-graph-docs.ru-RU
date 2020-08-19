---
title: Тип ресурса daylightTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 28c1db72eec1b1556949bee3ce0c5acdc12af9e7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809847"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="5bf7a-103">Тип ресурса daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="5bf7a-103">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="5bf7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bf7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bf7a-105">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-105">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="5bf7a-106">Допустим, для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="5bf7a-106">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="5bf7a-107">**bias** — 300;</span><span class="sxs-lookup"><span data-stu-id="5bf7a-107">**bias** is 300</span></span>
- <span data-ttu-id="5bf7a-108">**daylightBias** — -100;</span><span class="sxs-lookup"><span data-stu-id="5bf7a-108">**daylightBias** is -100</span></span>
- <span data-ttu-id="5bf7a-109">**dayOccurrence** — 4;</span><span class="sxs-lookup"><span data-stu-id="5bf7a-109">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="5bf7a-110">**dayOfWeek** — "sunday";</span><span class="sxs-lookup"><span data-stu-id="5bf7a-110">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="5bf7a-111">**month** — 5;</span><span class="sxs-lookup"><span data-stu-id="5bf7a-111">**month** is 5</span></span>
- <span data-ttu-id="5bf7a-112">**time** — 02:00:00; **year** — 0. Это означает, что летнее время опережает время в формате UTC на +300-100=200 минут.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-112">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="5bf7a-113">Переход с летнего на стандартное время в этом часовом поясе осуществляется ежегодно в четвертое воскресенье мая в 2:00.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-113">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="5bf7a-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bf7a-114">Properties</span></span>
| <span data-ttu-id="5bf7a-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bf7a-115">Property</span></span>     | <span data-ttu-id="5bf7a-116">Тип</span><span class="sxs-lookup"><span data-stu-id="5bf7a-116">Type</span></span>   |<span data-ttu-id="5bf7a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5bf7a-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5bf7a-118">daylightBias</span><span class="sxs-lookup"><span data-stu-id="5bf7a-118">daylightBias</span></span> | <span data-ttu-id="5bf7a-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="5bf7a-119">Edm.Int32</span></span> | <span data-ttu-id="5bf7a-120">Смещение летнего времени относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-120">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="5bf7a-121">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-121">This value is in minutes.</span></span>  |
| <span data-ttu-id="5bf7a-122">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="5bf7a-122">dayOccurrence</span></span> | <span data-ttu-id="5bf7a-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="5bf7a-123">Edm.Int32</span></span> | <span data-ttu-id="5bf7a-124">Представляет n-е повторение дня недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-124">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="5bf7a-125">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="5bf7a-125">dayOfWeek</span></span> | <span data-ttu-id="5bf7a-126">строка</span><span class="sxs-lookup"><span data-stu-id="5bf7a-126">string</span></span> | <span data-ttu-id="5bf7a-127">Представляет день недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-127">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="5bf7a-128">month</span><span class="sxs-lookup"><span data-stu-id="5bf7a-128">month</span></span> | <span data-ttu-id="5bf7a-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="5bf7a-129">Edm.Int32</span></span> | <span data-ttu-id="5bf7a-130">Представляет месяц года, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-130">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="5bf7a-131">time</span><span class="sxs-lookup"><span data-stu-id="5bf7a-131">time</span></span> | <span data-ttu-id="5bf7a-132">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5bf7a-132">Edm.TimeOfDay</span></span> | <span data-ttu-id="5bf7a-133">Представляет время суток, когда происходит переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-133">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="5bf7a-134">year</span><span class="sxs-lookup"><span data-stu-id="5bf7a-134">year</span></span> | <span data-ttu-id="5bf7a-135">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="5bf7a-135">Edm.Int32</span></span> | <span data-ttu-id="5bf7a-136">Указывает, как часто (в годах) осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-136">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="5bf7a-137">Например, значение 0 указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-137">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5bf7a-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5bf7a-138">JSON representation</span></span>

<span data-ttu-id="5bf7a-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bf7a-139">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
