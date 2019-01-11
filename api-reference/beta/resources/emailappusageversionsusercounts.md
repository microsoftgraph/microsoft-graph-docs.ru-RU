---
title: Тип ресурса emailAppUsageVersionsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 2aff22c0ae1d3042859f3457f398ef5d0a5ffbe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884849"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="a1762-103">Тип ресурса emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="a1762-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a1762-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1762-104">Properties</span></span>

| <span data-ttu-id="a1762-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1762-105">Property</span></span>          | <span data-ttu-id="a1762-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a1762-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a1762-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a1762-107">reportRefreshDate</span></span> | <span data-ttu-id="a1762-108">Date</span><span class="sxs-lookup"><span data-stu-id="a1762-108">Date</span></span>   |
| <span data-ttu-id="a1762-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="a1762-109">outlook2016</span></span>       | <span data-ttu-id="a1762-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a1762-110">Int64</span></span>  |
| <span data-ttu-id="a1762-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="a1762-111">outlook2013</span></span>       | <span data-ttu-id="a1762-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a1762-112">Int64</span></span>  |
| <span data-ttu-id="a1762-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="a1762-113">outlook2010</span></span>       | <span data-ttu-id="a1762-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a1762-114">Int64</span></span>  |
| <span data-ttu-id="a1762-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="a1762-115">outlook2007</span></span>       | <span data-ttu-id="a1762-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a1762-116">Int64</span></span>  |
| <span data-ttu-id="a1762-117">не определено</span><span class="sxs-lookup"><span data-stu-id="a1762-117">undetermined</span></span>      | <span data-ttu-id="a1762-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a1762-118">Int64</span></span>  |
| <span data-ttu-id="a1762-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a1762-119">reportPeriod</span></span>      | <span data-ttu-id="a1762-120">String</span><span class="sxs-lookup"><span data-stu-id="a1762-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1762-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1762-121">JSON representation</span></span>

<span data-ttu-id="a1762-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1762-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
