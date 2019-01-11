---
title: Тип ресурса emailAppUsageAppsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: efbc4ce75293237813e9a835cb45ff0bf0ec4b26
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807821"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="bdd81-103">Тип ресурса emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="bdd81-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bdd81-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="bdd81-104">Properties</span></span>

| <span data-ttu-id="bdd81-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdd81-105">Property</span></span>          | <span data-ttu-id="bdd81-106">Тип</span><span class="sxs-lookup"><span data-stu-id="bdd81-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="bdd81-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bdd81-107">reportRefreshDate</span></span> | <span data-ttu-id="bdd81-108">Date</span><span class="sxs-lookup"><span data-stu-id="bdd81-108">Date</span></span>   |
| <span data-ttu-id="bdd81-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="bdd81-109">mailForMac</span></span>        | <span data-ttu-id="bdd81-110">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-110">Int64</span></span>  |
| <span data-ttu-id="bdd81-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="bdd81-111">outlookForMac</span></span>     | <span data-ttu-id="bdd81-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-112">Int64</span></span>  |
| <span data-ttu-id="bdd81-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="bdd81-113">outlookForWindows</span></span> | <span data-ttu-id="bdd81-114">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-114">Int64</span></span>  |
| <span data-ttu-id="bdd81-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="bdd81-115">outlookForMobile</span></span>  | <span data-ttu-id="bdd81-116">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-116">Int64</span></span>  |
| <span data-ttu-id="bdd81-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="bdd81-117">otherForMobile</span></span>    | <span data-ttu-id="bdd81-118">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-118">Int64</span></span>  |
| <span data-ttu-id="bdd81-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="bdd81-119">outlookForWeb</span></span>     | <span data-ttu-id="bdd81-120">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-120">Int64</span></span>  |
| <span data-ttu-id="bdd81-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="bdd81-121">pop3App</span></span>           | <span data-ttu-id="bdd81-122">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-122">Int64</span></span>  |
| <span data-ttu-id="bdd81-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="bdd81-123">imap4App</span></span>          | <span data-ttu-id="bdd81-124">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-124">Int64</span></span>  |
| <span data-ttu-id="bdd81-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="bdd81-125">smtpApp</span></span>           | <span data-ttu-id="bdd81-126">Int64</span><span class="sxs-lookup"><span data-stu-id="bdd81-126">Int64</span></span>  |
| <span data-ttu-id="bdd81-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bdd81-127">reportPeriod</span></span>      | <span data-ttu-id="bdd81-128">String</span><span class="sxs-lookup"><span data-stu-id="bdd81-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bdd81-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bdd81-129">JSON representation</span></span>

<span data-ttu-id="bdd81-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdd81-130">The following is a JSON representation of the resource.</span></span>

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
