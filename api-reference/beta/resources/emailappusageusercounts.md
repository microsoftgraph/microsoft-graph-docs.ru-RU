---
title: Тип ресурса Емаилаппусажеусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7822528aacc9d6f104012d43004fbb9aabba127c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506694"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="4a95c-103">Тип ресурса Емаилаппусажеусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="4a95c-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4a95c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a95c-104">Properties</span></span>

| <span data-ttu-id="4a95c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a95c-105">Property</span></span>          | <span data-ttu-id="4a95c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4a95c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4a95c-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="4a95c-107">reportRefreshDate</span></span> | <span data-ttu-id="4a95c-108">Дата</span><span class="sxs-lookup"><span data-stu-id="4a95c-108">Date</span></span>   |
| <span data-ttu-id="4a95c-109">Маилформак</span><span class="sxs-lookup"><span data-stu-id="4a95c-109">mailForMac</span></span>        | <span data-ttu-id="4a95c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-110">Int64</span></span>  |
| <span data-ttu-id="4a95c-111">Аутлукформак</span><span class="sxs-lookup"><span data-stu-id="4a95c-111">outlookForMac</span></span>     | <span data-ttu-id="4a95c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-112">Int64</span></span>  |
| <span data-ttu-id="4a95c-113">Аутлукфорвиндовс</span><span class="sxs-lookup"><span data-stu-id="4a95c-113">outlookForWindows</span></span> | <span data-ttu-id="4a95c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-114">Int64</span></span>  |
| <span data-ttu-id="4a95c-115">Аутлукформобиле</span><span class="sxs-lookup"><span data-stu-id="4a95c-115">outlookForMobile</span></span>  | <span data-ttu-id="4a95c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-116">Int64</span></span>  |
| <span data-ttu-id="4a95c-117">Осерформобиле</span><span class="sxs-lookup"><span data-stu-id="4a95c-117">otherForMobile</span></span>    | <span data-ttu-id="4a95c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-118">Int64</span></span>  |
| <span data-ttu-id="4a95c-119">Аутлукфорвеб</span><span class="sxs-lookup"><span data-stu-id="4a95c-119">outlookForWeb</span></span>     | <span data-ttu-id="4a95c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-120">Int64</span></span>  |
| <span data-ttu-id="4a95c-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="4a95c-121">pop3App</span></span>           | <span data-ttu-id="4a95c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-122">Int64</span></span>  |
| <span data-ttu-id="4a95c-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="4a95c-123">imap4App</span></span>          | <span data-ttu-id="4a95c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-124">Int64</span></span>  |
| <span data-ttu-id="4a95c-125">Смтпапп</span><span class="sxs-lookup"><span data-stu-id="4a95c-125">smtpApp</span></span>           | <span data-ttu-id="4a95c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4a95c-126">Int64</span></span>  |
| <span data-ttu-id="4a95c-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="4a95c-127">reportDate</span></span>        | <span data-ttu-id="4a95c-128">Дата</span><span class="sxs-lookup"><span data-stu-id="4a95c-128">Date</span></span>   |
| <span data-ttu-id="4a95c-129">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="4a95c-129">reportPeriod</span></span>      | <span data-ttu-id="4a95c-130">String</span><span class="sxs-lookup"><span data-stu-id="4a95c-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a95c-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a95c-131">JSON representation</span></span>

<span data-ttu-id="4a95c-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a95c-132">The following is a JSON representation of the resource.</span></span>

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
