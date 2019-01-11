---
title: Тип ресурса teamsUserActivityCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c7351795f6b3dafbac996844fc1ac11cd24bbc03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886592"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="833a3-103">Тип ресурса teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="833a3-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="833a3-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="833a3-104">Properties</span></span>

| <span data-ttu-id="833a3-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="833a3-105">Property</span></span>            | <span data-ttu-id="833a3-106">Тип</span><span class="sxs-lookup"><span data-stu-id="833a3-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="833a3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="833a3-107">reportRefreshDate</span></span>   | <span data-ttu-id="833a3-108">Date</span><span class="sxs-lookup"><span data-stu-id="833a3-108">Date</span></span>   |
| <span data-ttu-id="833a3-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="833a3-109">reportDate</span></span>          | <span data-ttu-id="833a3-110">Date</span><span class="sxs-lookup"><span data-stu-id="833a3-110">Date</span></span>   |
| <span data-ttu-id="833a3-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="833a3-111">teamChatMessages</span></span>    | <span data-ttu-id="833a3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="833a3-112">Int64</span></span>  |
| <span data-ttu-id="833a3-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="833a3-113">privateChatMessages</span></span> | <span data-ttu-id="833a3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="833a3-114">Int64</span></span>  |
| <span data-ttu-id="833a3-115">звонки</span><span class="sxs-lookup"><span data-stu-id="833a3-115">calls</span></span>               | <span data-ttu-id="833a3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="833a3-116">Int64</span></span>  |
| <span data-ttu-id="833a3-117">собрания</span><span class="sxs-lookup"><span data-stu-id="833a3-117">meetings</span></span>            | <span data-ttu-id="833a3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="833a3-118">Int64</span></span>  |
| <span data-ttu-id="833a3-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="833a3-119">reportPeriod</span></span>        | <span data-ttu-id="833a3-120">String</span><span class="sxs-lookup"><span data-stu-id="833a3-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="833a3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="833a3-121">JSON representation</span></span>

<span data-ttu-id="833a3-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="833a3-122">The following is a JSON representation of the resource.</span></span>

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
