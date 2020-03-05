---
title: Тип ресурса Емаилаппусажеверсионсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: edc9242a99f0a993b2fa21c95259582bdf31c3da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499416"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="24e75-103">Тип ресурса Емаилаппусажеверсионсусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="24e75-103">emailAppUsageVersionsUserCounts resource type</span></span>

<span data-ttu-id="24e75-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="24e75-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="24e75-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="24e75-105">Properties</span></span>

| <span data-ttu-id="24e75-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="24e75-106">Property</span></span>          | <span data-ttu-id="24e75-107">Тип</span><span class="sxs-lookup"><span data-stu-id="24e75-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="24e75-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="24e75-108">reportRefreshDate</span></span> | <span data-ttu-id="24e75-109">Дата</span><span class="sxs-lookup"><span data-stu-id="24e75-109">Date</span></span>   |
| <span data-ttu-id="24e75-110">outlook2016</span><span class="sxs-lookup"><span data-stu-id="24e75-110">outlook2016</span></span>       | <span data-ttu-id="24e75-111">Int64</span><span class="sxs-lookup"><span data-stu-id="24e75-111">Int64</span></span>  |
| <span data-ttu-id="24e75-112">outlook2013</span><span class="sxs-lookup"><span data-stu-id="24e75-112">outlook2013</span></span>       | <span data-ttu-id="24e75-113">Int64</span><span class="sxs-lookup"><span data-stu-id="24e75-113">Int64</span></span>  |
| <span data-ttu-id="24e75-114">outlook2010</span><span class="sxs-lookup"><span data-stu-id="24e75-114">outlook2010</span></span>       | <span data-ttu-id="24e75-115">Int64</span><span class="sxs-lookup"><span data-stu-id="24e75-115">Int64</span></span>  |
| <span data-ttu-id="24e75-116">outlook2007</span><span class="sxs-lookup"><span data-stu-id="24e75-116">outlook2007</span></span>       | <span data-ttu-id="24e75-117">Int64</span><span class="sxs-lookup"><span data-stu-id="24e75-117">Int64</span></span>  |
| <span data-ttu-id="24e75-118">определено</span><span class="sxs-lookup"><span data-stu-id="24e75-118">undetermined</span></span>      | <span data-ttu-id="24e75-119">Int64</span><span class="sxs-lookup"><span data-stu-id="24e75-119">Int64</span></span>  |
| <span data-ttu-id="24e75-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="24e75-120">reportPeriod</span></span>      | <span data-ttu-id="24e75-121">String</span><span class="sxs-lookup"><span data-stu-id="24e75-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24e75-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24e75-122">JSON representation</span></span>

<span data-ttu-id="24e75-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24e75-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
