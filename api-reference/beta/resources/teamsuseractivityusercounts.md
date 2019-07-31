---
title: Тип ресурса Теамсусерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f0b6d9d77518b6e40a5793c6715bfbae69600f3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964363"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="1f40a-103">Тип ресурса Теамсусерактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="1f40a-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1f40a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f40a-104">Properties</span></span>

| <span data-ttu-id="1f40a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f40a-105">Property</span></span>            | <span data-ttu-id="1f40a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="1f40a-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="1f40a-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="1f40a-107">reportRefreshDate</span></span>   | <span data-ttu-id="1f40a-108">Дата</span><span class="sxs-lookup"><span data-stu-id="1f40a-108">Date</span></span>   |
| <span data-ttu-id="1f40a-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="1f40a-109">reportDate</span></span>          | <span data-ttu-id="1f40a-110">Дата</span><span class="sxs-lookup"><span data-stu-id="1f40a-110">Date</span></span>   |
| <span data-ttu-id="1f40a-111">Теамчатмессажес</span><span class="sxs-lookup"><span data-stu-id="1f40a-111">teamChatMessages</span></span>    | <span data-ttu-id="1f40a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1f40a-112">Int64</span></span>  |
| <span data-ttu-id="1f40a-113">Приватечатмессажес</span><span class="sxs-lookup"><span data-stu-id="1f40a-113">privateChatMessages</span></span> | <span data-ttu-id="1f40a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1f40a-114">Int64</span></span>  |
| <span data-ttu-id="1f40a-115">calls</span><span class="sxs-lookup"><span data-stu-id="1f40a-115">calls</span></span>               | <span data-ttu-id="1f40a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1f40a-116">Int64</span></span>  |
| <span data-ttu-id="1f40a-117">meetings</span><span class="sxs-lookup"><span data-stu-id="1f40a-117">meetings</span></span>            | <span data-ttu-id="1f40a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1f40a-118">Int64</span></span>  |
| <span data-ttu-id="1f40a-119">Осерактионс</span><span class="sxs-lookup"><span data-stu-id="1f40a-119">otherActions</span></span>        | <span data-ttu-id="1f40a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1f40a-120">Int64</span></span>  |
| <span data-ttu-id="1f40a-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="1f40a-121">reportPeriod</span></span>        | <span data-ttu-id="1f40a-122">String</span><span class="sxs-lookup"><span data-stu-id="1f40a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1f40a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f40a-123">JSON representation</span></span>

<span data-ttu-id="1f40a-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f40a-124">The following is a JSON representation of the resource.</span></span>

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
