---
title: Тип ресурса emailAppUsageAppsUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: e588a671129c6aa131bce781e3a6db0d44128f6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077676"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="45124-103">Тип ресурса emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="45124-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="45124-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="45124-104">Properties</span></span>

| <span data-ttu-id="45124-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="45124-105">Property</span></span>          | <span data-ttu-id="45124-106">Тип</span><span class="sxs-lookup"><span data-stu-id="45124-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="45124-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="45124-107">reportRefreshDate</span></span> | <span data-ttu-id="45124-108">Date</span><span class="sxs-lookup"><span data-stu-id="45124-108">Date</span></span>   |
| <span data-ttu-id="45124-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="45124-109">mailForMac</span></span>        | <span data-ttu-id="45124-110">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-110">Int64</span></span>  |
| <span data-ttu-id="45124-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="45124-111">outlookForMac</span></span>     | <span data-ttu-id="45124-112">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-112">Int64</span></span>  |
| <span data-ttu-id="45124-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="45124-113">outlookForWindows</span></span> | <span data-ttu-id="45124-114">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-114">Int64</span></span>  |
| <span data-ttu-id="45124-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="45124-115">outlookForMobile</span></span>  | <span data-ttu-id="45124-116">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-116">Int64</span></span>  |
| <span data-ttu-id="45124-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="45124-117">otherForMobile</span></span>    | <span data-ttu-id="45124-118">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-118">Int64</span></span>  |
| <span data-ttu-id="45124-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="45124-119">outlookForWeb</span></span>     | <span data-ttu-id="45124-120">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-120">Int64</span></span>  |
| <span data-ttu-id="45124-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="45124-121">pop3App</span></span>           | <span data-ttu-id="45124-122">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-122">Int64</span></span>  |
| <span data-ttu-id="45124-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="45124-123">imap4App</span></span>          | <span data-ttu-id="45124-124">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-124">Int64</span></span>  |
| <span data-ttu-id="45124-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="45124-125">smtpApp</span></span>           | <span data-ttu-id="45124-126">Int64</span><span class="sxs-lookup"><span data-stu-id="45124-126">Int64</span></span>  |
| <span data-ttu-id="45124-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="45124-127">reportPeriod</span></span>      | <span data-ttu-id="45124-128">String</span><span class="sxs-lookup"><span data-stu-id="45124-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45124-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45124-129">JSON representation</span></span>

<span data-ttu-id="45124-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45124-130">The following is a JSON representation of the resource.</span></span>

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
