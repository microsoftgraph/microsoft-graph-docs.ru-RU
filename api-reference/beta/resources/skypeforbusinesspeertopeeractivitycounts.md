---
title: Тип ресурса skypeForBusinessPeerToPeerActivityCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: cdc8ec2a63c4a03ac8b77bedba06c6addfba4584
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078136"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="7c2ae-103">Тип ресурса skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="7c2ae-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7c2ae-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c2ae-104">Properties</span></span>

| <span data-ttu-id="7c2ae-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c2ae-105">Property</span></span>          | <span data-ttu-id="7c2ae-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7c2ae-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7c2ae-107">обмен мгновенными сообщениями</span><span class="sxs-lookup"><span data-stu-id="7c2ae-107">im</span></span>                | <span data-ttu-id="7c2ae-108">Int64</span><span class="sxs-lookup"><span data-stu-id="7c2ae-108">Int64</span></span>  |
| <span data-ttu-id="7c2ae-109">audio</span><span class="sxs-lookup"><span data-stu-id="7c2ae-109">audio</span></span>             | <span data-ttu-id="7c2ae-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7c2ae-110">Int64</span></span>  |
| <span data-ttu-id="7c2ae-111">video</span><span class="sxs-lookup"><span data-stu-id="7c2ae-111">video</span></span>             | <span data-ttu-id="7c2ae-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7c2ae-112">Int64</span></span>  |
| <span data-ttu-id="7c2ae-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="7c2ae-113">appSharing</span></span>        | <span data-ttu-id="7c2ae-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7c2ae-114">Int64</span></span>  |
| <span data-ttu-id="7c2ae-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="7c2ae-115">fileTransfer</span></span>      | <span data-ttu-id="7c2ae-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7c2ae-116">Int64</span></span>  |
| <span data-ttu-id="7c2ae-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7c2ae-117">reportRefreshDate</span></span> | <span data-ttu-id="7c2ae-118">Date</span><span class="sxs-lookup"><span data-stu-id="7c2ae-118">Date</span></span>   |
| <span data-ttu-id="7c2ae-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="7c2ae-119">reportDate</span></span>        | <span data-ttu-id="7c2ae-120">Date</span><span class="sxs-lookup"><span data-stu-id="7c2ae-120">Date</span></span>   |
| <span data-ttu-id="7c2ae-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7c2ae-121">reportPeriod</span></span>      | <span data-ttu-id="7c2ae-122">String</span><span class="sxs-lookup"><span data-stu-id="7c2ae-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c2ae-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c2ae-123">JSON representation</span></span>

<span data-ttu-id="7c2ae-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c2ae-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
