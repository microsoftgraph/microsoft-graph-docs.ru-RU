---
title: Тип ресурса siteUsageStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 1f656feacdbba3418049bd9f3072270aa04af798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879928"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="493ef-103">Тип ресурса siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="493ef-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="493ef-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="493ef-104">Properties</span></span>

| <span data-ttu-id="493ef-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="493ef-105">Property</span></span>           | <span data-ttu-id="493ef-106">Тип</span><span class="sxs-lookup"><span data-stu-id="493ef-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="493ef-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="493ef-107">reportRefreshDate</span></span>  | <span data-ttu-id="493ef-108">Date</span><span class="sxs-lookup"><span data-stu-id="493ef-108">Date</span></span>   |
| <span data-ttu-id="493ef-109">siteType</span><span class="sxs-lookup"><span data-stu-id="493ef-109">siteType</span></span>           | <span data-ttu-id="493ef-110">Строка</span><span class="sxs-lookup"><span data-stu-id="493ef-110">String</span></span> |
| <span data-ttu-id="493ef-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="493ef-111">storageUsedInBytes</span></span> | <span data-ttu-id="493ef-112">Int64</span><span class="sxs-lookup"><span data-stu-id="493ef-112">Int64</span></span>  |
| <span data-ttu-id="493ef-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="493ef-113">reportDate</span></span>         | <span data-ttu-id="493ef-114">Date</span><span class="sxs-lookup"><span data-stu-id="493ef-114">Date</span></span>   |
| <span data-ttu-id="493ef-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="493ef-115">reportPeriod</span></span>       | <span data-ttu-id="493ef-116">String</span><span class="sxs-lookup"><span data-stu-id="493ef-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="493ef-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="493ef-117">JSON representation</span></span>

<span data-ttu-id="493ef-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="493ef-118">The following is a JSON representation of the resource.</span></span>

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
