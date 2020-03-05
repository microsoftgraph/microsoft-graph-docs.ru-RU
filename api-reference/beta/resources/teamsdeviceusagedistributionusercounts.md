---
title: Тип ресурса Теамсдевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c6b10af0e4b32c37a5fe365dc8deedae63efc8c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519878"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="d4409-103">Тип ресурса Теамсдевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="d4409-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="d4409-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4409-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d4409-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4409-105">Properties</span></span>

| <span data-ttu-id="d4409-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4409-106">Property</span></span>          | <span data-ttu-id="d4409-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d4409-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d4409-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="d4409-108">reportRefreshDate</span></span> | <span data-ttu-id="d4409-109">Дата</span><span class="sxs-lookup"><span data-stu-id="d4409-109">Date</span></span>   |
| <span data-ttu-id="d4409-110">web</span><span class="sxs-lookup"><span data-stu-id="d4409-110">web</span></span>               | <span data-ttu-id="d4409-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d4409-111">Int64</span></span>  |
| <span data-ttu-id="d4409-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="d4409-112">windowsPhone</span></span>      | <span data-ttu-id="d4409-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d4409-113">Int64</span></span>  |
| <span data-ttu-id="d4409-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="d4409-114">androidPhone</span></span>      | <span data-ttu-id="d4409-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d4409-115">Int64</span></span>  |
| <span data-ttu-id="d4409-116">модуле</span><span class="sxs-lookup"><span data-stu-id="d4409-116">ios</span></span>               | <span data-ttu-id="d4409-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d4409-117">Int64</span></span>  |
| <span data-ttu-id="d4409-118">mac</span><span class="sxs-lookup"><span data-stu-id="d4409-118">mac</span></span>               | <span data-ttu-id="d4409-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d4409-119">Int64</span></span>  |
| <span data-ttu-id="d4409-120">под</span><span class="sxs-lookup"><span data-stu-id="d4409-120">windows</span></span>           | <span data-ttu-id="d4409-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d4409-121">Int64</span></span>  |
| <span data-ttu-id="d4409-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="d4409-122">reportPeriod</span></span>      | <span data-ttu-id="d4409-123">String</span><span class="sxs-lookup"><span data-stu-id="d4409-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4409-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4409-124">JSON representation</span></span>

<span data-ttu-id="d4409-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4409-125">The following is a JSON representation of the resource.</span></span>

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
