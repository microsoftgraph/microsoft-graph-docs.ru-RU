---
title: Тип ресурса teamsUserActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
ms.openlocfilehash: f4e10f1e34d4c6bdbed83279b98632c504630bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330459"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="75738-103">Тип ресурса teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="75738-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="75738-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="75738-104">Properties</span></span>

| <span data-ttu-id="75738-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="75738-105">Property</span></span>            | <span data-ttu-id="75738-106">Тип</span><span class="sxs-lookup"><span data-stu-id="75738-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="75738-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="75738-107">reportRefreshDate</span></span>   | <span data-ttu-id="75738-108">Date</span><span class="sxs-lookup"><span data-stu-id="75738-108">Date</span></span>   |
| <span data-ttu-id="75738-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="75738-109">reportDate</span></span>          | <span data-ttu-id="75738-110">Date</span><span class="sxs-lookup"><span data-stu-id="75738-110">Date</span></span>   |
| <span data-ttu-id="75738-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="75738-111">teamChatMessages</span></span>    | <span data-ttu-id="75738-112">Int64</span><span class="sxs-lookup"><span data-stu-id="75738-112">Int64</span></span>  |
| <span data-ttu-id="75738-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="75738-113">privateChatMessages</span></span> | <span data-ttu-id="75738-114">Int64</span><span class="sxs-lookup"><span data-stu-id="75738-114">Int64</span></span>  |
| <span data-ttu-id="75738-115">звонки</span><span class="sxs-lookup"><span data-stu-id="75738-115">calls</span></span>               | <span data-ttu-id="75738-116">Int64</span><span class="sxs-lookup"><span data-stu-id="75738-116">Int64</span></span>  |
| <span data-ttu-id="75738-117">собрания</span><span class="sxs-lookup"><span data-stu-id="75738-117">meetings</span></span>            | <span data-ttu-id="75738-118">Int64</span><span class="sxs-lookup"><span data-stu-id="75738-118">Int64</span></span>  |
| <span data-ttu-id="75738-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="75738-119">otherActions</span></span>        | <span data-ttu-id="75738-120">Int64</span><span class="sxs-lookup"><span data-stu-id="75738-120">Int64</span></span>  |
| <span data-ttu-id="75738-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="75738-121">reportPeriod</span></span>        | <span data-ttu-id="75738-122">String</span><span class="sxs-lookup"><span data-stu-id="75738-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75738-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75738-123">JSON representation</span></span>

<span data-ttu-id="75738-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75738-124">The following is a JSON representation of the resource.</span></span>

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
