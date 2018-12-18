---
title: Тип ресурса teamsUserActivityCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
ms.openlocfilehash: f67540f4172993b1076d9590438262b0d4da1846
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334519"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="79de0-103">Тип ресурса teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="79de0-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="79de0-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="79de0-104">Properties</span></span>

| <span data-ttu-id="79de0-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="79de0-105">Property</span></span>            | <span data-ttu-id="79de0-106">Тип</span><span class="sxs-lookup"><span data-stu-id="79de0-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="79de0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="79de0-107">reportRefreshDate</span></span>   | <span data-ttu-id="79de0-108">Date</span><span class="sxs-lookup"><span data-stu-id="79de0-108">Date</span></span>   |
| <span data-ttu-id="79de0-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="79de0-109">reportDate</span></span>          | <span data-ttu-id="79de0-110">Date</span><span class="sxs-lookup"><span data-stu-id="79de0-110">Date</span></span>   |
| <span data-ttu-id="79de0-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="79de0-111">teamChatMessages</span></span>    | <span data-ttu-id="79de0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="79de0-112">Int64</span></span>  |
| <span data-ttu-id="79de0-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="79de0-113">privateChatMessages</span></span> | <span data-ttu-id="79de0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="79de0-114">Int64</span></span>  |
| <span data-ttu-id="79de0-115">звонки</span><span class="sxs-lookup"><span data-stu-id="79de0-115">calls</span></span>               | <span data-ttu-id="79de0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="79de0-116">Int64</span></span>  |
| <span data-ttu-id="79de0-117">собрания</span><span class="sxs-lookup"><span data-stu-id="79de0-117">meetings</span></span>            | <span data-ttu-id="79de0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="79de0-118">Int64</span></span>  |
| <span data-ttu-id="79de0-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="79de0-119">reportPeriod</span></span>        | <span data-ttu-id="79de0-120">String</span><span class="sxs-lookup"><span data-stu-id="79de0-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="79de0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79de0-121">JSON representation</span></span>

<span data-ttu-id="79de0-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79de0-122">The following is a JSON representation of the resource.</span></span>

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
