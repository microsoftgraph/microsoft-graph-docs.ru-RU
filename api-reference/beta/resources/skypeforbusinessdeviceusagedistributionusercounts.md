---
title: Тип ресурса Скипефорбусинессдевицеусажедистрибутионусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d7b6639b810507d7bee0c0a54f98cefae8d51677
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520424"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="5739a-103">Тип ресурса Скипефорбусинессдевицеусажедистрибутионусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="5739a-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="5739a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5739a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5739a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5739a-105">Properties</span></span>

| <span data-ttu-id="5739a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5739a-106">Property</span></span>          | <span data-ttu-id="5739a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5739a-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5739a-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="5739a-108">reportRefreshDate</span></span> | <span data-ttu-id="5739a-109">Дата</span><span class="sxs-lookup"><span data-stu-id="5739a-109">Date</span></span>   |
| <span data-ttu-id="5739a-110">под</span><span class="sxs-lookup"><span data-stu-id="5739a-110">windows</span></span>           | <span data-ttu-id="5739a-111">Int64</span><span class="sxs-lookup"><span data-stu-id="5739a-111">Int64</span></span>  |
| <span data-ttu-id="5739a-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5739a-112">windowsPhone</span></span>      | <span data-ttu-id="5739a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5739a-113">Int64</span></span>  |
| <span data-ttu-id="5739a-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="5739a-114">androidPhone</span></span>      | <span data-ttu-id="5739a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5739a-115">Int64</span></span>  |
| <span data-ttu-id="5739a-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="5739a-116">iPhone</span></span>            | <span data-ttu-id="5739a-117">Int64</span><span class="sxs-lookup"><span data-stu-id="5739a-117">Int64</span></span>  |
| <span data-ttu-id="5739a-118">iPad</span><span class="sxs-lookup"><span data-stu-id="5739a-118">iPad</span></span>              | <span data-ttu-id="5739a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5739a-119">Int64</span></span>  |
| <span data-ttu-id="5739a-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="5739a-120">reportPeriod</span></span>      | <span data-ttu-id="5739a-121">String</span><span class="sxs-lookup"><span data-stu-id="5739a-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5739a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5739a-122">JSON representation</span></span>

<span data-ttu-id="5739a-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5739a-123">The following is a JSON representation of the resource.</span></span>

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
