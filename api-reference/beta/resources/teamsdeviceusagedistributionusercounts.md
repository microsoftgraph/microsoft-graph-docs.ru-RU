---
title: Тип ресурса teamsDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: a02dfa5a5036d67a624656d715c0fb0d3c8194ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868700"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="b0628-103">Тип ресурса teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="b0628-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b0628-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0628-104">Properties</span></span>

| <span data-ttu-id="b0628-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0628-105">Property</span></span>          | <span data-ttu-id="b0628-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b0628-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b0628-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b0628-107">reportRefreshDate</span></span> | <span data-ttu-id="b0628-108">Date</span><span class="sxs-lookup"><span data-stu-id="b0628-108">Date</span></span>   |
| <span data-ttu-id="b0628-109">web</span><span class="sxs-lookup"><span data-stu-id="b0628-109">web</span></span>               | <span data-ttu-id="b0628-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b0628-110">Int64</span></span>  |
| <span data-ttu-id="b0628-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="b0628-111">windowsPhone</span></span>      | <span data-ttu-id="b0628-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b0628-112">Int64</span></span>  |
| <span data-ttu-id="b0628-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="b0628-113">androidPhone</span></span>      | <span data-ttu-id="b0628-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b0628-114">Int64</span></span>  |
| <span data-ttu-id="b0628-115">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="b0628-115">ios</span></span>               | <span data-ttu-id="b0628-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b0628-116">Int64</span></span>  |
| <span data-ttu-id="b0628-117">mac</span><span class="sxs-lookup"><span data-stu-id="b0628-117">mac</span></span>               | <span data-ttu-id="b0628-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b0628-118">Int64</span></span>  |
| <span data-ttu-id="b0628-119">Windows</span><span class="sxs-lookup"><span data-stu-id="b0628-119">windows</span></span>           | <span data-ttu-id="b0628-120">Int64</span><span class="sxs-lookup"><span data-stu-id="b0628-120">Int64</span></span>  |
| <span data-ttu-id="b0628-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b0628-121">reportPeriod</span></span>      | <span data-ttu-id="b0628-122">String</span><span class="sxs-lookup"><span data-stu-id="b0628-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0628-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0628-123">JSON representation</span></span>

<span data-ttu-id="b0628-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0628-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportPeriod": "String"
}
```
