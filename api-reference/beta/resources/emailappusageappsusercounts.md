---
title: Тип ресурса Емаилаппусажеаппсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34ceaf4450a66f07c0678e55db344adc20bb0b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499500"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="fa4fa-103">Тип ресурса Емаилаппусажеаппсусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="fa4fa-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="fa4fa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa4fa-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="fa4fa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa4fa-105">Properties</span></span>

| <span data-ttu-id="fa4fa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa4fa-106">Property</span></span>          | <span data-ttu-id="fa4fa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fa4fa-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fa4fa-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="fa4fa-108">reportRefreshDate</span></span> | <span data-ttu-id="fa4fa-109">Дата</span><span class="sxs-lookup"><span data-stu-id="fa4fa-109">Date</span></span>   |
| <span data-ttu-id="fa4fa-110">маилформак</span><span class="sxs-lookup"><span data-stu-id="fa4fa-110">mailForMac</span></span>        | <span data-ttu-id="fa4fa-111">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-111">Int64</span></span>  |
| <span data-ttu-id="fa4fa-112">аутлукформак</span><span class="sxs-lookup"><span data-stu-id="fa4fa-112">outlookForMac</span></span>     | <span data-ttu-id="fa4fa-113">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-113">Int64</span></span>  |
| <span data-ttu-id="fa4fa-114">аутлукфорвиндовс</span><span class="sxs-lookup"><span data-stu-id="fa4fa-114">outlookForWindows</span></span> | <span data-ttu-id="fa4fa-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-115">Int64</span></span>  |
| <span data-ttu-id="fa4fa-116">аутлукформобиле</span><span class="sxs-lookup"><span data-stu-id="fa4fa-116">outlookForMobile</span></span>  | <span data-ttu-id="fa4fa-117">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-117">Int64</span></span>  |
| <span data-ttu-id="fa4fa-118">осерформобиле</span><span class="sxs-lookup"><span data-stu-id="fa4fa-118">otherForMobile</span></span>    | <span data-ttu-id="fa4fa-119">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-119">Int64</span></span>  |
| <span data-ttu-id="fa4fa-120">аутлукфорвеб</span><span class="sxs-lookup"><span data-stu-id="fa4fa-120">outlookForWeb</span></span>     | <span data-ttu-id="fa4fa-121">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-121">Int64</span></span>  |
| <span data-ttu-id="fa4fa-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="fa4fa-122">pop3App</span></span>           | <span data-ttu-id="fa4fa-123">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-123">Int64</span></span>  |
| <span data-ttu-id="fa4fa-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="fa4fa-124">imap4App</span></span>          | <span data-ttu-id="fa4fa-125">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-125">Int64</span></span>  |
| <span data-ttu-id="fa4fa-126">смтпапп</span><span class="sxs-lookup"><span data-stu-id="fa4fa-126">smtpApp</span></span>           | <span data-ttu-id="fa4fa-127">Int64</span><span class="sxs-lookup"><span data-stu-id="fa4fa-127">Int64</span></span>  |
| <span data-ttu-id="fa4fa-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="fa4fa-128">reportPeriod</span></span>      | <span data-ttu-id="fa4fa-129">String</span><span class="sxs-lookup"><span data-stu-id="fa4fa-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa4fa-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa4fa-130">JSON representation</span></span>

<span data-ttu-id="fa4fa-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa4fa-131">The following is a JSON representation of the resource.</span></span>

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
