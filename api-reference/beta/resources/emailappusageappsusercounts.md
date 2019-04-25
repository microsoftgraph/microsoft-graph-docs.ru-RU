---
title: Тип ресурса Емаилаппусажеаппсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542813"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="dd32a-103">Тип ресурса Емаилаппусажеаппсусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="dd32a-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dd32a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd32a-104">Properties</span></span>

| <span data-ttu-id="dd32a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd32a-105">Property</span></span>          | <span data-ttu-id="dd32a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="dd32a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="dd32a-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="dd32a-107">reportRefreshDate</span></span> | <span data-ttu-id="dd32a-108">Дата</span><span class="sxs-lookup"><span data-stu-id="dd32a-108">Date</span></span>   |
| <span data-ttu-id="dd32a-109">Маилформак</span><span class="sxs-lookup"><span data-stu-id="dd32a-109">mailForMac</span></span>        | <span data-ttu-id="dd32a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-110">Int64</span></span>  |
| <span data-ttu-id="dd32a-111">Аутлукформак</span><span class="sxs-lookup"><span data-stu-id="dd32a-111">outlookForMac</span></span>     | <span data-ttu-id="dd32a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-112">Int64</span></span>  |
| <span data-ttu-id="dd32a-113">Аутлукфорвиндовс</span><span class="sxs-lookup"><span data-stu-id="dd32a-113">outlookForWindows</span></span> | <span data-ttu-id="dd32a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-114">Int64</span></span>  |
| <span data-ttu-id="dd32a-115">Аутлукформобиле</span><span class="sxs-lookup"><span data-stu-id="dd32a-115">outlookForMobile</span></span>  | <span data-ttu-id="dd32a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-116">Int64</span></span>  |
| <span data-ttu-id="dd32a-117">Осерформобиле</span><span class="sxs-lookup"><span data-stu-id="dd32a-117">otherForMobile</span></span>    | <span data-ttu-id="dd32a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-118">Int64</span></span>  |
| <span data-ttu-id="dd32a-119">Аутлукфорвеб</span><span class="sxs-lookup"><span data-stu-id="dd32a-119">outlookForWeb</span></span>     | <span data-ttu-id="dd32a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-120">Int64</span></span>  |
| <span data-ttu-id="dd32a-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="dd32a-121">pop3App</span></span>           | <span data-ttu-id="dd32a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-122">Int64</span></span>  |
| <span data-ttu-id="dd32a-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="dd32a-123">imap4App</span></span>          | <span data-ttu-id="dd32a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-124">Int64</span></span>  |
| <span data-ttu-id="dd32a-125">Смтпапп</span><span class="sxs-lookup"><span data-stu-id="dd32a-125">smtpApp</span></span>           | <span data-ttu-id="dd32a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="dd32a-126">Int64</span></span>  |
| <span data-ttu-id="dd32a-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="dd32a-127">reportPeriod</span></span>      | <span data-ttu-id="dd32a-128">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd32a-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dd32a-129">JSON representation</span></span>

<span data-ttu-id="dd32a-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd32a-130">The following is a JSON representation of the resource.</span></span>

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
