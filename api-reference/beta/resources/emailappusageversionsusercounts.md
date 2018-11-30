---
title: Тип ресурса emailAppUsageVersionsUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 7b4a59a1e15ddf41f0e4204efc4d3e0c6549e587
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080207"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="fe7dd-103">Тип ресурса emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="fe7dd-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fe7dd-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe7dd-104">Properties</span></span>

| <span data-ttu-id="fe7dd-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe7dd-105">Property</span></span>          | <span data-ttu-id="fe7dd-106">Тип</span><span class="sxs-lookup"><span data-stu-id="fe7dd-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fe7dd-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fe7dd-107">reportRefreshDate</span></span> | <span data-ttu-id="fe7dd-108">Date</span><span class="sxs-lookup"><span data-stu-id="fe7dd-108">Date</span></span>   |
| <span data-ttu-id="fe7dd-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="fe7dd-109">outlook2016</span></span>       | <span data-ttu-id="fe7dd-110">Int64</span><span class="sxs-lookup"><span data-stu-id="fe7dd-110">Int64</span></span>  |
| <span data-ttu-id="fe7dd-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="fe7dd-111">outlook2013</span></span>       | <span data-ttu-id="fe7dd-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fe7dd-112">Int64</span></span>  |
| <span data-ttu-id="fe7dd-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="fe7dd-113">outlook2010</span></span>       | <span data-ttu-id="fe7dd-114">Int64</span><span class="sxs-lookup"><span data-stu-id="fe7dd-114">Int64</span></span>  |
| <span data-ttu-id="fe7dd-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="fe7dd-115">outlook2007</span></span>       | <span data-ttu-id="fe7dd-116">Int64</span><span class="sxs-lookup"><span data-stu-id="fe7dd-116">Int64</span></span>  |
| <span data-ttu-id="fe7dd-117">не определено</span><span class="sxs-lookup"><span data-stu-id="fe7dd-117">undetermined</span></span>      | <span data-ttu-id="fe7dd-118">Int64</span><span class="sxs-lookup"><span data-stu-id="fe7dd-118">Int64</span></span>  |
| <span data-ttu-id="fe7dd-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fe7dd-119">reportPeriod</span></span>      | <span data-ttu-id="fe7dd-120">String</span><span class="sxs-lookup"><span data-stu-id="fe7dd-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe7dd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe7dd-121">JSON representation</span></span>

<span data-ttu-id="fe7dd-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe7dd-122">The following is a JSON representation of the resource.</span></span>

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
