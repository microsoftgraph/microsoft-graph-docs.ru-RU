---
title: Тип ресурса Теамсдевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: af62b0bf6d11c256252b2c6c6f16f4e3b5ba2354
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046470"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="b2228-103">Тип ресурса Теамсдевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="b2228-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="b2228-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2228-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b2228-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2228-105">Properties</span></span>

| <span data-ttu-id="b2228-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2228-106">Property</span></span>          | <span data-ttu-id="b2228-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b2228-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b2228-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="b2228-108">reportRefreshDate</span></span> | <span data-ttu-id="b2228-109">Дата</span><span class="sxs-lookup"><span data-stu-id="b2228-109">Date</span></span>   |
| <span data-ttu-id="b2228-110">web</span><span class="sxs-lookup"><span data-stu-id="b2228-110">web</span></span>               | <span data-ttu-id="b2228-111">Int64</span><span class="sxs-lookup"><span data-stu-id="b2228-111">Int64</span></span>  |
| <span data-ttu-id="b2228-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="b2228-112">windowsPhone</span></span>      | <span data-ttu-id="b2228-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b2228-113">Int64</span></span>  |
| <span data-ttu-id="b2228-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="b2228-114">androidPhone</span></span>      | <span data-ttu-id="b2228-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b2228-115">Int64</span></span>  |
| <span data-ttu-id="b2228-116">модуле</span><span class="sxs-lookup"><span data-stu-id="b2228-116">ios</span></span>               | <span data-ttu-id="b2228-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b2228-117">Int64</span></span>  |
| <span data-ttu-id="b2228-118">mac</span><span class="sxs-lookup"><span data-stu-id="b2228-118">mac</span></span>               | <span data-ttu-id="b2228-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b2228-119">Int64</span></span>  |
| <span data-ttu-id="b2228-120">под</span><span class="sxs-lookup"><span data-stu-id="b2228-120">windows</span></span>           | <span data-ttu-id="b2228-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b2228-121">Int64</span></span>  |
| <span data-ttu-id="b2228-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="b2228-122">reportDate</span></span>        | <span data-ttu-id="b2228-123">Дата</span><span class="sxs-lookup"><span data-stu-id="b2228-123">Date</span></span>   |
| <span data-ttu-id="b2228-124">репортпериод</span><span class="sxs-lookup"><span data-stu-id="b2228-124">reportPeriod</span></span>      | <span data-ttu-id="b2228-125">Строка</span><span class="sxs-lookup"><span data-stu-id="b2228-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2228-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2228-126">JSON representation</span></span>

<span data-ttu-id="b2228-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2228-127">The following is a JSON representation of the resource.</span></span>

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


