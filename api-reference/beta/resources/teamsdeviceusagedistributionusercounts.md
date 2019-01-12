---
title: Тип ресурса teamsDeviceUsageDistributionUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d398782cef79cdf92bc56502f7c6cbf1bcdee99d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979287"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="ba160-103">Тип ресурса teamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ba160-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ba160-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba160-104">Properties</span></span>

| <span data-ttu-id="ba160-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba160-105">Property</span></span>          | <span data-ttu-id="ba160-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ba160-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ba160-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ba160-107">reportRefreshDate</span></span> | <span data-ttu-id="ba160-108">Date</span><span class="sxs-lookup"><span data-stu-id="ba160-108">Date</span></span>   |
| <span data-ttu-id="ba160-109">web</span><span class="sxs-lookup"><span data-stu-id="ba160-109">web</span></span>               | <span data-ttu-id="ba160-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ba160-110">Int64</span></span>  |
| <span data-ttu-id="ba160-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="ba160-111">windowsPhone</span></span>      | <span data-ttu-id="ba160-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ba160-112">Int64</span></span>  |
| <span data-ttu-id="ba160-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="ba160-113">androidPhone</span></span>      | <span data-ttu-id="ba160-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ba160-114">Int64</span></span>  |
| <span data-ttu-id="ba160-115">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="ba160-115">ios</span></span>               | <span data-ttu-id="ba160-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ba160-116">Int64</span></span>  |
| <span data-ttu-id="ba160-117">mac</span><span class="sxs-lookup"><span data-stu-id="ba160-117">mac</span></span>               | <span data-ttu-id="ba160-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ba160-118">Int64</span></span>  |
| <span data-ttu-id="ba160-119">Windows</span><span class="sxs-lookup"><span data-stu-id="ba160-119">windows</span></span>           | <span data-ttu-id="ba160-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ba160-120">Int64</span></span>  |
| <span data-ttu-id="ba160-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ba160-121">reportPeriod</span></span>      | <span data-ttu-id="ba160-122">String</span><span class="sxs-lookup"><span data-stu-id="ba160-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba160-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba160-123">JSON representation</span></span>

<span data-ttu-id="ba160-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba160-124">The following is a JSON representation of the resource.</span></span>

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
