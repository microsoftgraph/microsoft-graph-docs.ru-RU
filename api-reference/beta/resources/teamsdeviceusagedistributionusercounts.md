---
title: Тип ресурса teamsDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: b039320e389e1a61832089991b2368b27e51c475
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075070"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="495a6-103">Тип ресурса teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="495a6-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="495a6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="495a6-104">Properties</span></span>

| <span data-ttu-id="495a6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="495a6-105">Property</span></span>          | <span data-ttu-id="495a6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="495a6-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="495a6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="495a6-107">reportRefreshDate</span></span> | <span data-ttu-id="495a6-108">Date</span><span class="sxs-lookup"><span data-stu-id="495a6-108">Date</span></span>   |
| <span data-ttu-id="495a6-109">web</span><span class="sxs-lookup"><span data-stu-id="495a6-109">web</span></span>               | <span data-ttu-id="495a6-110">Int64</span><span class="sxs-lookup"><span data-stu-id="495a6-110">Int64</span></span>  |
| <span data-ttu-id="495a6-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="495a6-111">windowsPhone</span></span>      | <span data-ttu-id="495a6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="495a6-112">Int64</span></span>  |
| <span data-ttu-id="495a6-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="495a6-113">androidPhone</span></span>      | <span data-ttu-id="495a6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="495a6-114">Int64</span></span>  |
| <span data-ttu-id="495a6-115">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="495a6-115">ios</span></span>               | <span data-ttu-id="495a6-116">Int64</span><span class="sxs-lookup"><span data-stu-id="495a6-116">Int64</span></span>  |
| <span data-ttu-id="495a6-117">mac</span><span class="sxs-lookup"><span data-stu-id="495a6-117">mac</span></span>               | <span data-ttu-id="495a6-118">Int64</span><span class="sxs-lookup"><span data-stu-id="495a6-118">Int64</span></span>  |
| <span data-ttu-id="495a6-119">Windows</span><span class="sxs-lookup"><span data-stu-id="495a6-119">windows</span></span>           | <span data-ttu-id="495a6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="495a6-120">Int64</span></span>  |
| <span data-ttu-id="495a6-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="495a6-121">reportPeriod</span></span>      | <span data-ttu-id="495a6-122">String</span><span class="sxs-lookup"><span data-stu-id="495a6-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="495a6-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="495a6-123">JSON representation</span></span>

<span data-ttu-id="495a6-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="495a6-124">The following is a JSON representation of the resource.</span></span>

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
