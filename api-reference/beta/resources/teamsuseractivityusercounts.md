---
title: Тип ресурса Теамсусерактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582915"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="665bc-103">Тип ресурса Теамсусерактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="665bc-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="665bc-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="665bc-104">Properties</span></span>

| <span data-ttu-id="665bc-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="665bc-105">Property</span></span>            | <span data-ttu-id="665bc-106">Тип</span><span class="sxs-lookup"><span data-stu-id="665bc-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="665bc-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="665bc-107">reportRefreshDate</span></span>   | <span data-ttu-id="665bc-108">Дата</span><span class="sxs-lookup"><span data-stu-id="665bc-108">Date</span></span>   |
| <span data-ttu-id="665bc-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="665bc-109">reportDate</span></span>          | <span data-ttu-id="665bc-110">Дата</span><span class="sxs-lookup"><span data-stu-id="665bc-110">Date</span></span>   |
| <span data-ttu-id="665bc-111">Теамчатмессажес</span><span class="sxs-lookup"><span data-stu-id="665bc-111">teamChatMessages</span></span>    | <span data-ttu-id="665bc-112">Int64</span><span class="sxs-lookup"><span data-stu-id="665bc-112">Int64</span></span>  |
| <span data-ttu-id="665bc-113">Приватечатмессажес</span><span class="sxs-lookup"><span data-stu-id="665bc-113">privateChatMessages</span></span> | <span data-ttu-id="665bc-114">Int64</span><span class="sxs-lookup"><span data-stu-id="665bc-114">Int64</span></span>  |
| <span data-ttu-id="665bc-115">calls</span><span class="sxs-lookup"><span data-stu-id="665bc-115">calls</span></span>               | <span data-ttu-id="665bc-116">Int64</span><span class="sxs-lookup"><span data-stu-id="665bc-116">Int64</span></span>  |
| <span data-ttu-id="665bc-117">meetings</span><span class="sxs-lookup"><span data-stu-id="665bc-117">meetings</span></span>            | <span data-ttu-id="665bc-118">Int64</span><span class="sxs-lookup"><span data-stu-id="665bc-118">Int64</span></span>  |
| <span data-ttu-id="665bc-119">Осерактионс</span><span class="sxs-lookup"><span data-stu-id="665bc-119">otherActions</span></span>        | <span data-ttu-id="665bc-120">Int64</span><span class="sxs-lookup"><span data-stu-id="665bc-120">Int64</span></span>  |
| <span data-ttu-id="665bc-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="665bc-121">reportPeriod</span></span>        | <span data-ttu-id="665bc-122">String</span><span class="sxs-lookup"><span data-stu-id="665bc-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="665bc-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="665bc-123">JSON representation</span></span>

<span data-ttu-id="665bc-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="665bc-124">The following is a JSON representation of the resource.</span></span>

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
