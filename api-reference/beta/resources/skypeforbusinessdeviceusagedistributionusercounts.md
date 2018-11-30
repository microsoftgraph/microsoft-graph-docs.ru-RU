---
title: Тип ресурса skypeForBusinessDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 1534051455d805cf3bc9fabbb301ffde5be85ad9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082831"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="fe6ea-103">Тип ресурса skypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="fe6ea-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fe6ea-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe6ea-104">Properties</span></span>

| <span data-ttu-id="fe6ea-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe6ea-105">Property</span></span>          | <span data-ttu-id="fe6ea-106">Тип</span><span class="sxs-lookup"><span data-stu-id="fe6ea-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fe6ea-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fe6ea-107">reportRefreshDate</span></span> | <span data-ttu-id="fe6ea-108">Date</span><span class="sxs-lookup"><span data-stu-id="fe6ea-108">Date</span></span>   |
| <span data-ttu-id="fe6ea-109">Windows</span><span class="sxs-lookup"><span data-stu-id="fe6ea-109">windows</span></span>           | <span data-ttu-id="fe6ea-110">Int64</span><span class="sxs-lookup"><span data-stu-id="fe6ea-110">Int64</span></span>  |
| <span data-ttu-id="fe6ea-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="fe6ea-111">windowsPhone</span></span>      | <span data-ttu-id="fe6ea-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fe6ea-112">Int64</span></span>  |
| <span data-ttu-id="fe6ea-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="fe6ea-113">androidPhone</span></span>      | <span data-ttu-id="fe6ea-114">Int64</span><span class="sxs-lookup"><span data-stu-id="fe6ea-114">Int64</span></span>  |
| <span data-ttu-id="fe6ea-115">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="fe6ea-115">iPhone</span></span>            | <span data-ttu-id="fe6ea-116">Int64</span><span class="sxs-lookup"><span data-stu-id="fe6ea-116">Int64</span></span>  |
| <span data-ttu-id="fe6ea-117">"iPad";</span><span class="sxs-lookup"><span data-stu-id="fe6ea-117">iPad</span></span>              | <span data-ttu-id="fe6ea-118">Int64</span><span class="sxs-lookup"><span data-stu-id="fe6ea-118">Int64</span></span>  |
| <span data-ttu-id="fe6ea-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fe6ea-119">reportPeriod</span></span>      | <span data-ttu-id="fe6ea-120">String</span><span class="sxs-lookup"><span data-stu-id="fe6ea-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe6ea-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe6ea-121">JSON representation</span></span>

<span data-ttu-id="fe6ea-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe6ea-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportPeriod": "String"
}
```
