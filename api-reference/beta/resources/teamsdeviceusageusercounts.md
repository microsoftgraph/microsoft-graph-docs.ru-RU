---
title: Тип ресурса Теамсдевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 02dc1b734e039e7c5eac7b8ffaed7a418e443c71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519871"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="b484e-103">Тип ресурса Теамсдевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="b484e-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="b484e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b484e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b484e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b484e-105">Properties</span></span>

| <span data-ttu-id="b484e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b484e-106">Property</span></span>          | <span data-ttu-id="b484e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b484e-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b484e-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="b484e-108">reportRefreshDate</span></span> | <span data-ttu-id="b484e-109">Дата</span><span class="sxs-lookup"><span data-stu-id="b484e-109">Date</span></span>   |
| <span data-ttu-id="b484e-110">web</span><span class="sxs-lookup"><span data-stu-id="b484e-110">web</span></span>               | <span data-ttu-id="b484e-111">Int64</span><span class="sxs-lookup"><span data-stu-id="b484e-111">Int64</span></span>  |
| <span data-ttu-id="b484e-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="b484e-112">windowsPhone</span></span>      | <span data-ttu-id="b484e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b484e-113">Int64</span></span>  |
| <span data-ttu-id="b484e-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="b484e-114">androidPhone</span></span>      | <span data-ttu-id="b484e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b484e-115">Int64</span></span>  |
| <span data-ttu-id="b484e-116">модуле</span><span class="sxs-lookup"><span data-stu-id="b484e-116">ios</span></span>               | <span data-ttu-id="b484e-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b484e-117">Int64</span></span>  |
| <span data-ttu-id="b484e-118">mac</span><span class="sxs-lookup"><span data-stu-id="b484e-118">mac</span></span>               | <span data-ttu-id="b484e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b484e-119">Int64</span></span>  |
| <span data-ttu-id="b484e-120">под</span><span class="sxs-lookup"><span data-stu-id="b484e-120">windows</span></span>           | <span data-ttu-id="b484e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b484e-121">Int64</span></span>  |
| <span data-ttu-id="b484e-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="b484e-122">reportDate</span></span>        | <span data-ttu-id="b484e-123">Дата</span><span class="sxs-lookup"><span data-stu-id="b484e-123">Date</span></span>   |
| <span data-ttu-id="b484e-124">репортпериод</span><span class="sxs-lookup"><span data-stu-id="b484e-124">reportPeriod</span></span>      | <span data-ttu-id="b484e-125">String</span><span class="sxs-lookup"><span data-stu-id="b484e-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b484e-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b484e-126">JSON representation</span></span>

<span data-ttu-id="b484e-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b484e-127">The following is a JSON representation of the resource.</span></span>

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
