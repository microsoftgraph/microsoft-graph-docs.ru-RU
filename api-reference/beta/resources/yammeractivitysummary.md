---
title: Тип ресурса yammerActivitySummary
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 6ff2b347de77f91c96cb5f5be797eb70db0bbbee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075767"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="dfdb2-103">Тип ресурса yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="dfdb2-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dfdb2-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfdb2-104">Properties</span></span>

| <span data-ttu-id="dfdb2-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfdb2-105">Property</span></span>          | <span data-ttu-id="dfdb2-106">Тип</span><span class="sxs-lookup"><span data-stu-id="dfdb2-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="dfdb2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dfdb2-107">reportRefreshDate</span></span> | <span data-ttu-id="dfdb2-108">Date</span><span class="sxs-lookup"><span data-stu-id="dfdb2-108">Date</span></span>   |
| <span data-ttu-id="dfdb2-109">нравится, что</span><span class="sxs-lookup"><span data-stu-id="dfdb2-109">liked</span></span>             | <span data-ttu-id="dfdb2-110">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb2-110">Int64</span></span>  |
| <span data-ttu-id="dfdb2-111">учтена</span><span class="sxs-lookup"><span data-stu-id="dfdb2-111">posted</span></span>            | <span data-ttu-id="dfdb2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb2-112">Int64</span></span>  |
| <span data-ttu-id="dfdb2-113">чтение</span><span class="sxs-lookup"><span data-stu-id="dfdb2-113">read</span></span>              | <span data-ttu-id="dfdb2-114">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdb2-114">Int64</span></span>  |
| <span data-ttu-id="dfdb2-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="dfdb2-115">reportDate</span></span>        | <span data-ttu-id="dfdb2-116">Date</span><span class="sxs-lookup"><span data-stu-id="dfdb2-116">Date</span></span>   |
| <span data-ttu-id="dfdb2-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="dfdb2-117">reportPeriod</span></span>      | <span data-ttu-id="dfdb2-118">String</span><span class="sxs-lookup"><span data-stu-id="dfdb2-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dfdb2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfdb2-119">JSON representation</span></span>

<span data-ttu-id="dfdb2-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfdb2-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
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
