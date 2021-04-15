---
title: тип ресурса teamsUserActivityCounts
description: Представляет числы действий по типу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7e931d3488fce488710c638a0155ef0c5dd3a521
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766093"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="a3d8f-103">тип ресурса teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a3d8f-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="a3d8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3d8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3d8f-105">Представляет числы действий по типу.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-105">Represents numers of activities by type.</span></span>

## <a name="properties"></a><span data-ttu-id="a3d8f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3d8f-106">Properties</span></span>

| <span data-ttu-id="a3d8f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3d8f-107">Property</span></span>            | <span data-ttu-id="a3d8f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a3d8f-108">Type</span></span>   | <span data-ttu-id="a3d8f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a3d8f-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="a3d8f-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a3d8f-110">reportRefreshDate</span></span>   | <span data-ttu-id="a3d8f-111">Дата</span><span class="sxs-lookup"><span data-stu-id="a3d8f-111">Date</span></span>   | <span data-ttu-id="a3d8f-112">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="a3d8f-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="a3d8f-113">reportDate</span></span>          | <span data-ttu-id="a3d8f-114">Дата</span><span class="sxs-lookup"><span data-stu-id="a3d8f-114">Date</span></span>   | <span data-ttu-id="a3d8f-115">Дата выполнения пользователями действий.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-115">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="a3d8f-116">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="a3d8f-116">teamChatMessages</span></span>    | <span data-ttu-id="a3d8f-117">Int64</span><span class="sxs-lookup"><span data-stu-id="a3d8f-117">Int64</span></span>  | <span data-ttu-id="a3d8f-118">Количество уникальных сообщений, которые пользователи разместили в командном чате.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-118">The number of unique messages that users posted in a team chat.</span></span> |
| <span data-ttu-id="a3d8f-119">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="a3d8f-119">privateChatMessages</span></span> | <span data-ttu-id="a3d8f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a3d8f-120">Int64</span></span>  | <span data-ttu-id="a3d8f-121">Количество уникальных сообщений, которые пользователи разместили в частном чате.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-121">The number of unique messages that users posted in a private chat.</span></span> |
| <span data-ttu-id="a3d8f-122">calls</span><span class="sxs-lookup"><span data-stu-id="a3d8f-122">calls</span></span>               | <span data-ttu-id="a3d8f-123">Int64</span><span class="sxs-lookup"><span data-stu-id="a3d8f-123">Int64</span></span>  | <span data-ttu-id="a3d8f-124">Количество уникальных вызовов 1:1, в которые участвовали пользователи.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-124">The number of unique 1:1 calls that users participated in.</span></span>   |
| <span data-ttu-id="a3d8f-125">meetings</span><span class="sxs-lookup"><span data-stu-id="a3d8f-125">meetings</span></span>            | <span data-ttu-id="a3d8f-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a3d8f-126">Int64</span></span>  | <span data-ttu-id="a3d8f-127">Количество уникальных онлайн-собраний, в которые участвовали пользователи.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-127">The number of unique online meetings that users participated in.</span></span> |
| <span data-ttu-id="a3d8f-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a3d8f-128">reportPeriod</span></span>        | <span data-ttu-id="a3d8f-129">String</span><span class="sxs-lookup"><span data-stu-id="a3d8f-129">String</span></span> | <span data-ttu-id="a3d8f-130">Количество дней, которые охватывает отчет.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-130">The number of days the report covers.</span></span>                        |


## <a name="json-representation"></a><span data-ttu-id="a3d8f-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3d8f-131">JSON representation</span></span>

<span data-ttu-id="a3d8f-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3d8f-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


