---
title: Тип ресурса standardTimeZoneOffset
description: Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 695fd6dbe04ce35cff061f11f8c9783c78830d61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034015"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="6f136-103">Тип ресурса standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="6f136-103">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="6f136-104">Определяет, когда в часовом поясе осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="6f136-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="6f136-105">Например, если для указанного часового пояса заданы следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="6f136-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="6f136-106">**dayOccurrence** — 3</span><span class="sxs-lookup"><span data-stu-id="6f136-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="6f136-107">**dayOfWeek** — "Sunday"</span><span class="sxs-lookup"><span data-stu-id="6f136-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="6f136-108">**month** — 10</span><span class="sxs-lookup"><span data-stu-id="6f136-108">**month** is 10</span></span>
- <span data-ttu-id="6f136-109">**time** — 02:00:00 _ **year** — 0, это означает, что переход с летнего на стандартное время осуществляется ежегодно в третье воскресенье октября в 02:00.</span><span class="sxs-lookup"><span data-stu-id="6f136-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="6f136-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f136-110">Properties</span></span>
| <span data-ttu-id="6f136-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f136-111">Property</span></span>     | <span data-ttu-id="6f136-112">Тип</span><span class="sxs-lookup"><span data-stu-id="6f136-112">Type</span></span>   |<span data-ttu-id="6f136-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6f136-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f136-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="6f136-114">dayOccurrence</span></span> | <span data-ttu-id="6f136-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6f136-115">Edm.Int32</span></span> | <span data-ttu-id="6f136-116">Представляет n-е повторение дня недели, в который происходит переход с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="6f136-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="6f136-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="6f136-117">dayOfWeek</span></span> | <span data-ttu-id="6f136-118">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="6f136-118">dayOfWeek</span></span> | <span data-ttu-id="6f136-119">Представляет день недели, в который осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="6f136-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="6f136-120">month</span><span class="sxs-lookup"><span data-stu-id="6f136-120">month</span></span> | <span data-ttu-id="6f136-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6f136-121">Edm.Int32</span></span> | <span data-ttu-id="6f136-122">Представляет месяц, когда осуществляется переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="6f136-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="6f136-123">time</span><span class="sxs-lookup"><span data-stu-id="6f136-123">time</span></span> | <span data-ttu-id="6f136-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6f136-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="6f136-125">Представляет время суток, когда происходит переход с летнего времени на стандартное.</span><span class="sxs-lookup"><span data-stu-id="6f136-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="6f136-126">year</span><span class="sxs-lookup"><span data-stu-id="6f136-126">year</span></span> | <span data-ttu-id="6f136-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6f136-127">Edm.Int32</span></span> | <span data-ttu-id="6f136-128">Указывает периодичность перехода с летнего времени на стандартное (в годах).</span><span class="sxs-lookup"><span data-stu-id="6f136-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="6f136-129">Например, значение "0" указывает, что переход осуществляется ежегодно.</span><span class="sxs-lookup"><span data-stu-id="6f136-129">For example, a value of 0 means every year.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f136-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f136-130">JSON representation</span></span>

<span data-ttu-id="6f136-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f136-131">Here is a JSON representation of the resource.</span></span>

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
