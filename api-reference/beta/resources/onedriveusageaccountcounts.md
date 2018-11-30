---
title: Тип ресурса oneDriveUsageAccountCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 959d6602cec98f7351ec3d9819fb9a59599d3e6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078677"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="6d256-103">Тип ресурса oneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="6d256-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d256-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d256-104">Properties</span></span>

| <span data-ttu-id="6d256-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d256-105">Property</span></span>          | <span data-ttu-id="6d256-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6d256-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6d256-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d256-107">reportRefreshDate</span></span> | <span data-ttu-id="6d256-108">Date</span><span class="sxs-lookup"><span data-stu-id="6d256-108">Date</span></span>   |
| <span data-ttu-id="6d256-109">siteType</span><span class="sxs-lookup"><span data-stu-id="6d256-109">siteType</span></span>          | <span data-ttu-id="6d256-110">String</span><span class="sxs-lookup"><span data-stu-id="6d256-110">String</span></span> |
| <span data-ttu-id="6d256-111">total</span><span class="sxs-lookup"><span data-stu-id="6d256-111">total</span></span>             | <span data-ttu-id="6d256-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6d256-112">Int64</span></span>  |
| <span data-ttu-id="6d256-113">активных</span><span class="sxs-lookup"><span data-stu-id="6d256-113">active</span></span>            | <span data-ttu-id="6d256-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6d256-114">Int64</span></span>  |
| <span data-ttu-id="6d256-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="6d256-115">reportDate</span></span>        | <span data-ttu-id="6d256-116">Date</span><span class="sxs-lookup"><span data-stu-id="6d256-116">Date</span></span>   |
| <span data-ttu-id="6d256-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d256-117">reportPeriod</span></span>      | <span data-ttu-id="6d256-118">String</span><span class="sxs-lookup"><span data-stu-id="6d256-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d256-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d256-119">JSON representation</span></span>

<span data-ttu-id="6d256-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d256-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
