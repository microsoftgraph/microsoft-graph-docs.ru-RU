---
title: Тип ресурса yammerDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1797facecb5047badb35c0a4d876680e817cc643
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576803"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="a9612-103">Тип ресурса yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="a9612-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a9612-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9612-104">Properties</span></span>

| <span data-ttu-id="a9612-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9612-105">Property</span></span>          | <span data-ttu-id="a9612-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a9612-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a9612-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a9612-107">reportRefreshDate</span></span> | <span data-ttu-id="a9612-108">Date</span><span class="sxs-lookup"><span data-stu-id="a9612-108">Date</span></span>   |
| <span data-ttu-id="a9612-109">web</span><span class="sxs-lookup"><span data-stu-id="a9612-109">web</span></span>               | <span data-ttu-id="a9612-110">Int32</span><span class="sxs-lookup"><span data-stu-id="a9612-110">Int32</span></span>  |
| <span data-ttu-id="a9612-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="a9612-111">windowsPhone</span></span>      | <span data-ttu-id="a9612-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a9612-112">Int32</span></span>  |
| <span data-ttu-id="a9612-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="a9612-113">androidPhone</span></span>      | <span data-ttu-id="a9612-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a9612-114">Int32</span></span>  |
| <span data-ttu-id="a9612-115">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="a9612-115">iPhone</span></span>            | <span data-ttu-id="a9612-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a9612-116">Int32</span></span>  |
| <span data-ttu-id="a9612-117">"iPad";</span><span class="sxs-lookup"><span data-stu-id="a9612-117">iPad</span></span>              | <span data-ttu-id="a9612-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a9612-118">Int32</span></span>  |
| <span data-ttu-id="a9612-119">другие</span><span class="sxs-lookup"><span data-stu-id="a9612-119">other</span></span>             | <span data-ttu-id="a9612-120">Int32</span><span class="sxs-lookup"><span data-stu-id="a9612-120">Int32</span></span>  |
| <span data-ttu-id="a9612-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a9612-121">reportPeriod</span></span>      | <span data-ttu-id="a9612-122">String</span><span class="sxs-lookup"><span data-stu-id="a9612-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9612-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9612-123">JSON representation</span></span>

<span data-ttu-id="a9612-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9612-124">The following is a JSON representation of the resource.</span></span>

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
