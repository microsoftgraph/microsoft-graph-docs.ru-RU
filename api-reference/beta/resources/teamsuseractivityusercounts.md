---
title: Тип ресурса Теамсусерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7a330223a7b72b32387998d458456f0661979ae2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519822"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="7423f-103">Тип ресурса Теамсусерактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="7423f-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="7423f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7423f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="7423f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7423f-105">Properties</span></span>

| <span data-ttu-id="7423f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7423f-106">Property</span></span>            | <span data-ttu-id="7423f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7423f-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="7423f-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="7423f-108">reportRefreshDate</span></span>   | <span data-ttu-id="7423f-109">Дата</span><span class="sxs-lookup"><span data-stu-id="7423f-109">Date</span></span>   |
| <span data-ttu-id="7423f-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="7423f-110">reportDate</span></span>          | <span data-ttu-id="7423f-111">Дата</span><span class="sxs-lookup"><span data-stu-id="7423f-111">Date</span></span>   |
| <span data-ttu-id="7423f-112">теамчатмессажес</span><span class="sxs-lookup"><span data-stu-id="7423f-112">teamChatMessages</span></span>    | <span data-ttu-id="7423f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="7423f-113">Int64</span></span>  |
| <span data-ttu-id="7423f-114">приватечатмессажес</span><span class="sxs-lookup"><span data-stu-id="7423f-114">privateChatMessages</span></span> | <span data-ttu-id="7423f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7423f-115">Int64</span></span>  |
| <span data-ttu-id="7423f-116">calls</span><span class="sxs-lookup"><span data-stu-id="7423f-116">calls</span></span>               | <span data-ttu-id="7423f-117">Int64</span><span class="sxs-lookup"><span data-stu-id="7423f-117">Int64</span></span>  |
| <span data-ttu-id="7423f-118">meetings</span><span class="sxs-lookup"><span data-stu-id="7423f-118">meetings</span></span>            | <span data-ttu-id="7423f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="7423f-119">Int64</span></span>  |
| <span data-ttu-id="7423f-120">осерактионс</span><span class="sxs-lookup"><span data-stu-id="7423f-120">otherActions</span></span>        | <span data-ttu-id="7423f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="7423f-121">Int64</span></span>  |
| <span data-ttu-id="7423f-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="7423f-122">reportPeriod</span></span>        | <span data-ttu-id="7423f-123">String</span><span class="sxs-lookup"><span data-stu-id="7423f-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7423f-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7423f-124">JSON representation</span></span>

<span data-ttu-id="7423f-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7423f-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
