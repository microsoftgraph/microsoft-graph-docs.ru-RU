---
title: Тип ресурса teamsDeviceUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 671dfada02b9c16d3392d0a97023b82020fd1218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987400"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="ad5bf-103">Тип ресурса teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ad5bf-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ad5bf-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad5bf-104">Properties</span></span>

| <span data-ttu-id="ad5bf-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad5bf-105">Property</span></span>          | <span data-ttu-id="ad5bf-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ad5bf-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ad5bf-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ad5bf-107">reportRefreshDate</span></span> | <span data-ttu-id="ad5bf-108">Date</span><span class="sxs-lookup"><span data-stu-id="ad5bf-108">Date</span></span>   |
| <span data-ttu-id="ad5bf-109">web</span><span class="sxs-lookup"><span data-stu-id="ad5bf-109">web</span></span>               | <span data-ttu-id="ad5bf-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ad5bf-110">Int64</span></span>  |
| <span data-ttu-id="ad5bf-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="ad5bf-111">windowsPhone</span></span>      | <span data-ttu-id="ad5bf-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ad5bf-112">Int64</span></span>  |
| <span data-ttu-id="ad5bf-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="ad5bf-113">androidPhone</span></span>      | <span data-ttu-id="ad5bf-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ad5bf-114">Int64</span></span>  |
| <span data-ttu-id="ad5bf-115">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="ad5bf-115">ios</span></span>               | <span data-ttu-id="ad5bf-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ad5bf-116">Int64</span></span>  |
| <span data-ttu-id="ad5bf-117">mac</span><span class="sxs-lookup"><span data-stu-id="ad5bf-117">mac</span></span>               | <span data-ttu-id="ad5bf-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ad5bf-118">Int64</span></span>  |
| <span data-ttu-id="ad5bf-119">Windows</span><span class="sxs-lookup"><span data-stu-id="ad5bf-119">windows</span></span>           | <span data-ttu-id="ad5bf-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ad5bf-120">Int64</span></span>  |
| <span data-ttu-id="ad5bf-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="ad5bf-121">reportDate</span></span>        | <span data-ttu-id="ad5bf-122">Date</span><span class="sxs-lookup"><span data-stu-id="ad5bf-122">Date</span></span>   |
| <span data-ttu-id="ad5bf-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ad5bf-123">reportPeriod</span></span>      | <span data-ttu-id="ad5bf-124">String</span><span class="sxs-lookup"><span data-stu-id="ad5bf-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad5bf-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad5bf-125">JSON representation</span></span>

<span data-ttu-id="ad5bf-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad5bf-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
