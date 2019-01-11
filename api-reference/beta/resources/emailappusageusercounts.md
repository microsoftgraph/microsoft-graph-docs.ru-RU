---
title: Тип ресурса emailAppUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: a018776f092e9b7f378e8069666d015e1cd3e4a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835450"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="48c70-103">Тип ресурса emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="48c70-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="48c70-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="48c70-104">Properties</span></span>

| <span data-ttu-id="48c70-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="48c70-105">Property</span></span>          | <span data-ttu-id="48c70-106">Тип</span><span class="sxs-lookup"><span data-stu-id="48c70-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="48c70-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="48c70-107">reportRefreshDate</span></span> | <span data-ttu-id="48c70-108">Date</span><span class="sxs-lookup"><span data-stu-id="48c70-108">Date</span></span>   |
| <span data-ttu-id="48c70-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="48c70-109">mailForMac</span></span>        | <span data-ttu-id="48c70-110">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-110">Int64</span></span>  |
| <span data-ttu-id="48c70-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="48c70-111">outlookForMac</span></span>     | <span data-ttu-id="48c70-112">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-112">Int64</span></span>  |
| <span data-ttu-id="48c70-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="48c70-113">outlookForWindows</span></span> | <span data-ttu-id="48c70-114">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-114">Int64</span></span>  |
| <span data-ttu-id="48c70-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="48c70-115">outlookForMobile</span></span>  | <span data-ttu-id="48c70-116">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-116">Int64</span></span>  |
| <span data-ttu-id="48c70-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="48c70-117">otherForMobile</span></span>    | <span data-ttu-id="48c70-118">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-118">Int64</span></span>  |
| <span data-ttu-id="48c70-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="48c70-119">outlookForWeb</span></span>     | <span data-ttu-id="48c70-120">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-120">Int64</span></span>  |
| <span data-ttu-id="48c70-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="48c70-121">pop3App</span></span>           | <span data-ttu-id="48c70-122">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-122">Int64</span></span>  |
| <span data-ttu-id="48c70-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="48c70-123">imap4App</span></span>          | <span data-ttu-id="48c70-124">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-124">Int64</span></span>  |
| <span data-ttu-id="48c70-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="48c70-125">smtpApp</span></span>           | <span data-ttu-id="48c70-126">Int64</span><span class="sxs-lookup"><span data-stu-id="48c70-126">Int64</span></span>  |
| <span data-ttu-id="48c70-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="48c70-127">reportDate</span></span>        | <span data-ttu-id="48c70-128">Date</span><span class="sxs-lookup"><span data-stu-id="48c70-128">Date</span></span>   |
| <span data-ttu-id="48c70-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="48c70-129">reportPeriod</span></span>      | <span data-ttu-id="48c70-130">String</span><span class="sxs-lookup"><span data-stu-id="48c70-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48c70-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48c70-131">JSON representation</span></span>

<span data-ttu-id="48c70-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48c70-132">The following is a JSON representation of the resource.</span></span>

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
