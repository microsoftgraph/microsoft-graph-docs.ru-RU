---
title: Тип ресурса Теамсусерактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 68eb66cbd0e076d9cf2559170fee4c81dca1e65c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046344"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="c4777-103">Тип ресурса Теамсусерактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="c4777-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="c4777-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4777-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c4777-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4777-105">Properties</span></span>

| <span data-ttu-id="c4777-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4777-106">Property</span></span>            | <span data-ttu-id="c4777-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c4777-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="c4777-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c4777-108">reportRefreshDate</span></span>   | <span data-ttu-id="c4777-109">Дата</span><span class="sxs-lookup"><span data-stu-id="c4777-109">Date</span></span>   |
| <span data-ttu-id="c4777-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="c4777-110">reportDate</span></span>          | <span data-ttu-id="c4777-111">Дата</span><span class="sxs-lookup"><span data-stu-id="c4777-111">Date</span></span>   |
| <span data-ttu-id="c4777-112">теамчатмессажес</span><span class="sxs-lookup"><span data-stu-id="c4777-112">teamChatMessages</span></span>    | <span data-ttu-id="c4777-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c4777-113">Int64</span></span>  |
| <span data-ttu-id="c4777-114">приватечатмессажес</span><span class="sxs-lookup"><span data-stu-id="c4777-114">privateChatMessages</span></span> | <span data-ttu-id="c4777-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c4777-115">Int64</span></span>  |
| <span data-ttu-id="c4777-116">calls</span><span class="sxs-lookup"><span data-stu-id="c4777-116">calls</span></span>               | <span data-ttu-id="c4777-117">Int64</span><span class="sxs-lookup"><span data-stu-id="c4777-117">Int64</span></span>  |
| <span data-ttu-id="c4777-118">meetings</span><span class="sxs-lookup"><span data-stu-id="c4777-118">meetings</span></span>            | <span data-ttu-id="c4777-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c4777-119">Int64</span></span>  |
| <span data-ttu-id="c4777-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="c4777-120">reportPeriod</span></span>        | <span data-ttu-id="c4777-121">Строка</span><span class="sxs-lookup"><span data-stu-id="c4777-121">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c4777-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4777-122">JSON representation</span></span>

<span data-ttu-id="c4777-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4777-123">The following is a JSON representation of the resource.</span></span>

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


