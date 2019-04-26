---
title: Тип ресурса standardTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.
localization_priority: Normal
ms.openlocfilehash: 5e224865f201041b72fb943bc3a76e8a67f7975a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555894"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="194b6-103">Тип ресурса standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="194b6-103">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="194b6-104">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="194b6-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="194b6-105">Например, если для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="194b6-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="194b6-106">**dayOccurrence** — 3</span><span class="sxs-lookup"><span data-stu-id="194b6-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="194b6-107">**dayOfWeek** — "Sunday"</span><span class="sxs-lookup"><span data-stu-id="194b6-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="194b6-108">**month** — 10</span><span class="sxs-lookup"><span data-stu-id="194b6-108">**month** is 10</span></span>
- <span data-ttu-id="194b6-109">**time** — 02:00:00 _ **year** — 0, это означает, что переход с летнего на стандартное время осуществляется ежегодно в третье воскресенье октября в 02:00.</span><span class="sxs-lookup"><span data-stu-id="194b6-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="194b6-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="194b6-110">Properties</span></span>
| <span data-ttu-id="194b6-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="194b6-111">Property</span></span>     | <span data-ttu-id="194b6-112">Тип</span><span class="sxs-lookup"><span data-stu-id="194b6-112">Type</span></span>   |<span data-ttu-id="194b6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="194b6-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="194b6-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="194b6-114">dayOccurrence</span></span> | <span data-ttu-id="194b6-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="194b6-115">Edm.Int32</span></span> | <span data-ttu-id="194b6-116">Представляет n-е повторение дня недели, в который происходит переход с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="194b6-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="194b6-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="194b6-117">dayOfWeek</span></span> | <span data-ttu-id="194b6-118">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="194b6-118">dayOfWeek</span></span> | <span data-ttu-id="194b6-119">Представляет день недели, в который осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="194b6-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="194b6-120">month</span><span class="sxs-lookup"><span data-stu-id="194b6-120">month</span></span> | <span data-ttu-id="194b6-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="194b6-121">Edm.Int32</span></span> | <span data-ttu-id="194b6-122">Представляет месяц, когда осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="194b6-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="194b6-123">time</span><span class="sxs-lookup"><span data-stu-id="194b6-123">time</span></span> | <span data-ttu-id="194b6-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="194b6-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="194b6-125">Представляет время суток, когда происходит переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="194b6-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="194b6-126">year</span><span class="sxs-lookup"><span data-stu-id="194b6-126">year</span></span> | <span data-ttu-id="194b6-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="194b6-127">Edm.Int32</span></span> | <span data-ttu-id="194b6-128">Указывает периодичность перехода с летнего времени на стандартное (в годах).</span><span class="sxs-lookup"><span data-stu-id="194b6-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="194b6-129">Например, значение "0" указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="194b6-129">For example, a value of 0 means every year.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="194b6-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="194b6-130">JSON representation</span></span>

<span data-ttu-id="194b6-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="194b6-131">Here is a JSON representation of the resource.</span></span>

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
