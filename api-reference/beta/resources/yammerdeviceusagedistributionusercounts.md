---
title: Тип ресурса yammerDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: f98c8831c147a82985d1e59b5559d88e1a4824c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078303"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="15b74-103">Тип ресурса yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="15b74-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="15b74-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="15b74-104">Properties</span></span>

| <span data-ttu-id="15b74-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="15b74-105">Property</span></span>          | <span data-ttu-id="15b74-106">Тип</span><span class="sxs-lookup"><span data-stu-id="15b74-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="15b74-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="15b74-107">reportRefreshDate</span></span> | <span data-ttu-id="15b74-108">Date</span><span class="sxs-lookup"><span data-stu-id="15b74-108">Date</span></span>   |
| <span data-ttu-id="15b74-109">web</span><span class="sxs-lookup"><span data-stu-id="15b74-109">web</span></span>               | <span data-ttu-id="15b74-110">Int32</span><span class="sxs-lookup"><span data-stu-id="15b74-110">Int32</span></span>  |
| <span data-ttu-id="15b74-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="15b74-111">windowsPhone</span></span>      | <span data-ttu-id="15b74-112">Int32</span><span class="sxs-lookup"><span data-stu-id="15b74-112">Int32</span></span>  |
| <span data-ttu-id="15b74-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="15b74-113">androidPhone</span></span>      | <span data-ttu-id="15b74-114">Int32</span><span class="sxs-lookup"><span data-stu-id="15b74-114">Int32</span></span>  |
| <span data-ttu-id="15b74-115">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="15b74-115">iPhone</span></span>            | <span data-ttu-id="15b74-116">Int32</span><span class="sxs-lookup"><span data-stu-id="15b74-116">Int32</span></span>  |
| <span data-ttu-id="15b74-117">"iPad";</span><span class="sxs-lookup"><span data-stu-id="15b74-117">iPad</span></span>              | <span data-ttu-id="15b74-118">Int32</span><span class="sxs-lookup"><span data-stu-id="15b74-118">Int32</span></span>  |
| <span data-ttu-id="15b74-119">другие</span><span class="sxs-lookup"><span data-stu-id="15b74-119">other</span></span>             | <span data-ttu-id="15b74-120">Int32</span><span class="sxs-lookup"><span data-stu-id="15b74-120">Int32</span></span>  |
| <span data-ttu-id="15b74-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="15b74-121">reportPeriod</span></span>      | <span data-ttu-id="15b74-122">String</span><span class="sxs-lookup"><span data-stu-id="15b74-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15b74-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15b74-123">JSON representation</span></span>

<span data-ttu-id="15b74-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15b74-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportPeriod": "String"
}
```
