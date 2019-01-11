---
title: Тип ресурса skypeForBusinessDeviceUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: d98590e83637e45d35f135c56f2c0b8ff7d282bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866929"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="6f883-103">Тип ресурса skypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="6f883-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6f883-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f883-104">Properties</span></span>

| <span data-ttu-id="6f883-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f883-105">Property</span></span>          | <span data-ttu-id="6f883-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6f883-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6f883-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6f883-107">reportRefreshDate</span></span> | <span data-ttu-id="6f883-108">Date</span><span class="sxs-lookup"><span data-stu-id="6f883-108">Date</span></span>   |
| <span data-ttu-id="6f883-109">Windows</span><span class="sxs-lookup"><span data-stu-id="6f883-109">windows</span></span>           | <span data-ttu-id="6f883-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6f883-110">Int64</span></span>  |
| <span data-ttu-id="6f883-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="6f883-111">windowsPhone</span></span>      | <span data-ttu-id="6f883-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6f883-112">Int64</span></span>  |
| <span data-ttu-id="6f883-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="6f883-113">androidPhone</span></span>      | <span data-ttu-id="6f883-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6f883-114">Int64</span></span>  |
| <span data-ttu-id="6f883-115">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="6f883-115">iPhone</span></span>            | <span data-ttu-id="6f883-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6f883-116">Int64</span></span>  |
| <span data-ttu-id="6f883-117">"iPad";</span><span class="sxs-lookup"><span data-stu-id="6f883-117">iPad</span></span>              | <span data-ttu-id="6f883-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6f883-118">Int64</span></span>  |
| <span data-ttu-id="6f883-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="6f883-119">reportDate</span></span>        | <span data-ttu-id="6f883-120">Date</span><span class="sxs-lookup"><span data-stu-id="6f883-120">Date</span></span>   |
| <span data-ttu-id="6f883-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6f883-121">reportPeriod</span></span>      | <span data-ttu-id="6f883-122">String</span><span class="sxs-lookup"><span data-stu-id="6f883-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f883-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f883-123">JSON representation</span></span>

<span data-ttu-id="6f883-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f883-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
