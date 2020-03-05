---
title: Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5a5149b3a247d4245f95d05f5e3f6b3e4be59e3d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520501"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="04a84-103">Тип ресурса Скипефорбусинессдевицеусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="04a84-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="04a84-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04a84-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="04a84-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="04a84-105">Properties</span></span>

| <span data-ttu-id="04a84-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="04a84-106">Property</span></span>          | <span data-ttu-id="04a84-107">Тип</span><span class="sxs-lookup"><span data-stu-id="04a84-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="04a84-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="04a84-108">reportRefreshDate</span></span> | <span data-ttu-id="04a84-109">Дата</span><span class="sxs-lookup"><span data-stu-id="04a84-109">Date</span></span>   |
| <span data-ttu-id="04a84-110">под</span><span class="sxs-lookup"><span data-stu-id="04a84-110">windows</span></span>           | <span data-ttu-id="04a84-111">Int64</span><span class="sxs-lookup"><span data-stu-id="04a84-111">Int64</span></span>  |
| <span data-ttu-id="04a84-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="04a84-112">windowsPhone</span></span>      | <span data-ttu-id="04a84-113">Int64</span><span class="sxs-lookup"><span data-stu-id="04a84-113">Int64</span></span>  |
| <span data-ttu-id="04a84-114">андроидфоне</span><span class="sxs-lookup"><span data-stu-id="04a84-114">androidPhone</span></span>      | <span data-ttu-id="04a84-115">Int64</span><span class="sxs-lookup"><span data-stu-id="04a84-115">Int64</span></span>  |
| <span data-ttu-id="04a84-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="04a84-116">iPhone</span></span>            | <span data-ttu-id="04a84-117">Int64</span><span class="sxs-lookup"><span data-stu-id="04a84-117">Int64</span></span>  |
| <span data-ttu-id="04a84-118">iPad</span><span class="sxs-lookup"><span data-stu-id="04a84-118">iPad</span></span>              | <span data-ttu-id="04a84-119">Int64</span><span class="sxs-lookup"><span data-stu-id="04a84-119">Int64</span></span>  |
| <span data-ttu-id="04a84-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="04a84-120">reportDate</span></span>        | <span data-ttu-id="04a84-121">Дата</span><span class="sxs-lookup"><span data-stu-id="04a84-121">Date</span></span>   |
| <span data-ttu-id="04a84-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="04a84-122">reportPeriod</span></span>      | <span data-ttu-id="04a84-123">String</span><span class="sxs-lookup"><span data-stu-id="04a84-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="04a84-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04a84-124">JSON representation</span></span>

<span data-ttu-id="04a84-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04a84-125">The following is a JSON representation of the resource.</span></span>

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
