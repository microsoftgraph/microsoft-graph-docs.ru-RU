---
title: Тип ресурса skypeForBusinessActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: e59bd33b1709780bac9726ee716ef9d81ef33c1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810131"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="56585-103">Тип ресурса skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="56585-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="56585-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="56585-104">Properties</span></span>

| <span data-ttu-id="56585-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="56585-105">Property</span></span>          | <span data-ttu-id="56585-106">Тип</span><span class="sxs-lookup"><span data-stu-id="56585-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="56585-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="56585-107">peerToPeer</span></span>        | <span data-ttu-id="56585-108">Int64</span><span class="sxs-lookup"><span data-stu-id="56585-108">Int64</span></span>  |
| <span data-ttu-id="56585-109">упорядоченные</span><span class="sxs-lookup"><span data-stu-id="56585-109">organized</span></span>         | <span data-ttu-id="56585-110">Int64</span><span class="sxs-lookup"><span data-stu-id="56585-110">Int64</span></span>  |
| <span data-ttu-id="56585-111">являлся</span><span class="sxs-lookup"><span data-stu-id="56585-111">participated</span></span>      | <span data-ttu-id="56585-112">Int64</span><span class="sxs-lookup"><span data-stu-id="56585-112">Int64</span></span>  |
| <span data-ttu-id="56585-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="56585-113">reportRefreshDate</span></span> | <span data-ttu-id="56585-114">Date</span><span class="sxs-lookup"><span data-stu-id="56585-114">Date</span></span>   |
| <span data-ttu-id="56585-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="56585-115">reportDate</span></span>        | <span data-ttu-id="56585-116">Date</span><span class="sxs-lookup"><span data-stu-id="56585-116">Date</span></span>   |
| <span data-ttu-id="56585-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="56585-117">reportPeriod</span></span>      | <span data-ttu-id="56585-118">String</span><span class="sxs-lookup"><span data-stu-id="56585-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56585-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56585-119">JSON representation</span></span>

<span data-ttu-id="56585-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56585-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
