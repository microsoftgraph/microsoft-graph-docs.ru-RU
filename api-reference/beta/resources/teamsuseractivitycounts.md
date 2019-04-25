---
title: Тип ресурса Теамсусерактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582922"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="7786d-103">Тип ресурса Теамсусерактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="7786d-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7786d-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7786d-104">Properties</span></span>

| <span data-ttu-id="7786d-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7786d-105">Property</span></span>            | <span data-ttu-id="7786d-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7786d-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="7786d-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="7786d-107">reportRefreshDate</span></span>   | <span data-ttu-id="7786d-108">Дата</span><span class="sxs-lookup"><span data-stu-id="7786d-108">Date</span></span>   |
| <span data-ttu-id="7786d-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="7786d-109">reportDate</span></span>          | <span data-ttu-id="7786d-110">Дата</span><span class="sxs-lookup"><span data-stu-id="7786d-110">Date</span></span>   |
| <span data-ttu-id="7786d-111">Теамчатмессажес</span><span class="sxs-lookup"><span data-stu-id="7786d-111">teamChatMessages</span></span>    | <span data-ttu-id="7786d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7786d-112">Int64</span></span>  |
| <span data-ttu-id="7786d-113">Приватечатмессажес</span><span class="sxs-lookup"><span data-stu-id="7786d-113">privateChatMessages</span></span> | <span data-ttu-id="7786d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7786d-114">Int64</span></span>  |
| <span data-ttu-id="7786d-115">calls</span><span class="sxs-lookup"><span data-stu-id="7786d-115">calls</span></span>               | <span data-ttu-id="7786d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7786d-116">Int64</span></span>  |
| <span data-ttu-id="7786d-117">meetings</span><span class="sxs-lookup"><span data-stu-id="7786d-117">meetings</span></span>            | <span data-ttu-id="7786d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7786d-118">Int64</span></span>  |
| <span data-ttu-id="7786d-119">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="7786d-119">reportPeriod</span></span>        | <span data-ttu-id="7786d-120">String</span><span class="sxs-lookup"><span data-stu-id="7786d-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7786d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7786d-121">JSON representation</span></span>

<span data-ttu-id="7786d-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7786d-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
