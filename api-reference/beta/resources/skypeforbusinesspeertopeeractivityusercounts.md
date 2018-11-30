---
title: Тип ресурса skypeForBusinessPeerToPeerActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: ad3b409f3abc4cc9e7476825f9dbf5b7c2120d92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079811"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="5bfae-103">Тип ресурса skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="5bfae-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5bfae-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bfae-104">Properties</span></span>

| <span data-ttu-id="5bfae-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bfae-105">Property</span></span>          | <span data-ttu-id="5bfae-106">Тип</span><span class="sxs-lookup"><span data-stu-id="5bfae-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5bfae-107">обмен мгновенными сообщениями</span><span class="sxs-lookup"><span data-stu-id="5bfae-107">im</span></span>                | <span data-ttu-id="5bfae-108">Int64</span><span class="sxs-lookup"><span data-stu-id="5bfae-108">Int64</span></span>  |
| <span data-ttu-id="5bfae-109">audio</span><span class="sxs-lookup"><span data-stu-id="5bfae-109">audio</span></span>             | <span data-ttu-id="5bfae-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5bfae-110">Int64</span></span>  |
| <span data-ttu-id="5bfae-111">video</span><span class="sxs-lookup"><span data-stu-id="5bfae-111">video</span></span>             | <span data-ttu-id="5bfae-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5bfae-112">Int64</span></span>  |
| <span data-ttu-id="5bfae-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="5bfae-113">appSharing</span></span>        | <span data-ttu-id="5bfae-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5bfae-114">Int64</span></span>  |
| <span data-ttu-id="5bfae-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="5bfae-115">fileTransfer</span></span>      | <span data-ttu-id="5bfae-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5bfae-116">Int64</span></span>  |
| <span data-ttu-id="5bfae-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5bfae-117">reportRefreshDate</span></span> | <span data-ttu-id="5bfae-118">Date</span><span class="sxs-lookup"><span data-stu-id="5bfae-118">Date</span></span>   |
| <span data-ttu-id="5bfae-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="5bfae-119">reportDate</span></span>        | <span data-ttu-id="5bfae-120">Date</span><span class="sxs-lookup"><span data-stu-id="5bfae-120">Date</span></span>   |
| <span data-ttu-id="5bfae-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5bfae-121">reportPeriod</span></span>      | <span data-ttu-id="5bfae-122">String</span><span class="sxs-lookup"><span data-stu-id="5bfae-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5bfae-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bfae-123">JSON representation</span></span>

<span data-ttu-id="5bfae-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bfae-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
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
