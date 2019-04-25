---
title: Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: d98590e83637e45d35f135c56f2c0b8ff7d282bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583503"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="77c78-103">Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="77c78-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="77c78-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="77c78-104">Properties</span></span>

| <span data-ttu-id="77c78-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="77c78-105">Property</span></span>          | <span data-ttu-id="77c78-106">Тип</span><span class="sxs-lookup"><span data-stu-id="77c78-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="77c78-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="77c78-107">reportRefreshDate</span></span> | <span data-ttu-id="77c78-108">Дата</span><span class="sxs-lookup"><span data-stu-id="77c78-108">Date</span></span>   |
| <span data-ttu-id="77c78-109">под</span><span class="sxs-lookup"><span data-stu-id="77c78-109">windows</span></span>           | <span data-ttu-id="77c78-110">Int64</span><span class="sxs-lookup"><span data-stu-id="77c78-110">Int64</span></span>  |
| <span data-ttu-id="77c78-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="77c78-111">windowsPhone</span></span>      | <span data-ttu-id="77c78-112">Int64</span><span class="sxs-lookup"><span data-stu-id="77c78-112">Int64</span></span>  |
| <span data-ttu-id="77c78-113">Андроидфоне</span><span class="sxs-lookup"><span data-stu-id="77c78-113">androidPhone</span></span>      | <span data-ttu-id="77c78-114">Int64</span><span class="sxs-lookup"><span data-stu-id="77c78-114">Int64</span></span>  |
| <span data-ttu-id="77c78-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="77c78-115">iPhone</span></span>            | <span data-ttu-id="77c78-116">Int64</span><span class="sxs-lookup"><span data-stu-id="77c78-116">Int64</span></span>  |
| <span data-ttu-id="77c78-117">iPad</span><span class="sxs-lookup"><span data-stu-id="77c78-117">iPad</span></span>              | <span data-ttu-id="77c78-118">Int64</span><span class="sxs-lookup"><span data-stu-id="77c78-118">Int64</span></span>  |
| <span data-ttu-id="77c78-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="77c78-119">reportDate</span></span>        | <span data-ttu-id="77c78-120">Дата</span><span class="sxs-lookup"><span data-stu-id="77c78-120">Date</span></span>   |
| <span data-ttu-id="77c78-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="77c78-121">reportPeriod</span></span>      | <span data-ttu-id="77c78-122">String</span><span class="sxs-lookup"><span data-stu-id="77c78-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77c78-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77c78-123">JSON representation</span></span>

<span data-ttu-id="77c78-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77c78-124">The following is a JSON representation of the resource.</span></span>

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
