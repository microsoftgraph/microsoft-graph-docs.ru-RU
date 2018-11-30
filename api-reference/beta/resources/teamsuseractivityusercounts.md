---
title: Тип ресурса teamsUserActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: f6478175252e99af2bfe5561d29eebe75b638eb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075763"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="1bb49-103">Тип ресурса teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1bb49-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1bb49-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bb49-104">Properties</span></span>

| <span data-ttu-id="1bb49-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bb49-105">Property</span></span>            | <span data-ttu-id="1bb49-106">Тип</span><span class="sxs-lookup"><span data-stu-id="1bb49-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="1bb49-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1bb49-107">reportRefreshDate</span></span>   | <span data-ttu-id="1bb49-108">Date</span><span class="sxs-lookup"><span data-stu-id="1bb49-108">Date</span></span>   |
| <span data-ttu-id="1bb49-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="1bb49-109">reportDate</span></span>          | <span data-ttu-id="1bb49-110">Date</span><span class="sxs-lookup"><span data-stu-id="1bb49-110">Date</span></span>   |
| <span data-ttu-id="1bb49-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="1bb49-111">teamChatMessages</span></span>    | <span data-ttu-id="1bb49-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1bb49-112">Int64</span></span>  |
| <span data-ttu-id="1bb49-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="1bb49-113">privateChatMessages</span></span> | <span data-ttu-id="1bb49-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1bb49-114">Int64</span></span>  |
| <span data-ttu-id="1bb49-115">звонки</span><span class="sxs-lookup"><span data-stu-id="1bb49-115">calls</span></span>               | <span data-ttu-id="1bb49-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1bb49-116">Int64</span></span>  |
| <span data-ttu-id="1bb49-117">собрания</span><span class="sxs-lookup"><span data-stu-id="1bb49-117">meetings</span></span>            | <span data-ttu-id="1bb49-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1bb49-118">Int64</span></span>  |
| <span data-ttu-id="1bb49-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="1bb49-119">otherActions</span></span>        | <span data-ttu-id="1bb49-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1bb49-120">Int64</span></span>  |
| <span data-ttu-id="1bb49-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1bb49-121">reportPeriod</span></span>        | <span data-ttu-id="1bb49-122">String</span><span class="sxs-lookup"><span data-stu-id="1bb49-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1bb49-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bb49-123">JSON representation</span></span>

<span data-ttu-id="1bb49-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bb49-124">The following is a JSON representation of the resource.</span></span>

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
