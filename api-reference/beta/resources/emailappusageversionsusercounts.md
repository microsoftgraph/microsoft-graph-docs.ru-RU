---
title: Тип ресурса emailAppUsageVersionsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 371352c42e870f45224999b7a618d1bb694ea512
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965287"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="1b84c-103">Тип ресурса emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="1b84c-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1b84c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b84c-104">Properties</span></span>

| <span data-ttu-id="1b84c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b84c-105">Property</span></span>          | <span data-ttu-id="1b84c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="1b84c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1b84c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1b84c-107">reportRefreshDate</span></span> | <span data-ttu-id="1b84c-108">Date</span><span class="sxs-lookup"><span data-stu-id="1b84c-108">Date</span></span>   |
| <span data-ttu-id="1b84c-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="1b84c-109">outlook2016</span></span>       | <span data-ttu-id="1b84c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1b84c-110">Int64</span></span>  |
| <span data-ttu-id="1b84c-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="1b84c-111">outlook2013</span></span>       | <span data-ttu-id="1b84c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1b84c-112">Int64</span></span>  |
| <span data-ttu-id="1b84c-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="1b84c-113">outlook2010</span></span>       | <span data-ttu-id="1b84c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1b84c-114">Int64</span></span>  |
| <span data-ttu-id="1b84c-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="1b84c-115">outlook2007</span></span>       | <span data-ttu-id="1b84c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1b84c-116">Int64</span></span>  |
| <span data-ttu-id="1b84c-117">не определено</span><span class="sxs-lookup"><span data-stu-id="1b84c-117">undetermined</span></span>      | <span data-ttu-id="1b84c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1b84c-118">Int64</span></span>  |
| <span data-ttu-id="1b84c-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1b84c-119">reportPeriod</span></span>      | <span data-ttu-id="1b84c-120">String</span><span class="sxs-lookup"><span data-stu-id="1b84c-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1b84c-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b84c-121">JSON representation</span></span>

<span data-ttu-id="1b84c-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b84c-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
