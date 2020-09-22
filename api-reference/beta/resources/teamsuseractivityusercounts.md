---
title: Тип ресурса Теамсусерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3982b679802a2ca80eac5fe4e8f76fee91bbf1d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046351"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="41c29-103">Тип ресурса Теамсусерактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="41c29-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="41c29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41c29-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="41c29-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="41c29-105">Properties</span></span>

| <span data-ttu-id="41c29-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="41c29-106">Property</span></span>            | <span data-ttu-id="41c29-107">Тип</span><span class="sxs-lookup"><span data-stu-id="41c29-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="41c29-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="41c29-108">reportRefreshDate</span></span>   | <span data-ttu-id="41c29-109">Дата</span><span class="sxs-lookup"><span data-stu-id="41c29-109">Date</span></span>   |
| <span data-ttu-id="41c29-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="41c29-110">reportDate</span></span>          | <span data-ttu-id="41c29-111">Дата</span><span class="sxs-lookup"><span data-stu-id="41c29-111">Date</span></span>   |
| <span data-ttu-id="41c29-112">теамчатмессажес</span><span class="sxs-lookup"><span data-stu-id="41c29-112">teamChatMessages</span></span>    | <span data-ttu-id="41c29-113">Int64</span><span class="sxs-lookup"><span data-stu-id="41c29-113">Int64</span></span>  |
| <span data-ttu-id="41c29-114">приватечатмессажес</span><span class="sxs-lookup"><span data-stu-id="41c29-114">privateChatMessages</span></span> | <span data-ttu-id="41c29-115">Int64</span><span class="sxs-lookup"><span data-stu-id="41c29-115">Int64</span></span>  |
| <span data-ttu-id="41c29-116">calls</span><span class="sxs-lookup"><span data-stu-id="41c29-116">calls</span></span>               | <span data-ttu-id="41c29-117">Int64</span><span class="sxs-lookup"><span data-stu-id="41c29-117">Int64</span></span>  |
| <span data-ttu-id="41c29-118">meetings</span><span class="sxs-lookup"><span data-stu-id="41c29-118">meetings</span></span>            | <span data-ttu-id="41c29-119">Int64</span><span class="sxs-lookup"><span data-stu-id="41c29-119">Int64</span></span>  |
| <span data-ttu-id="41c29-120">осерактионс</span><span class="sxs-lookup"><span data-stu-id="41c29-120">otherActions</span></span>        | <span data-ttu-id="41c29-121">Int64</span><span class="sxs-lookup"><span data-stu-id="41c29-121">Int64</span></span>  |
| <span data-ttu-id="41c29-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="41c29-122">reportPeriod</span></span>        | <span data-ttu-id="41c29-123">Строка</span><span class="sxs-lookup"><span data-stu-id="41c29-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41c29-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41c29-124">JSON representation</span></span>

<span data-ttu-id="41c29-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41c29-125">The following is a JSON representation of the resource.</span></span>

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


