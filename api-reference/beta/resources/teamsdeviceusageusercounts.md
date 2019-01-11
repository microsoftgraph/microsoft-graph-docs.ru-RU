---
title: Тип ресурса teamsDeviceUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 07a43b024d133e5ac1d8eb8a2665fd3027001edb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857353"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="1001a-103">Тип ресурса teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="1001a-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1001a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="1001a-104">Properties</span></span>

| <span data-ttu-id="1001a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="1001a-105">Property</span></span>          | <span data-ttu-id="1001a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="1001a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1001a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1001a-107">reportRefreshDate</span></span> | <span data-ttu-id="1001a-108">Date</span><span class="sxs-lookup"><span data-stu-id="1001a-108">Date</span></span>   |
| <span data-ttu-id="1001a-109">web</span><span class="sxs-lookup"><span data-stu-id="1001a-109">web</span></span>               | <span data-ttu-id="1001a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1001a-110">Int64</span></span>  |
| <span data-ttu-id="1001a-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="1001a-111">windowsPhone</span></span>      | <span data-ttu-id="1001a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1001a-112">Int64</span></span>  |
| <span data-ttu-id="1001a-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="1001a-113">androidPhone</span></span>      | <span data-ttu-id="1001a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1001a-114">Int64</span></span>  |
| <span data-ttu-id="1001a-115">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="1001a-115">ios</span></span>               | <span data-ttu-id="1001a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1001a-116">Int64</span></span>  |
| <span data-ttu-id="1001a-117">mac</span><span class="sxs-lookup"><span data-stu-id="1001a-117">mac</span></span>               | <span data-ttu-id="1001a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1001a-118">Int64</span></span>  |
| <span data-ttu-id="1001a-119">Windows</span><span class="sxs-lookup"><span data-stu-id="1001a-119">windows</span></span>           | <span data-ttu-id="1001a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1001a-120">Int64</span></span>  |
| <span data-ttu-id="1001a-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="1001a-121">reportDate</span></span>        | <span data-ttu-id="1001a-122">Date</span><span class="sxs-lookup"><span data-stu-id="1001a-122">Date</span></span>   |
| <span data-ttu-id="1001a-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1001a-123">reportPeriod</span></span>      | <span data-ttu-id="1001a-124">String</span><span class="sxs-lookup"><span data-stu-id="1001a-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1001a-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1001a-125">JSON representation</span></span>

<span data-ttu-id="1001a-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1001a-126">The following is a JSON representation of the resource.</span></span>

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
