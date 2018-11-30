---
title: Тип ресурса sharePointActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 271ea6a70d56c55cf5a9561c2a1485c674a365f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078110"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="54f8f-103">Тип ресурса sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="54f8f-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="54f8f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="54f8f-104">Properties</span></span>

| <span data-ttu-id="54f8f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="54f8f-105">Property</span></span>          | <span data-ttu-id="54f8f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="54f8f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="54f8f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="54f8f-107">reportRefreshDate</span></span> | <span data-ttu-id="54f8f-108">Date</span><span class="sxs-lookup"><span data-stu-id="54f8f-108">Date</span></span>   |
| <span data-ttu-id="54f8f-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="54f8f-109">visitedPage</span></span>       | <span data-ttu-id="54f8f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="54f8f-110">Int64</span></span>  |
| <span data-ttu-id="54f8f-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="54f8f-111">viewedOrEdited</span></span>    | <span data-ttu-id="54f8f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="54f8f-112">Int64</span></span>  |
| <span data-ttu-id="54f8f-113">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="54f8f-113">synced</span></span>            | <span data-ttu-id="54f8f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="54f8f-114">Int64</span></span>  |
| <span data-ttu-id="54f8f-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="54f8f-115">sharedInternally</span></span>  | <span data-ttu-id="54f8f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="54f8f-116">Int64</span></span>  |
| <span data-ttu-id="54f8f-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="54f8f-117">sharedExternally</span></span>  | <span data-ttu-id="54f8f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="54f8f-118">Int64</span></span>  |
| <span data-ttu-id="54f8f-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="54f8f-119">reportDate</span></span>        | <span data-ttu-id="54f8f-120">Date</span><span class="sxs-lookup"><span data-stu-id="54f8f-120">Date</span></span>   |
| <span data-ttu-id="54f8f-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="54f8f-121">reportPeriod</span></span>      | <span data-ttu-id="54f8f-122">String</span><span class="sxs-lookup"><span data-stu-id="54f8f-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54f8f-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54f8f-123">JSON representation</span></span>

<span data-ttu-id="54f8f-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54f8f-124">The following is a JSON representation of the resource.</span></span>

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
