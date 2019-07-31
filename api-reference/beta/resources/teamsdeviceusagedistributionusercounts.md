---
title: Тип ресурса Теамсдевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1842d2edc9e527d577b6a44e61443018f8309c17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007615"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="c2b48-103">Тип ресурса Теамсдевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="c2b48-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c2b48-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2b48-104">Properties</span></span>

| <span data-ttu-id="c2b48-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2b48-105">Property</span></span>          | <span data-ttu-id="c2b48-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c2b48-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c2b48-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c2b48-107">reportRefreshDate</span></span> | <span data-ttu-id="c2b48-108">Дата</span><span class="sxs-lookup"><span data-stu-id="c2b48-108">Date</span></span>   |
| <span data-ttu-id="c2b48-109">web</span><span class="sxs-lookup"><span data-stu-id="c2b48-109">web</span></span>               | <span data-ttu-id="c2b48-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c2b48-110">Int64</span></span>  |
| <span data-ttu-id="c2b48-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="c2b48-111">windowsPhone</span></span>      | <span data-ttu-id="c2b48-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c2b48-112">Int64</span></span>  |
| <span data-ttu-id="c2b48-113">Андроидфоне</span><span class="sxs-lookup"><span data-stu-id="c2b48-113">androidPhone</span></span>      | <span data-ttu-id="c2b48-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c2b48-114">Int64</span></span>  |
| <span data-ttu-id="c2b48-115">модуле</span><span class="sxs-lookup"><span data-stu-id="c2b48-115">ios</span></span>               | <span data-ttu-id="c2b48-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c2b48-116">Int64</span></span>  |
| <span data-ttu-id="c2b48-117">mac</span><span class="sxs-lookup"><span data-stu-id="c2b48-117">mac</span></span>               | <span data-ttu-id="c2b48-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c2b48-118">Int64</span></span>  |
| <span data-ttu-id="c2b48-119">под</span><span class="sxs-lookup"><span data-stu-id="c2b48-119">windows</span></span>           | <span data-ttu-id="c2b48-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c2b48-120">Int64</span></span>  |
| <span data-ttu-id="c2b48-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="c2b48-121">reportPeriod</span></span>      | <span data-ttu-id="c2b48-122">String</span><span class="sxs-lookup"><span data-stu-id="c2b48-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c2b48-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2b48-123">JSON representation</span></span>

<span data-ttu-id="c2b48-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2b48-124">The following is a JSON representation of the resource.</span></span>

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
