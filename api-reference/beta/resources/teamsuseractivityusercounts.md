---
title: Тип ресурса teamsUserActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a48a80992d8370a3b6b198862a3af901737fa04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836661"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="14fa2-103">Тип ресурса teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="14fa2-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="14fa2-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="14fa2-104">Properties</span></span>

| <span data-ttu-id="14fa2-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="14fa2-105">Property</span></span>            | <span data-ttu-id="14fa2-106">Тип</span><span class="sxs-lookup"><span data-stu-id="14fa2-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="14fa2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="14fa2-107">reportRefreshDate</span></span>   | <span data-ttu-id="14fa2-108">Date</span><span class="sxs-lookup"><span data-stu-id="14fa2-108">Date</span></span>   |
| <span data-ttu-id="14fa2-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="14fa2-109">reportDate</span></span>          | <span data-ttu-id="14fa2-110">Date</span><span class="sxs-lookup"><span data-stu-id="14fa2-110">Date</span></span>   |
| <span data-ttu-id="14fa2-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="14fa2-111">teamChatMessages</span></span>    | <span data-ttu-id="14fa2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="14fa2-112">Int64</span></span>  |
| <span data-ttu-id="14fa2-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="14fa2-113">privateChatMessages</span></span> | <span data-ttu-id="14fa2-114">Int64</span><span class="sxs-lookup"><span data-stu-id="14fa2-114">Int64</span></span>  |
| <span data-ttu-id="14fa2-115">звонки</span><span class="sxs-lookup"><span data-stu-id="14fa2-115">calls</span></span>               | <span data-ttu-id="14fa2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="14fa2-116">Int64</span></span>  |
| <span data-ttu-id="14fa2-117">собрания</span><span class="sxs-lookup"><span data-stu-id="14fa2-117">meetings</span></span>            | <span data-ttu-id="14fa2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="14fa2-118">Int64</span></span>  |
| <span data-ttu-id="14fa2-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="14fa2-119">otherActions</span></span>        | <span data-ttu-id="14fa2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="14fa2-120">Int64</span></span>  |
| <span data-ttu-id="14fa2-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="14fa2-121">reportPeriod</span></span>        | <span data-ttu-id="14fa2-122">String</span><span class="sxs-lookup"><span data-stu-id="14fa2-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="14fa2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14fa2-123">JSON representation</span></span>

<span data-ttu-id="14fa2-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14fa2-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
