---
title: Тип ресурса oneDriveUsageFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: ec428179cb35755e545aded70929eccd9d558fec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829535"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="6bfc8-103">Тип ресурса oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="6bfc8-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6bfc8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bfc8-104">Properties</span></span>

| <span data-ttu-id="6bfc8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bfc8-105">Property</span></span>          | <span data-ttu-id="6bfc8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6bfc8-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6bfc8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6bfc8-107">reportRefreshDate</span></span> | <span data-ttu-id="6bfc8-108">Date</span><span class="sxs-lookup"><span data-stu-id="6bfc8-108">Date</span></span>   |
| <span data-ttu-id="6bfc8-109">siteType</span><span class="sxs-lookup"><span data-stu-id="6bfc8-109">siteType</span></span>          | <span data-ttu-id="6bfc8-110">Строка</span><span class="sxs-lookup"><span data-stu-id="6bfc8-110">String</span></span> |
| <span data-ttu-id="6bfc8-111">total</span><span class="sxs-lookup"><span data-stu-id="6bfc8-111">total</span></span>             | <span data-ttu-id="6bfc8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6bfc8-112">Int64</span></span>  |
| <span data-ttu-id="6bfc8-113">активных</span><span class="sxs-lookup"><span data-stu-id="6bfc8-113">active</span></span>            | <span data-ttu-id="6bfc8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6bfc8-114">Int64</span></span>  |
| <span data-ttu-id="6bfc8-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="6bfc8-115">reportDate</span></span>        | <span data-ttu-id="6bfc8-116">Date</span><span class="sxs-lookup"><span data-stu-id="6bfc8-116">Date</span></span>   |
| <span data-ttu-id="6bfc8-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6bfc8-117">reportPeriod</span></span>      | <span data-ttu-id="6bfc8-118">String</span><span class="sxs-lookup"><span data-stu-id="6bfc8-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6bfc8-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bfc8-119">JSON representation</span></span>

<span data-ttu-id="6bfc8-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bfc8-120">The following is a JSON representation of the resource.</span></span>

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
