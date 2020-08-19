---
title: Тип ресурса Скипефорбусинессдевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: c0134bedc15de07d89709a623b6a31a8f53ac5fe
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808615"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="e850e-103">Тип ресурса Скипефорбусинессдевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="e850e-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="e850e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e850e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e850e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e850e-105">Properties</span></span>

| <span data-ttu-id="e850e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e850e-106">Property</span></span>          | <span data-ttu-id="e850e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e850e-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e850e-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="e850e-108">reportRefreshDate</span></span> | <span data-ttu-id="e850e-109">Дата</span><span class="sxs-lookup"><span data-stu-id="e850e-109">Date</span></span>   |
| <span data-ttu-id="e850e-110">под</span><span class="sxs-lookup"><span data-stu-id="e850e-110">windows</span></span>           | <span data-ttu-id="e850e-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e850e-111">Int64</span></span>  |
| <span data-ttu-id="e850e-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="e850e-112">windowsPhone</span></span>      | <span data-ttu-id="e850e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e850e-113">Int64</span></span>  |
| <span data-ttu-id="e850e-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="e850e-114">androidPhone</span></span>      | <span data-ttu-id="e850e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e850e-115">Int64</span></span>  |
| <span data-ttu-id="e850e-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="e850e-116">iPhone</span></span>            | <span data-ttu-id="e850e-117">Int64</span><span class="sxs-lookup"><span data-stu-id="e850e-117">Int64</span></span>  |
| <span data-ttu-id="e850e-118">iPad</span><span class="sxs-lookup"><span data-stu-id="e850e-118">iPad</span></span>              | <span data-ttu-id="e850e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e850e-119">Int64</span></span>  |
| <span data-ttu-id="e850e-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="e850e-120">reportPeriod</span></span>      | <span data-ttu-id="e850e-121">String</span><span class="sxs-lookup"><span data-stu-id="e850e-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e850e-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e850e-122">JSON representation</span></span>

<span data-ttu-id="e850e-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e850e-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "windows": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "reportPeriod": "String"
}
```
