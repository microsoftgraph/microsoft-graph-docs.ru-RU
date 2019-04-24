---
title: Тип ресурса Емаилаппусажеверсионсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 371352c42e870f45224999b7a618d1bb694ea512
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506680"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="d97ef-103">Тип ресурса Емаилаппусажеверсионсусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="d97ef-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d97ef-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d97ef-104">Properties</span></span>

| <span data-ttu-id="d97ef-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d97ef-105">Property</span></span>          | <span data-ttu-id="d97ef-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d97ef-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d97ef-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="d97ef-107">reportRefreshDate</span></span> | <span data-ttu-id="d97ef-108">Дата</span><span class="sxs-lookup"><span data-stu-id="d97ef-108">Date</span></span>   |
| <span data-ttu-id="d97ef-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="d97ef-109">outlook2016</span></span>       | <span data-ttu-id="d97ef-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d97ef-110">Int64</span></span>  |
| <span data-ttu-id="d97ef-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="d97ef-111">outlook2013</span></span>       | <span data-ttu-id="d97ef-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d97ef-112">Int64</span></span>  |
| <span data-ttu-id="d97ef-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="d97ef-113">outlook2010</span></span>       | <span data-ttu-id="d97ef-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d97ef-114">Int64</span></span>  |
| <span data-ttu-id="d97ef-115">Outlook2007</span><span class="sxs-lookup"><span data-stu-id="d97ef-115">outlook2007</span></span>       | <span data-ttu-id="d97ef-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d97ef-116">Int64</span></span>  |
| <span data-ttu-id="d97ef-117">определено</span><span class="sxs-lookup"><span data-stu-id="d97ef-117">undetermined</span></span>      | <span data-ttu-id="d97ef-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d97ef-118">Int64</span></span>  |
| <span data-ttu-id="d97ef-119">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="d97ef-119">reportPeriod</span></span>      | <span data-ttu-id="d97ef-120">String</span><span class="sxs-lookup"><span data-stu-id="d97ef-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d97ef-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d97ef-121">JSON representation</span></span>

<span data-ttu-id="d97ef-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d97ef-122">The following is a JSON representation of the resource.</span></span>

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
