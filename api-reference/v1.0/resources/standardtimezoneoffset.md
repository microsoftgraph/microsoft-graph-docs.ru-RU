---
title: Тип ресурса standardTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1888bf89265ff3b62fccd0e52c10c7c7b9bdb3c5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132582"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="fe1d2-103">Тип ресурса standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="fe1d2-103">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="fe1d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe1d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe1d2-105">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fe1d2-105">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="fe1d2-106">Например, если для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="fe1d2-106">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="fe1d2-107">**dayOccurrence** — 3</span><span class="sxs-lookup"><span data-stu-id="fe1d2-107">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="fe1d2-108">**dayOfWeek** — "Sunday"</span><span class="sxs-lookup"><span data-stu-id="fe1d2-108">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="fe1d2-109">**month** — 10</span><span class="sxs-lookup"><span data-stu-id="fe1d2-109">**month** is 10</span></span>
- <span data-ttu-id="fe1d2-110">**time** — 02:00:00 _ **year** — 0, это означает, что переход с летнего на стандартное время осуществляется ежегодно в третье воскресенье октября в 02:00.</span><span class="sxs-lookup"><span data-stu-id="fe1d2-110">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="fe1d2-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe1d2-111">Properties</span></span>
| <span data-ttu-id="fe1d2-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe1d2-112">Property</span></span>     | <span data-ttu-id="fe1d2-113">Тип</span><span class="sxs-lookup"><span data-stu-id="fe1d2-113">Type</span></span>   |<span data-ttu-id="fe1d2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="fe1d2-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe1d2-115">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="fe1d2-115">dayOccurrence</span></span> | <span data-ttu-id="fe1d2-116">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fe1d2-116">Edm.Int32</span></span> | <span data-ttu-id="fe1d2-117">Представляет n-е повторение дня недели, в который происходит переход с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="fe1d2-117">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="fe1d2-118">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="fe1d2-118">dayOfWeek</span></span> | <span data-ttu-id="fe1d2-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="fe1d2-119">dayOfWeek</span></span> | <span data-ttu-id="fe1d2-120">Представляет день недели, в который осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fe1d2-120">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="fe1d2-121">month</span><span class="sxs-lookup"><span data-stu-id="fe1d2-121">month</span></span> | <span data-ttu-id="fe1d2-122">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fe1d2-122">Edm.Int32</span></span> | <span data-ttu-id="fe1d2-123">Представляет месяц, когда осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fe1d2-123">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="fe1d2-124">time</span><span class="sxs-lookup"><span data-stu-id="fe1d2-124">time</span></span> | <span data-ttu-id="fe1d2-125">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fe1d2-125">Edm.TimeOfDay</span></span> | <span data-ttu-id="fe1d2-126">Представляет время суток, когда происходит переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="fe1d2-126">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="fe1d2-127">year</span><span class="sxs-lookup"><span data-stu-id="fe1d2-127">year</span></span> | <span data-ttu-id="fe1d2-128">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fe1d2-128">Edm.Int32</span></span> | <span data-ttu-id="fe1d2-129">Указывает периодичность перехода с летнего времени на стандартное (в годах).</span><span class="sxs-lookup"><span data-stu-id="fe1d2-129">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="fe1d2-130">Например, значение "0" указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="fe1d2-130">For example, a value of 0 means every year.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe1d2-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe1d2-131">JSON representation</span></span>

<span data-ttu-id="fe1d2-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe1d2-132">Here is a JSON representation of the resource.</span></span>

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

