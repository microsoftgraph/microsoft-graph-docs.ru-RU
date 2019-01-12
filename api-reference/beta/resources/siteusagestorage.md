---
title: Тип ресурса siteUsageStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928103"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="bafa0-103">Тип ресурса siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="bafa0-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bafa0-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="bafa0-104">Properties</span></span>

| <span data-ttu-id="bafa0-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="bafa0-105">Property</span></span>           | <span data-ttu-id="bafa0-106">Тип</span><span class="sxs-lookup"><span data-stu-id="bafa0-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="bafa0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bafa0-107">reportRefreshDate</span></span>  | <span data-ttu-id="bafa0-108">Date</span><span class="sxs-lookup"><span data-stu-id="bafa0-108">Date</span></span>   |
| <span data-ttu-id="bafa0-109">siteType</span><span class="sxs-lookup"><span data-stu-id="bafa0-109">siteType</span></span>           | <span data-ttu-id="bafa0-110">Строка</span><span class="sxs-lookup"><span data-stu-id="bafa0-110">String</span></span> |
| <span data-ttu-id="bafa0-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="bafa0-111">storageUsedInBytes</span></span> | <span data-ttu-id="bafa0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bafa0-112">Int64</span></span>  |
| <span data-ttu-id="bafa0-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="bafa0-113">reportDate</span></span>         | <span data-ttu-id="bafa0-114">Date</span><span class="sxs-lookup"><span data-stu-id="bafa0-114">Date</span></span>   |
| <span data-ttu-id="bafa0-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bafa0-115">reportPeriod</span></span>       | <span data-ttu-id="bafa0-116">String</span><span class="sxs-lookup"><span data-stu-id="bafa0-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bafa0-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bafa0-117">JSON representation</span></span>

<span data-ttu-id="bafa0-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bafa0-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
