---
title: Тип ресурса Теамсдевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d398782cef79cdf92bc56502f7c6cbf1bcdee99d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553612"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="18587-103">Тип ресурса Теамсдевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="18587-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="18587-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="18587-104">Properties</span></span>

| <span data-ttu-id="18587-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="18587-105">Property</span></span>          | <span data-ttu-id="18587-106">Тип</span><span class="sxs-lookup"><span data-stu-id="18587-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="18587-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="18587-107">reportRefreshDate</span></span> | <span data-ttu-id="18587-108">Дата</span><span class="sxs-lookup"><span data-stu-id="18587-108">Date</span></span>   |
| <span data-ttu-id="18587-109">web</span><span class="sxs-lookup"><span data-stu-id="18587-109">web</span></span>               | <span data-ttu-id="18587-110">Int64</span><span class="sxs-lookup"><span data-stu-id="18587-110">Int64</span></span>  |
| <span data-ttu-id="18587-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="18587-111">windowsPhone</span></span>      | <span data-ttu-id="18587-112">Int64</span><span class="sxs-lookup"><span data-stu-id="18587-112">Int64</span></span>  |
| <span data-ttu-id="18587-113">Андроидфоне</span><span class="sxs-lookup"><span data-stu-id="18587-113">androidPhone</span></span>      | <span data-ttu-id="18587-114">Int64</span><span class="sxs-lookup"><span data-stu-id="18587-114">Int64</span></span>  |
| <span data-ttu-id="18587-115">модуле</span><span class="sxs-lookup"><span data-stu-id="18587-115">ios</span></span>               | <span data-ttu-id="18587-116">Int64</span><span class="sxs-lookup"><span data-stu-id="18587-116">Int64</span></span>  |
| <span data-ttu-id="18587-117">mac</span><span class="sxs-lookup"><span data-stu-id="18587-117">mac</span></span>               | <span data-ttu-id="18587-118">Int64</span><span class="sxs-lookup"><span data-stu-id="18587-118">Int64</span></span>  |
| <span data-ttu-id="18587-119">под</span><span class="sxs-lookup"><span data-stu-id="18587-119">windows</span></span>           | <span data-ttu-id="18587-120">Int64</span><span class="sxs-lookup"><span data-stu-id="18587-120">Int64</span></span>  |
| <span data-ttu-id="18587-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="18587-121">reportPeriod</span></span>      | <span data-ttu-id="18587-122">String</span><span class="sxs-lookup"><span data-stu-id="18587-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18587-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="18587-123">JSON representation</span></span>

<span data-ttu-id="18587-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18587-124">The following is a JSON representation of the resource.</span></span>

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
