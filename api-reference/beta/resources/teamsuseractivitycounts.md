---
title: Тип ресурса teamsUserActivityCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987526"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="4c920-103">Тип ресурса teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4c920-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4c920-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c920-104">Properties</span></span>

| <span data-ttu-id="4c920-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c920-105">Property</span></span>            | <span data-ttu-id="4c920-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4c920-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="4c920-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4c920-107">reportRefreshDate</span></span>   | <span data-ttu-id="4c920-108">Date</span><span class="sxs-lookup"><span data-stu-id="4c920-108">Date</span></span>   |
| <span data-ttu-id="4c920-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="4c920-109">reportDate</span></span>          | <span data-ttu-id="4c920-110">Date</span><span class="sxs-lookup"><span data-stu-id="4c920-110">Date</span></span>   |
| <span data-ttu-id="4c920-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="4c920-111">teamChatMessages</span></span>    | <span data-ttu-id="4c920-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4c920-112">Int64</span></span>  |
| <span data-ttu-id="4c920-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="4c920-113">privateChatMessages</span></span> | <span data-ttu-id="4c920-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4c920-114">Int64</span></span>  |
| <span data-ttu-id="4c920-115">звонки</span><span class="sxs-lookup"><span data-stu-id="4c920-115">calls</span></span>               | <span data-ttu-id="4c920-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4c920-116">Int64</span></span>  |
| <span data-ttu-id="4c920-117">собрания</span><span class="sxs-lookup"><span data-stu-id="4c920-117">meetings</span></span>            | <span data-ttu-id="4c920-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4c920-118">Int64</span></span>  |
| <span data-ttu-id="4c920-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4c920-119">reportPeriod</span></span>        | <span data-ttu-id="4c920-120">String</span><span class="sxs-lookup"><span data-stu-id="4c920-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="4c920-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c920-121">JSON representation</span></span>

<span data-ttu-id="4c920-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c920-122">The following is a JSON representation of the resource.</span></span>

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
