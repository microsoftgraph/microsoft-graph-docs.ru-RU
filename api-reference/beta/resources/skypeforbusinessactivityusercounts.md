---
title: Тип ресурса skypeForBusinessActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: eee736958540f2a3fb42cf3c76a37da4ebe78afd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082832"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a><span data-ttu-id="16761-103">Тип ресурса skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="16761-103">skypeForBusinessActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="16761-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="16761-104">Properties</span></span>

| <span data-ttu-id="16761-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="16761-105">Property</span></span>          | <span data-ttu-id="16761-106">Тип</span><span class="sxs-lookup"><span data-stu-id="16761-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="16761-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="16761-107">peerToPeer</span></span>        | <span data-ttu-id="16761-108">Int64</span><span class="sxs-lookup"><span data-stu-id="16761-108">Int64</span></span>  |
| <span data-ttu-id="16761-109">упорядоченные</span><span class="sxs-lookup"><span data-stu-id="16761-109">organized</span></span>         | <span data-ttu-id="16761-110">Int64</span><span class="sxs-lookup"><span data-stu-id="16761-110">Int64</span></span>  |
| <span data-ttu-id="16761-111">являлся</span><span class="sxs-lookup"><span data-stu-id="16761-111">participated</span></span>      | <span data-ttu-id="16761-112">Int64</span><span class="sxs-lookup"><span data-stu-id="16761-112">Int64</span></span>  |
| <span data-ttu-id="16761-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="16761-113">reportRefreshDate</span></span> | <span data-ttu-id="16761-114">Date</span><span class="sxs-lookup"><span data-stu-id="16761-114">Date</span></span>   |
| <span data-ttu-id="16761-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="16761-115">reportDate</span></span>        | <span data-ttu-id="16761-116">Date</span><span class="sxs-lookup"><span data-stu-id="16761-116">Date</span></span>   |
| <span data-ttu-id="16761-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="16761-117">reportPeriod</span></span>      | <span data-ttu-id="16761-118">String</span><span class="sxs-lookup"><span data-stu-id="16761-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16761-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16761-119">JSON representation</span></span>

<span data-ttu-id="16761-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16761-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
