---
title: Тип ресурса daylightTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c31225868b463b8ea3dd719d451726f59a087f99
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507291"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="fcf0b-103">Тип ресурса daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="fcf0b-103">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="fcf0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcf0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcf0b-105">Определяет, когда в часовом поясе осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-105">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="fcf0b-106">Допустим, для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="fcf0b-106">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="fcf0b-107">**bias** — 300;</span><span class="sxs-lookup"><span data-stu-id="fcf0b-107">**bias** is 300</span></span>
- <span data-ttu-id="fcf0b-108">**daylightBias** — -100;</span><span class="sxs-lookup"><span data-stu-id="fcf0b-108">**daylightBias** is -100</span></span>
- <span data-ttu-id="fcf0b-109">**dayOccurrence** — 4;</span><span class="sxs-lookup"><span data-stu-id="fcf0b-109">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="fcf0b-110">**dayOfWeek** — "sunday";</span><span class="sxs-lookup"><span data-stu-id="fcf0b-110">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="fcf0b-111">**month** — 5;</span><span class="sxs-lookup"><span data-stu-id="fcf0b-111">**month** is 5</span></span>
- <span data-ttu-id="fcf0b-112">**time** — 02:00:00; **year** — 0. Это означает, что летнее время опережает время в формате UTC на +300-100=200 минут.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-112">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="fcf0b-113">Переход с летнего на стандартное время в этом часовом поясе осуществляется ежегодно в четвертое воскресенье мая в 2:00.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-113">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="fcf0b-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcf0b-114">Properties</span></span>
| <span data-ttu-id="fcf0b-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcf0b-115">Property</span></span>     | <span data-ttu-id="fcf0b-116">Тип</span><span class="sxs-lookup"><span data-stu-id="fcf0b-116">Type</span></span>   |<span data-ttu-id="fcf0b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf0b-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fcf0b-118">daylightBias</span><span class="sxs-lookup"><span data-stu-id="fcf0b-118">daylightBias</span></span> | <span data-ttu-id="fcf0b-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fcf0b-119">Edm.Int32</span></span> | <span data-ttu-id="fcf0b-120">Смещение летнего времени относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-120">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="fcf0b-121">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-121">This value is in minutes.</span></span>  |
| <span data-ttu-id="fcf0b-122">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="fcf0b-122">dayOccurrence</span></span> | <span data-ttu-id="fcf0b-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fcf0b-123">Edm.Int32</span></span> | <span data-ttu-id="fcf0b-124">Представляет n-е повторение дня недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-124">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="fcf0b-125">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="fcf0b-125">dayOfWeek</span></span> | <span data-ttu-id="fcf0b-126">строка</span><span class="sxs-lookup"><span data-stu-id="fcf0b-126">string</span></span> | <span data-ttu-id="fcf0b-127">Представляет день недели, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-127">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="fcf0b-128">month</span><span class="sxs-lookup"><span data-stu-id="fcf0b-128">month</span></span> | <span data-ttu-id="fcf0b-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fcf0b-129">Edm.Int32</span></span> | <span data-ttu-id="fcf0b-130">Представляет месяц года, в который осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-130">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="fcf0b-131">time</span><span class="sxs-lookup"><span data-stu-id="fcf0b-131">time</span></span> | <span data-ttu-id="fcf0b-132">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fcf0b-132">Edm.TimeOfDay</span></span> | <span data-ttu-id="fcf0b-133">Представляет время суток, когда происходит переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-133">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="fcf0b-134">year</span><span class="sxs-lookup"><span data-stu-id="fcf0b-134">year</span></span> | <span data-ttu-id="fcf0b-135">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fcf0b-135">Edm.Int32</span></span> | <span data-ttu-id="fcf0b-136">Указывает, как часто (в годах) осуществляется переход со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-136">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="fcf0b-137">Например, значение 0 указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-137">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fcf0b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcf0b-138">JSON representation</span></span>

<span data-ttu-id="fcf0b-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcf0b-139">Here is a JSON representation of the resource.</span></span>

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
