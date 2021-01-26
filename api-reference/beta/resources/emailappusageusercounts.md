---
title: Тип ресурса emailAppUsageUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5630b239f9fb8d887e857993268a45c9d0e0d3b4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981839"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="b75ce-103">Тип ресурса emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="b75ce-103">emailAppUsageUserCounts resource type</span></span>

<span data-ttu-id="b75ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b75ce-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b75ce-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b75ce-105">Properties</span></span>

| <span data-ttu-id="b75ce-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b75ce-106">Property</span></span>          | <span data-ttu-id="b75ce-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b75ce-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b75ce-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b75ce-108">reportRefreshDate</span></span> | <span data-ttu-id="b75ce-109">Дата</span><span class="sxs-lookup"><span data-stu-id="b75ce-109">Date</span></span>   |
| <span data-ttu-id="b75ce-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="b75ce-110">mailForMac</span></span>        | <span data-ttu-id="b75ce-111">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-111">Int64</span></span>  |
| <span data-ttu-id="b75ce-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="b75ce-112">outlookForMac</span></span>     | <span data-ttu-id="b75ce-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-113">Int64</span></span>  |
| <span data-ttu-id="b75ce-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="b75ce-114">outlookForWindows</span></span> | <span data-ttu-id="b75ce-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-115">Int64</span></span>  |
| <span data-ttu-id="b75ce-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="b75ce-116">outlookForMobile</span></span>  | <span data-ttu-id="b75ce-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-117">Int64</span></span>  |
| <span data-ttu-id="b75ce-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="b75ce-118">otherForMobile</span></span>    | <span data-ttu-id="b75ce-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-119">Int64</span></span>  |
| <span data-ttu-id="b75ce-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="b75ce-120">outlookForWeb</span></span>     | <span data-ttu-id="b75ce-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-121">Int64</span></span>  |
| <span data-ttu-id="b75ce-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="b75ce-122">pop3App</span></span>           | <span data-ttu-id="b75ce-123">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-123">Int64</span></span>  |
| <span data-ttu-id="b75ce-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="b75ce-124">imap4App</span></span>          | <span data-ttu-id="b75ce-125">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-125">Int64</span></span>  |
| <span data-ttu-id="b75ce-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="b75ce-126">smtpApp</span></span>           | <span data-ttu-id="b75ce-127">Int64</span><span class="sxs-lookup"><span data-stu-id="b75ce-127">Int64</span></span>  |
| <span data-ttu-id="b75ce-128">reportDate</span><span class="sxs-lookup"><span data-stu-id="b75ce-128">reportDate</span></span>        | <span data-ttu-id="b75ce-129">Дата</span><span class="sxs-lookup"><span data-stu-id="b75ce-129">Date</span></span>   |
| <span data-ttu-id="b75ce-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b75ce-130">reportPeriod</span></span>      | <span data-ttu-id="b75ce-131">String</span><span class="sxs-lookup"><span data-stu-id="b75ce-131">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b75ce-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b75ce-132">JSON representation</span></span>

<span data-ttu-id="b75ce-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b75ce-133">The following is a JSON representation of the resource.</span></span>

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


