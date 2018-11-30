---
title: Тип ресурса oneDriveUsageFileCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 98e387b97687a4aab55e8d94e72fdbfa585a0e84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075718"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="17448-103">Тип ресурса oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="17448-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="17448-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="17448-104">Properties</span></span>

| <span data-ttu-id="17448-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="17448-105">Property</span></span>          | <span data-ttu-id="17448-106">Тип</span><span class="sxs-lookup"><span data-stu-id="17448-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="17448-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="17448-107">reportRefreshDate</span></span> | <span data-ttu-id="17448-108">Date</span><span class="sxs-lookup"><span data-stu-id="17448-108">Date</span></span>   |
| <span data-ttu-id="17448-109">siteType</span><span class="sxs-lookup"><span data-stu-id="17448-109">siteType</span></span>          | <span data-ttu-id="17448-110">String</span><span class="sxs-lookup"><span data-stu-id="17448-110">String</span></span> |
| <span data-ttu-id="17448-111">total</span><span class="sxs-lookup"><span data-stu-id="17448-111">total</span></span>             | <span data-ttu-id="17448-112">Int64</span><span class="sxs-lookup"><span data-stu-id="17448-112">Int64</span></span>  |
| <span data-ttu-id="17448-113">активных</span><span class="sxs-lookup"><span data-stu-id="17448-113">active</span></span>            | <span data-ttu-id="17448-114">Int64</span><span class="sxs-lookup"><span data-stu-id="17448-114">Int64</span></span>  |
| <span data-ttu-id="17448-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="17448-115">reportDate</span></span>        | <span data-ttu-id="17448-116">Date</span><span class="sxs-lookup"><span data-stu-id="17448-116">Date</span></span>   |
| <span data-ttu-id="17448-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="17448-117">reportPeriod</span></span>      | <span data-ttu-id="17448-118">String</span><span class="sxs-lookup"><span data-stu-id="17448-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17448-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17448-119">JSON representation</span></span>

<span data-ttu-id="17448-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17448-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
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
