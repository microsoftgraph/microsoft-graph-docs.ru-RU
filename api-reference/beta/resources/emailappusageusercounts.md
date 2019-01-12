---
title: Тип ресурса emailAppUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7822528aacc9d6f104012d43004fbb9aabba127c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990805"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="94531-103">Тип ресурса emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="94531-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="94531-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="94531-104">Properties</span></span>

| <span data-ttu-id="94531-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="94531-105">Property</span></span>          | <span data-ttu-id="94531-106">Тип</span><span class="sxs-lookup"><span data-stu-id="94531-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="94531-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="94531-107">reportRefreshDate</span></span> | <span data-ttu-id="94531-108">Date</span><span class="sxs-lookup"><span data-stu-id="94531-108">Date</span></span>   |
| <span data-ttu-id="94531-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="94531-109">mailForMac</span></span>        | <span data-ttu-id="94531-110">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-110">Int64</span></span>  |
| <span data-ttu-id="94531-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="94531-111">outlookForMac</span></span>     | <span data-ttu-id="94531-112">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-112">Int64</span></span>  |
| <span data-ttu-id="94531-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="94531-113">outlookForWindows</span></span> | <span data-ttu-id="94531-114">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-114">Int64</span></span>  |
| <span data-ttu-id="94531-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="94531-115">outlookForMobile</span></span>  | <span data-ttu-id="94531-116">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-116">Int64</span></span>  |
| <span data-ttu-id="94531-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="94531-117">otherForMobile</span></span>    | <span data-ttu-id="94531-118">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-118">Int64</span></span>  |
| <span data-ttu-id="94531-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="94531-119">outlookForWeb</span></span>     | <span data-ttu-id="94531-120">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-120">Int64</span></span>  |
| <span data-ttu-id="94531-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="94531-121">pop3App</span></span>           | <span data-ttu-id="94531-122">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-122">Int64</span></span>  |
| <span data-ttu-id="94531-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="94531-123">imap4App</span></span>          | <span data-ttu-id="94531-124">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-124">Int64</span></span>  |
| <span data-ttu-id="94531-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="94531-125">smtpApp</span></span>           | <span data-ttu-id="94531-126">Int64</span><span class="sxs-lookup"><span data-stu-id="94531-126">Int64</span></span>  |
| <span data-ttu-id="94531-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="94531-127">reportDate</span></span>        | <span data-ttu-id="94531-128">Date</span><span class="sxs-lookup"><span data-stu-id="94531-128">Date</span></span>   |
| <span data-ttu-id="94531-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="94531-129">reportPeriod</span></span>      | <span data-ttu-id="94531-130">String</span><span class="sxs-lookup"><span data-stu-id="94531-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94531-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94531-131">JSON representation</span></span>

<span data-ttu-id="94531-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94531-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
