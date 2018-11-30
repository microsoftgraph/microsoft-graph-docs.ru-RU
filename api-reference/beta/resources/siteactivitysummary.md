---
title: Тип ресурса siteActivitySummary
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 354b329f592964249590b2f551d66681f45de485
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078546"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="0df43-103">Тип ресурса siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="0df43-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0df43-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="0df43-104">Properties</span></span>

| <span data-ttu-id="0df43-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="0df43-105">Property</span></span>          | <span data-ttu-id="0df43-106">Тип</span><span class="sxs-lookup"><span data-stu-id="0df43-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0df43-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0df43-107">reportRefreshDate</span></span> | <span data-ttu-id="0df43-108">Date</span><span class="sxs-lookup"><span data-stu-id="0df43-108">Date</span></span>   |
| <span data-ttu-id="0df43-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="0df43-109">viewedOrEdited</span></span>    | <span data-ttu-id="0df43-110">Int64</span><span class="sxs-lookup"><span data-stu-id="0df43-110">Int64</span></span>  |
| <span data-ttu-id="0df43-111">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="0df43-111">synced</span></span>            | <span data-ttu-id="0df43-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0df43-112">Int64</span></span>  |
| <span data-ttu-id="0df43-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="0df43-113">sharedInternally</span></span>  | <span data-ttu-id="0df43-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0df43-114">Int64</span></span>  |
| <span data-ttu-id="0df43-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="0df43-115">sharedExternally</span></span>  | <span data-ttu-id="0df43-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0df43-116">Int64</span></span>  |
| <span data-ttu-id="0df43-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="0df43-117">reportDate</span></span>        | <span data-ttu-id="0df43-118">Date</span><span class="sxs-lookup"><span data-stu-id="0df43-118">Date</span></span>   |
| <span data-ttu-id="0df43-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0df43-119">reportPeriod</span></span>      | <span data-ttu-id="0df43-120">String</span><span class="sxs-lookup"><span data-stu-id="0df43-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0df43-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0df43-121">JSON representation</span></span>

<span data-ttu-id="0df43-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0df43-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
