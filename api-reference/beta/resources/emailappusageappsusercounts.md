---
title: Тип ресурса emailAppUsageAppsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970383"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="3a02a-103">Тип ресурса emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="3a02a-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3a02a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a02a-104">Properties</span></span>

| <span data-ttu-id="3a02a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a02a-105">Property</span></span>          | <span data-ttu-id="3a02a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="3a02a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3a02a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3a02a-107">reportRefreshDate</span></span> | <span data-ttu-id="3a02a-108">Date</span><span class="sxs-lookup"><span data-stu-id="3a02a-108">Date</span></span>   |
| <span data-ttu-id="3a02a-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="3a02a-109">mailForMac</span></span>        | <span data-ttu-id="3a02a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-110">Int64</span></span>  |
| <span data-ttu-id="3a02a-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="3a02a-111">outlookForMac</span></span>     | <span data-ttu-id="3a02a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-112">Int64</span></span>  |
| <span data-ttu-id="3a02a-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="3a02a-113">outlookForWindows</span></span> | <span data-ttu-id="3a02a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-114">Int64</span></span>  |
| <span data-ttu-id="3a02a-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="3a02a-115">outlookForMobile</span></span>  | <span data-ttu-id="3a02a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-116">Int64</span></span>  |
| <span data-ttu-id="3a02a-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="3a02a-117">otherForMobile</span></span>    | <span data-ttu-id="3a02a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-118">Int64</span></span>  |
| <span data-ttu-id="3a02a-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="3a02a-119">outlookForWeb</span></span>     | <span data-ttu-id="3a02a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-120">Int64</span></span>  |
| <span data-ttu-id="3a02a-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="3a02a-121">pop3App</span></span>           | <span data-ttu-id="3a02a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-122">Int64</span></span>  |
| <span data-ttu-id="3a02a-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="3a02a-123">imap4App</span></span>          | <span data-ttu-id="3a02a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-124">Int64</span></span>  |
| <span data-ttu-id="3a02a-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="3a02a-125">smtpApp</span></span>           | <span data-ttu-id="3a02a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="3a02a-126">Int64</span></span>  |
| <span data-ttu-id="3a02a-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3a02a-127">reportPeriod</span></span>      | <span data-ttu-id="3a02a-128">String</span><span class="sxs-lookup"><span data-stu-id="3a02a-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3a02a-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a02a-129">JSON representation</span></span>

<span data-ttu-id="3a02a-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a02a-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
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
  "reportPeriod": "String"
}
```
