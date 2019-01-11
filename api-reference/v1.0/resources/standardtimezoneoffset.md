---
title: Тип ресурса standardTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.
localization_priority: Normal
ms.openlocfilehash: 5e224865f201041b72fb943bc3a76e8a67f7975a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875847"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="9544a-103">Тип ресурса standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="9544a-103">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="9544a-104">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="9544a-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="9544a-105">Например, если для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="9544a-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="9544a-106">**dayOccurrence** — 3</span><span class="sxs-lookup"><span data-stu-id="9544a-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="9544a-107">**dayOfWeek** — "Sunday"</span><span class="sxs-lookup"><span data-stu-id="9544a-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="9544a-108">**month** — 10</span><span class="sxs-lookup"><span data-stu-id="9544a-108">**month** is 10</span></span>
- <span data-ttu-id="9544a-109">**time** — 02:00:00 _ **year** — 0, это означает, что переход с летнего на стандартное время осуществляется ежегодно в третье воскресенье октября в 02:00.</span><span class="sxs-lookup"><span data-stu-id="9544a-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="9544a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="9544a-110">Properties</span></span>
| <span data-ttu-id="9544a-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="9544a-111">Property</span></span>     | <span data-ttu-id="9544a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="9544a-112">Type</span></span>   |<span data-ttu-id="9544a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9544a-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9544a-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="9544a-114">dayOccurrence</span></span> | <span data-ttu-id="9544a-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="9544a-115">Edm.Int32</span></span> | <span data-ttu-id="9544a-116">Представляет n-е повторение дня недели, в который происходит переход с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="9544a-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="9544a-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="9544a-117">dayOfWeek</span></span> | <span data-ttu-id="9544a-118">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="9544a-118">dayOfWeek</span></span> | <span data-ttu-id="9544a-119">Представляет день недели, в который осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="9544a-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="9544a-120">month</span><span class="sxs-lookup"><span data-stu-id="9544a-120">month</span></span> | <span data-ttu-id="9544a-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="9544a-121">Edm.Int32</span></span> | <span data-ttu-id="9544a-122">Представляет месяц, когда осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="9544a-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="9544a-123">time</span><span class="sxs-lookup"><span data-stu-id="9544a-123">time</span></span> | <span data-ttu-id="9544a-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9544a-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="9544a-125">Представляет время суток, когда происходит переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="9544a-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="9544a-126">year</span><span class="sxs-lookup"><span data-stu-id="9544a-126">year</span></span> | <span data-ttu-id="9544a-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="9544a-127">Edm.Int32</span></span> | <span data-ttu-id="9544a-128">Указывает периодичность перехода с летнего времени на стандартное (в годах).</span><span class="sxs-lookup"><span data-stu-id="9544a-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="9544a-129">Например, значение "0" указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="9544a-129">For example, a value of 0 means every year.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9544a-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9544a-130">JSON representation</span></span>

<span data-ttu-id="9544a-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9544a-131">Here is a JSON representation of the resource.</span></span>

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
