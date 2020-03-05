---
title: Тип ресурса Теамсусерактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3066877d109e7dd61243b7cd2f4c105b03c0c533
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519829"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="5561b-103">Тип ресурса Теамсусерактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="5561b-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="5561b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5561b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5561b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5561b-105">Properties</span></span>

| <span data-ttu-id="5561b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5561b-106">Property</span></span>            | <span data-ttu-id="5561b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5561b-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="5561b-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="5561b-108">reportRefreshDate</span></span>   | <span data-ttu-id="5561b-109">Дата</span><span class="sxs-lookup"><span data-stu-id="5561b-109">Date</span></span>   |
| <span data-ttu-id="5561b-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="5561b-110">reportDate</span></span>          | <span data-ttu-id="5561b-111">Дата</span><span class="sxs-lookup"><span data-stu-id="5561b-111">Date</span></span>   |
| <span data-ttu-id="5561b-112">теамчатмессажес</span><span class="sxs-lookup"><span data-stu-id="5561b-112">teamChatMessages</span></span>    | <span data-ttu-id="5561b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5561b-113">Int64</span></span>  |
| <span data-ttu-id="5561b-114">приватечатмессажес</span><span class="sxs-lookup"><span data-stu-id="5561b-114">privateChatMessages</span></span> | <span data-ttu-id="5561b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5561b-115">Int64</span></span>  |
| <span data-ttu-id="5561b-116">calls</span><span class="sxs-lookup"><span data-stu-id="5561b-116">calls</span></span>               | <span data-ttu-id="5561b-117">Int64</span><span class="sxs-lookup"><span data-stu-id="5561b-117">Int64</span></span>  |
| <span data-ttu-id="5561b-118">meetings</span><span class="sxs-lookup"><span data-stu-id="5561b-118">meetings</span></span>            | <span data-ttu-id="5561b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5561b-119">Int64</span></span>  |
| <span data-ttu-id="5561b-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="5561b-120">reportPeriod</span></span>        | <span data-ttu-id="5561b-121">String</span><span class="sxs-lookup"><span data-stu-id="5561b-121">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="5561b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5561b-122">JSON representation</span></span>

<span data-ttu-id="5561b-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5561b-123">The following is a JSON representation of the resource.</span></span>

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
