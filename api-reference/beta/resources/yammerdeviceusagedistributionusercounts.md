---
title: Тип ресурса Яммердевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1797facecb5047badb35c0a4d876680e817cc643
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555082"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="411bd-103">Тип ресурса Яммердевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="411bd-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="411bd-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="411bd-104">Properties</span></span>

| <span data-ttu-id="411bd-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="411bd-105">Property</span></span>          | <span data-ttu-id="411bd-106">Тип</span><span class="sxs-lookup"><span data-stu-id="411bd-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="411bd-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="411bd-107">reportRefreshDate</span></span> | <span data-ttu-id="411bd-108">Дата</span><span class="sxs-lookup"><span data-stu-id="411bd-108">Date</span></span>   |
| <span data-ttu-id="411bd-109">web</span><span class="sxs-lookup"><span data-stu-id="411bd-109">web</span></span>               | <span data-ttu-id="411bd-110">Int32</span><span class="sxs-lookup"><span data-stu-id="411bd-110">Int32</span></span>  |
| <span data-ttu-id="411bd-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="411bd-111">windowsPhone</span></span>      | <span data-ttu-id="411bd-112">Int32</span><span class="sxs-lookup"><span data-stu-id="411bd-112">Int32</span></span>  |
| <span data-ttu-id="411bd-113">Андроидфоне</span><span class="sxs-lookup"><span data-stu-id="411bd-113">androidPhone</span></span>      | <span data-ttu-id="411bd-114">Int32</span><span class="sxs-lookup"><span data-stu-id="411bd-114">Int32</span></span>  |
| <span data-ttu-id="411bd-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="411bd-115">iPhone</span></span>            | <span data-ttu-id="411bd-116">Int32</span><span class="sxs-lookup"><span data-stu-id="411bd-116">Int32</span></span>  |
| <span data-ttu-id="411bd-117">iPad</span><span class="sxs-lookup"><span data-stu-id="411bd-117">iPad</span></span>              | <span data-ttu-id="411bd-118">Int32</span><span class="sxs-lookup"><span data-stu-id="411bd-118">Int32</span></span>  |
| <span data-ttu-id="411bd-119">остальные</span><span class="sxs-lookup"><span data-stu-id="411bd-119">other</span></span>             | <span data-ttu-id="411bd-120">Int32</span><span class="sxs-lookup"><span data-stu-id="411bd-120">Int32</span></span>  |
| <span data-ttu-id="411bd-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="411bd-121">reportPeriod</span></span>      | <span data-ttu-id="411bd-122">String</span><span class="sxs-lookup"><span data-stu-id="411bd-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="411bd-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="411bd-123">JSON representation</span></span>

<span data-ttu-id="411bd-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="411bd-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportPeriod": "String"
}
```
