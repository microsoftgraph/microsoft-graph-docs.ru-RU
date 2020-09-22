---
title: Тип ресурса Теамсдевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5a4a09c96c5b3691c4cbcc285ac947c903ce50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046484"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="5ca59-103">Тип ресурса Теамсдевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="5ca59-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="5ca59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca59-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5ca59-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ca59-105">Properties</span></span>

| <span data-ttu-id="5ca59-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ca59-106">Property</span></span>          | <span data-ttu-id="5ca59-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5ca59-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5ca59-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="5ca59-108">reportRefreshDate</span></span> | <span data-ttu-id="5ca59-109">Дата</span><span class="sxs-lookup"><span data-stu-id="5ca59-109">Date</span></span>   |
| <span data-ttu-id="5ca59-110">web</span><span class="sxs-lookup"><span data-stu-id="5ca59-110">web</span></span>               | <span data-ttu-id="5ca59-111">Int64</span><span class="sxs-lookup"><span data-stu-id="5ca59-111">Int64</span></span>  |
| <span data-ttu-id="5ca59-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5ca59-112">windowsPhone</span></span>      | <span data-ttu-id="5ca59-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5ca59-113">Int64</span></span>  |
| <span data-ttu-id="5ca59-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="5ca59-114">androidPhone</span></span>      | <span data-ttu-id="5ca59-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5ca59-115">Int64</span></span>  |
| <span data-ttu-id="5ca59-116">модуле</span><span class="sxs-lookup"><span data-stu-id="5ca59-116">ios</span></span>               | <span data-ttu-id="5ca59-117">Int64</span><span class="sxs-lookup"><span data-stu-id="5ca59-117">Int64</span></span>  |
| <span data-ttu-id="5ca59-118">mac</span><span class="sxs-lookup"><span data-stu-id="5ca59-118">mac</span></span>               | <span data-ttu-id="5ca59-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5ca59-119">Int64</span></span>  |
| <span data-ttu-id="5ca59-120">под</span><span class="sxs-lookup"><span data-stu-id="5ca59-120">windows</span></span>           | <span data-ttu-id="5ca59-121">Int64</span><span class="sxs-lookup"><span data-stu-id="5ca59-121">Int64</span></span>  |
| <span data-ttu-id="5ca59-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="5ca59-122">reportPeriod</span></span>      | <span data-ttu-id="5ca59-123">Строка</span><span class="sxs-lookup"><span data-stu-id="5ca59-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ca59-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ca59-124">JSON representation</span></span>

<span data-ttu-id="5ca59-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ca59-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```


