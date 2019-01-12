---
title: Тип ресурса teamsUserActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912822"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="c199a-103">Тип ресурса teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="c199a-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c199a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c199a-104">Properties</span></span>

| <span data-ttu-id="c199a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c199a-105">Property</span></span>            | <span data-ttu-id="c199a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c199a-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="c199a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c199a-107">reportRefreshDate</span></span>   | <span data-ttu-id="c199a-108">Date</span><span class="sxs-lookup"><span data-stu-id="c199a-108">Date</span></span>   |
| <span data-ttu-id="c199a-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="c199a-109">reportDate</span></span>          | <span data-ttu-id="c199a-110">Date</span><span class="sxs-lookup"><span data-stu-id="c199a-110">Date</span></span>   |
| <span data-ttu-id="c199a-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="c199a-111">teamChatMessages</span></span>    | <span data-ttu-id="c199a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c199a-112">Int64</span></span>  |
| <span data-ttu-id="c199a-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="c199a-113">privateChatMessages</span></span> | <span data-ttu-id="c199a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c199a-114">Int64</span></span>  |
| <span data-ttu-id="c199a-115">звонки</span><span class="sxs-lookup"><span data-stu-id="c199a-115">calls</span></span>               | <span data-ttu-id="c199a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c199a-116">Int64</span></span>  |
| <span data-ttu-id="c199a-117">собрания</span><span class="sxs-lookup"><span data-stu-id="c199a-117">meetings</span></span>            | <span data-ttu-id="c199a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c199a-118">Int64</span></span>  |
| <span data-ttu-id="c199a-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="c199a-119">otherActions</span></span>        | <span data-ttu-id="c199a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c199a-120">Int64</span></span>  |
| <span data-ttu-id="c199a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c199a-121">reportPeriod</span></span>        | <span data-ttu-id="c199a-122">String</span><span class="sxs-lookup"><span data-stu-id="c199a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c199a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c199a-123">JSON representation</span></span>

<span data-ttu-id="c199a-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c199a-124">The following is a JSON representation of the resource.</span></span>

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
