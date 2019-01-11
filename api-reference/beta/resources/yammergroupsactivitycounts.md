---
title: Тип ресурса yammerGroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: f8a205c2ecd74e8543a220508e7d4110a90317cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806792"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="bed94-103">Тип ресурса yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="bed94-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bed94-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="bed94-104">Properties</span></span>

| <span data-ttu-id="bed94-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="bed94-105">Property</span></span>          | <span data-ttu-id="bed94-106">Тип</span><span class="sxs-lookup"><span data-stu-id="bed94-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="bed94-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bed94-107">reportRefreshDate</span></span> | <span data-ttu-id="bed94-108">Date</span><span class="sxs-lookup"><span data-stu-id="bed94-108">Date</span></span>   |
| <span data-ttu-id="bed94-109">нравится, что</span><span class="sxs-lookup"><span data-stu-id="bed94-109">liked</span></span>             | <span data-ttu-id="bed94-110">Int64</span><span class="sxs-lookup"><span data-stu-id="bed94-110">Int64</span></span>  |
| <span data-ttu-id="bed94-111">учтена</span><span class="sxs-lookup"><span data-stu-id="bed94-111">posted</span></span>            | <span data-ttu-id="bed94-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bed94-112">Int64</span></span>  |
| <span data-ttu-id="bed94-113">чтение</span><span class="sxs-lookup"><span data-stu-id="bed94-113">read</span></span>              | <span data-ttu-id="bed94-114">Int64</span><span class="sxs-lookup"><span data-stu-id="bed94-114">Int64</span></span>  |
| <span data-ttu-id="bed94-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="bed94-115">reportDate</span></span>        | <span data-ttu-id="bed94-116">Date</span><span class="sxs-lookup"><span data-stu-id="bed94-116">Date</span></span>   |
| <span data-ttu-id="bed94-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bed94-117">reportPeriod</span></span>      | <span data-ttu-id="bed94-118">String</span><span class="sxs-lookup"><span data-stu-id="bed94-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bed94-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bed94-119">JSON representation</span></span>

<span data-ttu-id="bed94-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bed94-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
