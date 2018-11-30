---
title: Тип ресурса teamsUserActivityCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 39e90b4c9dc6b9929959139ba67ddb090d143e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081467"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="45b6e-103">Тип ресурса teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="45b6e-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="45b6e-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="45b6e-104">Properties</span></span>

| <span data-ttu-id="45b6e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="45b6e-105">Property</span></span>            | <span data-ttu-id="45b6e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="45b6e-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="45b6e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="45b6e-107">reportRefreshDate</span></span>   | <span data-ttu-id="45b6e-108">Date</span><span class="sxs-lookup"><span data-stu-id="45b6e-108">Date</span></span>   |
| <span data-ttu-id="45b6e-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="45b6e-109">reportDate</span></span>          | <span data-ttu-id="45b6e-110">Date</span><span class="sxs-lookup"><span data-stu-id="45b6e-110">Date</span></span>   |
| <span data-ttu-id="45b6e-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="45b6e-111">teamChatMessages</span></span>    | <span data-ttu-id="45b6e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="45b6e-112">Int64</span></span>  |
| <span data-ttu-id="45b6e-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="45b6e-113">privateChatMessages</span></span> | <span data-ttu-id="45b6e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="45b6e-114">Int64</span></span>  |
| <span data-ttu-id="45b6e-115">звонки</span><span class="sxs-lookup"><span data-stu-id="45b6e-115">calls</span></span>               | <span data-ttu-id="45b6e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="45b6e-116">Int64</span></span>  |
| <span data-ttu-id="45b6e-117">собрания</span><span class="sxs-lookup"><span data-stu-id="45b6e-117">meetings</span></span>            | <span data-ttu-id="45b6e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="45b6e-118">Int64</span></span>  |
| <span data-ttu-id="45b6e-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="45b6e-119">reportPeriod</span></span>        | <span data-ttu-id="45b6e-120">String</span><span class="sxs-lookup"><span data-stu-id="45b6e-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="45b6e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45b6e-121">JSON representation</span></span>

<span data-ttu-id="45b6e-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45b6e-122">The following is a JSON representation of the resource.</span></span>

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
