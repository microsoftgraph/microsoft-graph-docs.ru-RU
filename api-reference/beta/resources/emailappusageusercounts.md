---
title: Тип ресурса Емаилаппусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 18ce0629bbb2a700d873587de6d3e5244304bcb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499493"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="2c659-103">Тип ресурса Емаилаппусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="2c659-103">emailAppUsageUserCounts resource type</span></span>

<span data-ttu-id="2c659-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2c659-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2c659-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c659-105">Properties</span></span>

| <span data-ttu-id="2c659-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c659-106">Property</span></span>          | <span data-ttu-id="2c659-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2c659-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2c659-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="2c659-108">reportRefreshDate</span></span> | <span data-ttu-id="2c659-109">Дата</span><span class="sxs-lookup"><span data-stu-id="2c659-109">Date</span></span>   |
| <span data-ttu-id="2c659-110">маилформак</span><span class="sxs-lookup"><span data-stu-id="2c659-110">mailForMac</span></span>        | <span data-ttu-id="2c659-111">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-111">Int64</span></span>  |
| <span data-ttu-id="2c659-112">аутлукформак</span><span class="sxs-lookup"><span data-stu-id="2c659-112">outlookForMac</span></span>     | <span data-ttu-id="2c659-113">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-113">Int64</span></span>  |
| <span data-ttu-id="2c659-114">аутлукфорвиндовс</span><span class="sxs-lookup"><span data-stu-id="2c659-114">outlookForWindows</span></span> | <span data-ttu-id="2c659-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-115">Int64</span></span>  |
| <span data-ttu-id="2c659-116">аутлукформобиле</span><span class="sxs-lookup"><span data-stu-id="2c659-116">outlookForMobile</span></span>  | <span data-ttu-id="2c659-117">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-117">Int64</span></span>  |
| <span data-ttu-id="2c659-118">осерформобиле</span><span class="sxs-lookup"><span data-stu-id="2c659-118">otherForMobile</span></span>    | <span data-ttu-id="2c659-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-119">Int64</span></span>  |
| <span data-ttu-id="2c659-120">аутлукфорвеб</span><span class="sxs-lookup"><span data-stu-id="2c659-120">outlookForWeb</span></span>     | <span data-ttu-id="2c659-121">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-121">Int64</span></span>  |
| <span data-ttu-id="2c659-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="2c659-122">pop3App</span></span>           | <span data-ttu-id="2c659-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-123">Int64</span></span>  |
| <span data-ttu-id="2c659-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="2c659-124">imap4App</span></span>          | <span data-ttu-id="2c659-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-125">Int64</span></span>  |
| <span data-ttu-id="2c659-126">смтпапп</span><span class="sxs-lookup"><span data-stu-id="2c659-126">smtpApp</span></span>           | <span data-ttu-id="2c659-127">Int64</span><span class="sxs-lookup"><span data-stu-id="2c659-127">Int64</span></span>  |
| <span data-ttu-id="2c659-128">reportDate</span><span class="sxs-lookup"><span data-stu-id="2c659-128">reportDate</span></span>        | <span data-ttu-id="2c659-129">Дата</span><span class="sxs-lookup"><span data-stu-id="2c659-129">Date</span></span>   |
| <span data-ttu-id="2c659-130">репортпериод</span><span class="sxs-lookup"><span data-stu-id="2c659-130">reportPeriod</span></span>      | <span data-ttu-id="2c659-131">String</span><span class="sxs-lookup"><span data-stu-id="2c659-131">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c659-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c659-132">JSON representation</span></span>

<span data-ttu-id="2c659-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c659-133">The following is a JSON representation of the resource.</span></span>

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
