---
title: Тип ресурса skypeForBusinessPeerToPeerActivityUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 619e581fcdd25dda10be7210aefe5db8e4dcd8b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828639"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="05d73-103">Тип ресурса skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="05d73-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="05d73-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="05d73-104">Properties</span></span>

| <span data-ttu-id="05d73-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="05d73-105">Property</span></span>          | <span data-ttu-id="05d73-106">Тип</span><span class="sxs-lookup"><span data-stu-id="05d73-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="05d73-107">обмен мгновенными сообщениями</span><span class="sxs-lookup"><span data-stu-id="05d73-107">im</span></span>                | <span data-ttu-id="05d73-108">Int64</span><span class="sxs-lookup"><span data-stu-id="05d73-108">Int64</span></span>  |
| <span data-ttu-id="05d73-109">audio</span><span class="sxs-lookup"><span data-stu-id="05d73-109">audio</span></span>             | <span data-ttu-id="05d73-110">Int64</span><span class="sxs-lookup"><span data-stu-id="05d73-110">Int64</span></span>  |
| <span data-ttu-id="05d73-111">video</span><span class="sxs-lookup"><span data-stu-id="05d73-111">video</span></span>             | <span data-ttu-id="05d73-112">Int64</span><span class="sxs-lookup"><span data-stu-id="05d73-112">Int64</span></span>  |
| <span data-ttu-id="05d73-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="05d73-113">appSharing</span></span>        | <span data-ttu-id="05d73-114">Int64</span><span class="sxs-lookup"><span data-stu-id="05d73-114">Int64</span></span>  |
| <span data-ttu-id="05d73-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="05d73-115">fileTransfer</span></span>      | <span data-ttu-id="05d73-116">Int64</span><span class="sxs-lookup"><span data-stu-id="05d73-116">Int64</span></span>  |
| <span data-ttu-id="05d73-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="05d73-117">reportRefreshDate</span></span> | <span data-ttu-id="05d73-118">Date</span><span class="sxs-lookup"><span data-stu-id="05d73-118">Date</span></span>   |
| <span data-ttu-id="05d73-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="05d73-119">reportDate</span></span>        | <span data-ttu-id="05d73-120">Date</span><span class="sxs-lookup"><span data-stu-id="05d73-120">Date</span></span>   |
| <span data-ttu-id="05d73-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="05d73-121">reportPeriod</span></span>      | <span data-ttu-id="05d73-122">String</span><span class="sxs-lookup"><span data-stu-id="05d73-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05d73-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05d73-123">JSON representation</span></span>

<span data-ttu-id="05d73-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05d73-124">The following is a JSON representation of the resource.</span></span>

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
