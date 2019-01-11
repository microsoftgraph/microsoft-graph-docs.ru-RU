---
title: Тип ресурса skypeForBusinessDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 3658bec2d99c5098b970e35240221dbf954beba6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884436"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="a99af-103">Тип ресурса skypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="a99af-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a99af-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a99af-104">Properties</span></span>

| <span data-ttu-id="a99af-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a99af-105">Property</span></span>          | <span data-ttu-id="a99af-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a99af-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a99af-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a99af-107">reportRefreshDate</span></span> | <span data-ttu-id="a99af-108">Date</span><span class="sxs-lookup"><span data-stu-id="a99af-108">Date</span></span>   |
| <span data-ttu-id="a99af-109">Windows</span><span class="sxs-lookup"><span data-stu-id="a99af-109">windows</span></span>           | <span data-ttu-id="a99af-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a99af-110">Int64</span></span>  |
| <span data-ttu-id="a99af-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="a99af-111">windowsPhone</span></span>      | <span data-ttu-id="a99af-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a99af-112">Int64</span></span>  |
| <span data-ttu-id="a99af-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="a99af-113">androidPhone</span></span>      | <span data-ttu-id="a99af-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a99af-114">Int64</span></span>  |
| <span data-ttu-id="a99af-115">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="a99af-115">iPhone</span></span>            | <span data-ttu-id="a99af-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a99af-116">Int64</span></span>  |
| <span data-ttu-id="a99af-117">"iPad";</span><span class="sxs-lookup"><span data-stu-id="a99af-117">iPad</span></span>              | <span data-ttu-id="a99af-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a99af-118">Int64</span></span>  |
| <span data-ttu-id="a99af-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a99af-119">reportPeriod</span></span>      | <span data-ttu-id="a99af-120">String</span><span class="sxs-lookup"><span data-stu-id="a99af-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a99af-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a99af-121">JSON representation</span></span>

<span data-ttu-id="a99af-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a99af-122">The following is a JSON representation of the resource.</span></span>

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
