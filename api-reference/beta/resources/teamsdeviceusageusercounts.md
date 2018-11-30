---
title: Тип ресурса teamsDeviceUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 9640af67efc18f0a70c636673169e884ce82d971
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082099"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="6ce73-103">Тип ресурса teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="6ce73-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6ce73-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ce73-104">Properties</span></span>

| <span data-ttu-id="6ce73-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ce73-105">Property</span></span>          | <span data-ttu-id="6ce73-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6ce73-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6ce73-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6ce73-107">reportRefreshDate</span></span> | <span data-ttu-id="6ce73-108">Date</span><span class="sxs-lookup"><span data-stu-id="6ce73-108">Date</span></span>   |
| <span data-ttu-id="6ce73-109">web</span><span class="sxs-lookup"><span data-stu-id="6ce73-109">web</span></span>               | <span data-ttu-id="6ce73-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6ce73-110">Int64</span></span>  |
| <span data-ttu-id="6ce73-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="6ce73-111">windowsPhone</span></span>      | <span data-ttu-id="6ce73-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6ce73-112">Int64</span></span>  |
| <span data-ttu-id="6ce73-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="6ce73-113">androidPhone</span></span>      | <span data-ttu-id="6ce73-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6ce73-114">Int64</span></span>  |
| <span data-ttu-id="6ce73-115">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="6ce73-115">ios</span></span>               | <span data-ttu-id="6ce73-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6ce73-116">Int64</span></span>  |
| <span data-ttu-id="6ce73-117">mac</span><span class="sxs-lookup"><span data-stu-id="6ce73-117">mac</span></span>               | <span data-ttu-id="6ce73-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6ce73-118">Int64</span></span>  |
| <span data-ttu-id="6ce73-119">Windows</span><span class="sxs-lookup"><span data-stu-id="6ce73-119">windows</span></span>           | <span data-ttu-id="6ce73-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6ce73-120">Int64</span></span>  |
| <span data-ttu-id="6ce73-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="6ce73-121">reportDate</span></span>        | <span data-ttu-id="6ce73-122">Date</span><span class="sxs-lookup"><span data-stu-id="6ce73-122">Date</span></span>   |
| <span data-ttu-id="6ce73-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6ce73-123">reportPeriod</span></span>      | <span data-ttu-id="6ce73-124">String</span><span class="sxs-lookup"><span data-stu-id="6ce73-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ce73-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ce73-125">JSON representation</span></span>

<span data-ttu-id="6ce73-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ce73-126">The following is a JSON representation of the resource.</span></span>

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
