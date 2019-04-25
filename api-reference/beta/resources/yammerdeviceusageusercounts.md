---
title: Тип ресурса Яммердевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 63bd3e150e822d3c356f4409c2920e4998e53ec2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551521"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="f4492-103">Тип ресурса Яммердевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="f4492-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f4492-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4492-104">Properties</span></span>

| <span data-ttu-id="f4492-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4492-105">Property</span></span>          | <span data-ttu-id="f4492-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f4492-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f4492-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="f4492-107">reportRefreshDate</span></span> | <span data-ttu-id="f4492-108">Дата</span><span class="sxs-lookup"><span data-stu-id="f4492-108">Date</span></span>   |
| <span data-ttu-id="f4492-109">web</span><span class="sxs-lookup"><span data-stu-id="f4492-109">web</span></span>               | <span data-ttu-id="f4492-110">Int32</span><span class="sxs-lookup"><span data-stu-id="f4492-110">Int32</span></span>  |
| <span data-ttu-id="f4492-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="f4492-111">windowsPhone</span></span>      | <span data-ttu-id="f4492-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f4492-112">Int32</span></span>  |
| <span data-ttu-id="f4492-113">Андроидфоне</span><span class="sxs-lookup"><span data-stu-id="f4492-113">androidPhone</span></span>      | <span data-ttu-id="f4492-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f4492-114">Int32</span></span>  |
| <span data-ttu-id="f4492-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="f4492-115">iPhone</span></span>            | <span data-ttu-id="f4492-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f4492-116">Int32</span></span>  |
| <span data-ttu-id="f4492-117">iPad</span><span class="sxs-lookup"><span data-stu-id="f4492-117">iPad</span></span>              | <span data-ttu-id="f4492-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f4492-118">Int32</span></span>  |
| <span data-ttu-id="f4492-119">остальные</span><span class="sxs-lookup"><span data-stu-id="f4492-119">other</span></span>             | <span data-ttu-id="f4492-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f4492-120">Int32</span></span>  |
| <span data-ttu-id="f4492-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="f4492-121">reportDate</span></span>        | <span data-ttu-id="f4492-122">Дата</span><span class="sxs-lookup"><span data-stu-id="f4492-122">Date</span></span>   |
| <span data-ttu-id="f4492-123">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="f4492-123">reportPeriod</span></span>      | <span data-ttu-id="f4492-124">String</span><span class="sxs-lookup"><span data-stu-id="f4492-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4492-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f4492-125">JSON representation</span></span>

<span data-ttu-id="f4492-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4492-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
