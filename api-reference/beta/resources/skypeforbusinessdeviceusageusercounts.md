---
title: Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: e568e2bc396c5b7299441f8f8c513afcdada5c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997538"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="259fb-103">Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="259fb-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="259fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="259fb-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="259fb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="259fb-105">Properties</span></span>

| <span data-ttu-id="259fb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="259fb-106">Property</span></span>          | <span data-ttu-id="259fb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="259fb-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="259fb-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="259fb-108">reportRefreshDate</span></span> | <span data-ttu-id="259fb-109">Дата</span><span class="sxs-lookup"><span data-stu-id="259fb-109">Date</span></span>   |
| <span data-ttu-id="259fb-110">под</span><span class="sxs-lookup"><span data-stu-id="259fb-110">windows</span></span>           | <span data-ttu-id="259fb-111">Int64</span><span class="sxs-lookup"><span data-stu-id="259fb-111">Int64</span></span>  |
| <span data-ttu-id="259fb-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="259fb-112">windowsPhone</span></span>      | <span data-ttu-id="259fb-113">Int64</span><span class="sxs-lookup"><span data-stu-id="259fb-113">Int64</span></span>  |
| <span data-ttu-id="259fb-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="259fb-114">androidPhone</span></span>      | <span data-ttu-id="259fb-115">Int64</span><span class="sxs-lookup"><span data-stu-id="259fb-115">Int64</span></span>  |
| <span data-ttu-id="259fb-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="259fb-116">iPhone</span></span>            | <span data-ttu-id="259fb-117">Int64</span><span class="sxs-lookup"><span data-stu-id="259fb-117">Int64</span></span>  |
| <span data-ttu-id="259fb-118">iPad</span><span class="sxs-lookup"><span data-stu-id="259fb-118">iPad</span></span>              | <span data-ttu-id="259fb-119">Int64</span><span class="sxs-lookup"><span data-stu-id="259fb-119">Int64</span></span>  |
| <span data-ttu-id="259fb-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="259fb-120">reportDate</span></span>        | <span data-ttu-id="259fb-121">Дата</span><span class="sxs-lookup"><span data-stu-id="259fb-121">Date</span></span>   |
| <span data-ttu-id="259fb-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="259fb-122">reportPeriod</span></span>      | <span data-ttu-id="259fb-123">String</span><span class="sxs-lookup"><span data-stu-id="259fb-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="259fb-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="259fb-124">JSON representation</span></span>

<span data-ttu-id="259fb-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="259fb-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "windows": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


