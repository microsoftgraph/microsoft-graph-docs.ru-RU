---
title: Тип ресурса sharePointActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9656b39572eac5b6474dd7884eb7d1d2edb17310
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984726"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="6e318-103">Тип ресурса sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="6e318-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6e318-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e318-104">Properties</span></span>

| <span data-ttu-id="6e318-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e318-105">Property</span></span>          | <span data-ttu-id="6e318-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6e318-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6e318-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6e318-107">reportRefreshDate</span></span> | <span data-ttu-id="6e318-108">Date</span><span class="sxs-lookup"><span data-stu-id="6e318-108">Date</span></span>   |
| <span data-ttu-id="6e318-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="6e318-109">visitedPage</span></span>       | <span data-ttu-id="6e318-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6e318-110">Int64</span></span>  |
| <span data-ttu-id="6e318-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="6e318-111">viewedOrEdited</span></span>    | <span data-ttu-id="6e318-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6e318-112">Int64</span></span>  |
| <span data-ttu-id="6e318-113">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="6e318-113">synced</span></span>            | <span data-ttu-id="6e318-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6e318-114">Int64</span></span>  |
| <span data-ttu-id="6e318-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="6e318-115">sharedInternally</span></span>  | <span data-ttu-id="6e318-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6e318-116">Int64</span></span>  |
| <span data-ttu-id="6e318-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="6e318-117">sharedExternally</span></span>  | <span data-ttu-id="6e318-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6e318-118">Int64</span></span>  |
| <span data-ttu-id="6e318-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="6e318-119">reportDate</span></span>        | <span data-ttu-id="6e318-120">Date</span><span class="sxs-lookup"><span data-stu-id="6e318-120">Date</span></span>   |
| <span data-ttu-id="6e318-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6e318-121">reportPeriod</span></span>      | <span data-ttu-id="6e318-122">String</span><span class="sxs-lookup"><span data-stu-id="6e318-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e318-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e318-123">JSON representation</span></span>

<span data-ttu-id="6e318-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e318-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPage": 1024, 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
