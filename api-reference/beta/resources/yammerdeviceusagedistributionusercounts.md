---
title: Тип ресурса yammerDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 937691487046e2e77cc26b2c1f1a154966e1681b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936349"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="3fbe1-103">Тип ресурса yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="3fbe1-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3fbe1-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fbe1-104">Properties</span></span>

| <span data-ttu-id="3fbe1-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fbe1-105">Property</span></span>          | <span data-ttu-id="3fbe1-106">Тип</span><span class="sxs-lookup"><span data-stu-id="3fbe1-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3fbe1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3fbe1-107">reportRefreshDate</span></span> | <span data-ttu-id="3fbe1-108">Date</span><span class="sxs-lookup"><span data-stu-id="3fbe1-108">Date</span></span>   |
| <span data-ttu-id="3fbe1-109">web</span><span class="sxs-lookup"><span data-stu-id="3fbe1-109">web</span></span>               | <span data-ttu-id="3fbe1-110">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbe1-110">Int32</span></span>  |
| <span data-ttu-id="3fbe1-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="3fbe1-111">windowsPhone</span></span>      | <span data-ttu-id="3fbe1-112">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbe1-112">Int32</span></span>  |
| <span data-ttu-id="3fbe1-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="3fbe1-113">androidPhone</span></span>      | <span data-ttu-id="3fbe1-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbe1-114">Int32</span></span>  |
| <span data-ttu-id="3fbe1-115">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="3fbe1-115">iPhone</span></span>            | <span data-ttu-id="3fbe1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbe1-116">Int32</span></span>  |
| <span data-ttu-id="3fbe1-117">"iPad";</span><span class="sxs-lookup"><span data-stu-id="3fbe1-117">iPad</span></span>              | <span data-ttu-id="3fbe1-118">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbe1-118">Int32</span></span>  |
| <span data-ttu-id="3fbe1-119">другие</span><span class="sxs-lookup"><span data-stu-id="3fbe1-119">other</span></span>             | <span data-ttu-id="3fbe1-120">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbe1-120">Int32</span></span>  |
| <span data-ttu-id="3fbe1-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3fbe1-121">reportPeriod</span></span>      | <span data-ttu-id="3fbe1-122">String</span><span class="sxs-lookup"><span data-stu-id="3fbe1-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3fbe1-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fbe1-123">JSON representation</span></span>

<span data-ttu-id="3fbe1-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fbe1-124">The following is a JSON representation of the resource.</span></span>

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
