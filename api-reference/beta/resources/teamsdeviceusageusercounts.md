---
title: Тип ресурса Теамсдевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99cb675880962591d6298062f979f0930bc0a15d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964398"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="3c1c3-103">Тип ресурса Теамсдевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="3c1c3-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3c1c3-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c1c3-104">Properties</span></span>

| <span data-ttu-id="3c1c3-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c1c3-105">Property</span></span>          | <span data-ttu-id="3c1c3-106">Тип</span><span class="sxs-lookup"><span data-stu-id="3c1c3-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3c1c3-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="3c1c3-107">reportRefreshDate</span></span> | <span data-ttu-id="3c1c3-108">Дата</span><span class="sxs-lookup"><span data-stu-id="3c1c3-108">Date</span></span>   |
| <span data-ttu-id="3c1c3-109">web</span><span class="sxs-lookup"><span data-stu-id="3c1c3-109">web</span></span>               | <span data-ttu-id="3c1c3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="3c1c3-110">Int64</span></span>  |
| <span data-ttu-id="3c1c3-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="3c1c3-111">windowsPhone</span></span>      | <span data-ttu-id="3c1c3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3c1c3-112">Int64</span></span>  |
| <span data-ttu-id="3c1c3-113">Андроидфоне</span><span class="sxs-lookup"><span data-stu-id="3c1c3-113">androidPhone</span></span>      | <span data-ttu-id="3c1c3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3c1c3-114">Int64</span></span>  |
| <span data-ttu-id="3c1c3-115">модуле</span><span class="sxs-lookup"><span data-stu-id="3c1c3-115">ios</span></span>               | <span data-ttu-id="3c1c3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3c1c3-116">Int64</span></span>  |
| <span data-ttu-id="3c1c3-117">mac</span><span class="sxs-lookup"><span data-stu-id="3c1c3-117">mac</span></span>               | <span data-ttu-id="3c1c3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3c1c3-118">Int64</span></span>  |
| <span data-ttu-id="3c1c3-119">под</span><span class="sxs-lookup"><span data-stu-id="3c1c3-119">windows</span></span>           | <span data-ttu-id="3c1c3-120">Int64</span><span class="sxs-lookup"><span data-stu-id="3c1c3-120">Int64</span></span>  |
| <span data-ttu-id="3c1c3-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="3c1c3-121">reportDate</span></span>        | <span data-ttu-id="3c1c3-122">Дата</span><span class="sxs-lookup"><span data-stu-id="3c1c3-122">Date</span></span>   |
| <span data-ttu-id="3c1c3-123">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="3c1c3-123">reportPeriod</span></span>      | <span data-ttu-id="3c1c3-124">String</span><span class="sxs-lookup"><span data-stu-id="3c1c3-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3c1c3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c1c3-125">JSON representation</span></span>

<span data-ttu-id="3c1c3-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c1c3-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
