---
title: Тип ресурса mailboxUsageStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: dcabfab0e8a64f2d74442f7d7464708501a59b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840742"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="f33ad-103">Тип ресурса mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="f33ad-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f33ad-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f33ad-104">Properties</span></span>

| <span data-ttu-id="f33ad-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f33ad-105">Property</span></span>           | <span data-ttu-id="f33ad-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f33ad-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="f33ad-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f33ad-107">reportRefreshDate</span></span>  | <span data-ttu-id="f33ad-108">Date</span><span class="sxs-lookup"><span data-stu-id="f33ad-108">Date</span></span>   |
| <span data-ttu-id="f33ad-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="f33ad-109">storageUsedInBytes</span></span> | <span data-ttu-id="f33ad-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f33ad-110">Int64</span></span>  |
| <span data-ttu-id="f33ad-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="f33ad-111">reportDate</span></span>         | <span data-ttu-id="f33ad-112">Date</span><span class="sxs-lookup"><span data-stu-id="f33ad-112">Date</span></span>   |
| <span data-ttu-id="f33ad-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f33ad-113">reportPeriod</span></span>       | <span data-ttu-id="f33ad-114">String</span><span class="sxs-lookup"><span data-stu-id="f33ad-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f33ad-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f33ad-115">JSON representation</span></span>

<span data-ttu-id="f33ad-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f33ad-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
