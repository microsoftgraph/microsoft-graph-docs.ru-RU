---
title: Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 01867d92037f3bf80a7db2c25cc96a967ac560cd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808713"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="c31e9-103">Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="c31e9-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="c31e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c31e9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c31e9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c31e9-105">Properties</span></span>

| <span data-ttu-id="c31e9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c31e9-106">Property</span></span>          | <span data-ttu-id="c31e9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c31e9-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c31e9-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c31e9-108">reportRefreshDate</span></span> | <span data-ttu-id="c31e9-109">Дата</span><span class="sxs-lookup"><span data-stu-id="c31e9-109">Date</span></span>   |
| <span data-ttu-id="c31e9-110">под</span><span class="sxs-lookup"><span data-stu-id="c31e9-110">windows</span></span>           | <span data-ttu-id="c31e9-111">Int64</span><span class="sxs-lookup"><span data-stu-id="c31e9-111">Int64</span></span>  |
| <span data-ttu-id="c31e9-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="c31e9-112">windowsPhone</span></span>      | <span data-ttu-id="c31e9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c31e9-113">Int64</span></span>  |
| <span data-ttu-id="c31e9-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="c31e9-114">androidPhone</span></span>      | <span data-ttu-id="c31e9-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c31e9-115">Int64</span></span>  |
| <span data-ttu-id="c31e9-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="c31e9-116">iPhone</span></span>            | <span data-ttu-id="c31e9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="c31e9-117">Int64</span></span>  |
| <span data-ttu-id="c31e9-118">iPad</span><span class="sxs-lookup"><span data-stu-id="c31e9-118">iPad</span></span>              | <span data-ttu-id="c31e9-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c31e9-119">Int64</span></span>  |
| <span data-ttu-id="c31e9-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="c31e9-120">reportDate</span></span>        | <span data-ttu-id="c31e9-121">Дата</span><span class="sxs-lookup"><span data-stu-id="c31e9-121">Date</span></span>   |
| <span data-ttu-id="c31e9-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="c31e9-122">reportPeriod</span></span>      | <span data-ttu-id="c31e9-123">String</span><span class="sxs-lookup"><span data-stu-id="c31e9-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c31e9-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c31e9-124">JSON representation</span></span>

<span data-ttu-id="c31e9-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c31e9-125">The following is a JSON representation of the resource.</span></span>

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
