---
title: тип ресурса teamsUserActivityDistributionUserCounts
description: Представляет число пользователей по типу действия за выбранный период времени.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3d4fa8b3aec98a03d7e51819db0dc4797367f499
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766985"
---
# <a name="teamsuseractivitydistributionusercounts-resource-type"></a><span data-ttu-id="8d1ad-103">тип ресурса teamsUserActivityDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="8d1ad-103">teamsUserActivityDistributionUserCounts resource type</span></span>

<span data-ttu-id="8d1ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d1ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d1ad-105">Представляет число пользователей по типу действия за выбранный период времени.</span><span class="sxs-lookup"><span data-stu-id="8d1ad-105">Represents numbers of users by activity type over the selected time period.</span></span>

## <a name="properties"></a><span data-ttu-id="8d1ad-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d1ad-106">Properties</span></span>

| <span data-ttu-id="8d1ad-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d1ad-107">Property</span></span>            | <span data-ttu-id="8d1ad-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8d1ad-108">Type</span></span>   | <span data-ttu-id="8d1ad-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8d1ad-109">Description</span></span>                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="8d1ad-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8d1ad-110">reportRefreshDate</span></span>   | <span data-ttu-id="8d1ad-111">Дата</span><span class="sxs-lookup"><span data-stu-id="8d1ad-111">Date</span></span>   | <span data-ttu-id="8d1ad-112">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="8d1ad-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="8d1ad-113">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="8d1ad-113">teamChatMessages</span></span>    | <span data-ttu-id="8d1ad-114">Int64</span><span class="sxs-lookup"><span data-stu-id="8d1ad-114">Int64</span></span>  | <span data-ttu-id="8d1ad-115">Количество уникальных сообщений, которые пользователи разместили в командном чате.</span><span class="sxs-lookup"><span data-stu-id="8d1ad-115">The number of unique messages that users posted in a team chat.</span></span> |
| <span data-ttu-id="8d1ad-116">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="8d1ad-116">privateChatMessages</span></span> | <span data-ttu-id="8d1ad-117">Int64</span><span class="sxs-lookup"><span data-stu-id="8d1ad-117">Int64</span></span>  | <span data-ttu-id="8d1ad-118">Количество уникальных сообщений, которые пользователи разместили в частном чате.</span><span class="sxs-lookup"><span data-stu-id="8d1ad-118">The number of unique messages that users posted in a private chat.</span></span> |
| <span data-ttu-id="8d1ad-119">calls</span><span class="sxs-lookup"><span data-stu-id="8d1ad-119">calls</span></span>               | <span data-ttu-id="8d1ad-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8d1ad-120">Int64</span></span>  | <span data-ttu-id="8d1ad-121">Количество уникальных вызовов 1:1, в которые участвовали пользователи.</span><span class="sxs-lookup"><span data-stu-id="8d1ad-121">The number of unique 1:1 calls that users participated in.</span></span>   |
| <span data-ttu-id="8d1ad-122">meetings</span><span class="sxs-lookup"><span data-stu-id="8d1ad-122">meetings</span></span>            | <span data-ttu-id="8d1ad-123">Int64</span><span class="sxs-lookup"><span data-stu-id="8d1ad-123">Int64</span></span>  | <span data-ttu-id="8d1ad-124">Количество уникальных онлайн-собраний, в которые участвовали пользователи.</span><span class="sxs-lookup"><span data-stu-id="8d1ad-124">The number of unique online meetings that users participated in.</span></span> |
| <span data-ttu-id="8d1ad-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8d1ad-125">reportPeriod</span></span>        | <span data-ttu-id="8d1ad-126">String</span><span class="sxs-lookup"><span data-stu-id="8d1ad-126">String</span></span> | <span data-ttu-id="8d1ad-127">Количество дней, которые охватывает отчет.</span><span class="sxs-lookup"><span data-stu-id="8d1ad-127">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="8d1ad-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d1ad-128">JSON representation</span></span>

<span data-ttu-id="8d1ad-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d1ad-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


