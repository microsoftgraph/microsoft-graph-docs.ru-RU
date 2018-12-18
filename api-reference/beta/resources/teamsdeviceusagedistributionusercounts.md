---
title: Тип ресурса teamsDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
ms.openlocfilehash: 01b9f67f30a7b2f13aac65cbcd4795792ee0aaa0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345852"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="1e683-103">Тип ресурса teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="1e683-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1e683-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e683-104">Properties</span></span>

| <span data-ttu-id="1e683-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e683-105">Property</span></span>          | <span data-ttu-id="1e683-106">Тип</span><span class="sxs-lookup"><span data-stu-id="1e683-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1e683-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1e683-107">reportRefreshDate</span></span> | <span data-ttu-id="1e683-108">Date</span><span class="sxs-lookup"><span data-stu-id="1e683-108">Date</span></span>   |
| <span data-ttu-id="1e683-109">web</span><span class="sxs-lookup"><span data-stu-id="1e683-109">web</span></span>               | <span data-ttu-id="1e683-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1e683-110">Int64</span></span>  |
| <span data-ttu-id="1e683-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="1e683-111">windowsPhone</span></span>      | <span data-ttu-id="1e683-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1e683-112">Int64</span></span>  |
| <span data-ttu-id="1e683-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="1e683-113">androidPhone</span></span>      | <span data-ttu-id="1e683-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1e683-114">Int64</span></span>  |
| <span data-ttu-id="1e683-115">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="1e683-115">ios</span></span>               | <span data-ttu-id="1e683-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1e683-116">Int64</span></span>  |
| <span data-ttu-id="1e683-117">mac</span><span class="sxs-lookup"><span data-stu-id="1e683-117">mac</span></span>               | <span data-ttu-id="1e683-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1e683-118">Int64</span></span>  |
| <span data-ttu-id="1e683-119">Windows</span><span class="sxs-lookup"><span data-stu-id="1e683-119">windows</span></span>           | <span data-ttu-id="1e683-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1e683-120">Int64</span></span>  |
| <span data-ttu-id="1e683-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1e683-121">reportPeriod</span></span>      | <span data-ttu-id="1e683-122">String</span><span class="sxs-lookup"><span data-stu-id="1e683-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1e683-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e683-123">JSON representation</span></span>

<span data-ttu-id="1e683-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e683-124">The following is a JSON representation of the resource.</span></span>

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
