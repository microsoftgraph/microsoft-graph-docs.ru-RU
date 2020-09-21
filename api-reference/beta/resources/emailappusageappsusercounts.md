---
title: Тип ресурса Емаилаппусажеаппсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d4dd1bc6a84b1d3e5f1b412986de686c9e6f5312
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979478"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="1005e-103">Тип ресурса Емаилаппусажеаппсусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="1005e-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="1005e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1005e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="1005e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1005e-105">Properties</span></span>

| <span data-ttu-id="1005e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1005e-106">Property</span></span>          | <span data-ttu-id="1005e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1005e-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1005e-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="1005e-108">reportRefreshDate</span></span> | <span data-ttu-id="1005e-109">Дата</span><span class="sxs-lookup"><span data-stu-id="1005e-109">Date</span></span>   |
| <span data-ttu-id="1005e-110">маилформак</span><span class="sxs-lookup"><span data-stu-id="1005e-110">mailForMac</span></span>        | <span data-ttu-id="1005e-111">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-111">Int64</span></span>  |
| <span data-ttu-id="1005e-112">аутлукформак</span><span class="sxs-lookup"><span data-stu-id="1005e-112">outlookForMac</span></span>     | <span data-ttu-id="1005e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-113">Int64</span></span>  |
| <span data-ttu-id="1005e-114">аутлукфорвиндовс</span><span class="sxs-lookup"><span data-stu-id="1005e-114">outlookForWindows</span></span> | <span data-ttu-id="1005e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-115">Int64</span></span>  |
| <span data-ttu-id="1005e-116">аутлукформобиле</span><span class="sxs-lookup"><span data-stu-id="1005e-116">outlookForMobile</span></span>  | <span data-ttu-id="1005e-117">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-117">Int64</span></span>  |
| <span data-ttu-id="1005e-118">осерформобиле</span><span class="sxs-lookup"><span data-stu-id="1005e-118">otherForMobile</span></span>    | <span data-ttu-id="1005e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-119">Int64</span></span>  |
| <span data-ttu-id="1005e-120">аутлукфорвеб</span><span class="sxs-lookup"><span data-stu-id="1005e-120">outlookForWeb</span></span>     | <span data-ttu-id="1005e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-121">Int64</span></span>  |
| <span data-ttu-id="1005e-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="1005e-122">pop3App</span></span>           | <span data-ttu-id="1005e-123">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-123">Int64</span></span>  |
| <span data-ttu-id="1005e-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="1005e-124">imap4App</span></span>          | <span data-ttu-id="1005e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-125">Int64</span></span>  |
| <span data-ttu-id="1005e-126">смтпапп</span><span class="sxs-lookup"><span data-stu-id="1005e-126">smtpApp</span></span>           | <span data-ttu-id="1005e-127">Int64</span><span class="sxs-lookup"><span data-stu-id="1005e-127">Int64</span></span>  |
| <span data-ttu-id="1005e-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="1005e-128">reportPeriod</span></span>      | <span data-ttu-id="1005e-129">String</span><span class="sxs-lookup"><span data-stu-id="1005e-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1005e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1005e-130">JSON representation</span></span>

<span data-ttu-id="1005e-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1005e-131">The following is a JSON representation of the resource.</span></span>

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


