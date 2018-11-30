---
title: Тип ресурса skypeForBusinessDeviceUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 3ae63d942ef21152e54f3bf5234d1b9d8df9649b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076449"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="462f5-103">Тип ресурса skypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="462f5-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="462f5-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="462f5-104">Properties</span></span>

| <span data-ttu-id="462f5-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="462f5-105">Property</span></span>          | <span data-ttu-id="462f5-106">Тип</span><span class="sxs-lookup"><span data-stu-id="462f5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="462f5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="462f5-107">reportRefreshDate</span></span> | <span data-ttu-id="462f5-108">Date</span><span class="sxs-lookup"><span data-stu-id="462f5-108">Date</span></span>   |
| <span data-ttu-id="462f5-109">Windows</span><span class="sxs-lookup"><span data-stu-id="462f5-109">windows</span></span>           | <span data-ttu-id="462f5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="462f5-110">Int64</span></span>  |
| <span data-ttu-id="462f5-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="462f5-111">windowsPhone</span></span>      | <span data-ttu-id="462f5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="462f5-112">Int64</span></span>  |
| <span data-ttu-id="462f5-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="462f5-113">androidPhone</span></span>      | <span data-ttu-id="462f5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="462f5-114">Int64</span></span>  |
| <span data-ttu-id="462f5-115">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="462f5-115">iPhone</span></span>            | <span data-ttu-id="462f5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="462f5-116">Int64</span></span>  |
| <span data-ttu-id="462f5-117">"iPad";</span><span class="sxs-lookup"><span data-stu-id="462f5-117">iPad</span></span>              | <span data-ttu-id="462f5-118">Int64</span><span class="sxs-lookup"><span data-stu-id="462f5-118">Int64</span></span>  |
| <span data-ttu-id="462f5-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="462f5-119">reportDate</span></span>        | <span data-ttu-id="462f5-120">Date</span><span class="sxs-lookup"><span data-stu-id="462f5-120">Date</span></span>   |
| <span data-ttu-id="462f5-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="462f5-121">reportPeriod</span></span>      | <span data-ttu-id="462f5-122">String</span><span class="sxs-lookup"><span data-stu-id="462f5-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="462f5-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="462f5-123">JSON representation</span></span>

<span data-ttu-id="462f5-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="462f5-124">The following is a JSON representation of the resource.</span></span>

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
