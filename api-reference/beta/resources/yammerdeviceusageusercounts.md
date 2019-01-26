---
title: Тип ресурса yammerDeviceUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 63bd3e150e822d3c356f4409c2920e4998e53ec2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577328"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="7340d-103">Тип ресурса yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="7340d-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7340d-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7340d-104">Properties</span></span>

| <span data-ttu-id="7340d-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7340d-105">Property</span></span>          | <span data-ttu-id="7340d-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7340d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7340d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7340d-107">reportRefreshDate</span></span> | <span data-ttu-id="7340d-108">Date</span><span class="sxs-lookup"><span data-stu-id="7340d-108">Date</span></span>   |
| <span data-ttu-id="7340d-109">web</span><span class="sxs-lookup"><span data-stu-id="7340d-109">web</span></span>               | <span data-ttu-id="7340d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="7340d-110">Int32</span></span>  |
| <span data-ttu-id="7340d-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="7340d-111">windowsPhone</span></span>      | <span data-ttu-id="7340d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="7340d-112">Int32</span></span>  |
| <span data-ttu-id="7340d-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="7340d-113">androidPhone</span></span>      | <span data-ttu-id="7340d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7340d-114">Int32</span></span>  |
| <span data-ttu-id="7340d-115">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="7340d-115">iPhone</span></span>            | <span data-ttu-id="7340d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="7340d-116">Int32</span></span>  |
| <span data-ttu-id="7340d-117">"iPad";</span><span class="sxs-lookup"><span data-stu-id="7340d-117">iPad</span></span>              | <span data-ttu-id="7340d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="7340d-118">Int32</span></span>  |
| <span data-ttu-id="7340d-119">другие</span><span class="sxs-lookup"><span data-stu-id="7340d-119">other</span></span>             | <span data-ttu-id="7340d-120">Int32</span><span class="sxs-lookup"><span data-stu-id="7340d-120">Int32</span></span>  |
| <span data-ttu-id="7340d-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="7340d-121">reportDate</span></span>        | <span data-ttu-id="7340d-122">Date</span><span class="sxs-lookup"><span data-stu-id="7340d-122">Date</span></span>   |
| <span data-ttu-id="7340d-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7340d-123">reportPeriod</span></span>      | <span data-ttu-id="7340d-124">String</span><span class="sxs-lookup"><span data-stu-id="7340d-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7340d-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7340d-125">JSON representation</span></span>

<span data-ttu-id="7340d-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7340d-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
