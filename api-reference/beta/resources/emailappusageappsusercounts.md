---
title: Тип ресурса Емаилаппусажеаппсусеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0ca694c5d416dcc062984ba03a3521a39a010a87
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972182"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="eb438-103">Тип ресурса Емаилаппусажеаппсусеркаунтс</span><span class="sxs-lookup"><span data-stu-id="eb438-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="eb438-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb438-104">Properties</span></span>

| <span data-ttu-id="eb438-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb438-105">Property</span></span>          | <span data-ttu-id="eb438-106">Тип</span><span class="sxs-lookup"><span data-stu-id="eb438-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="eb438-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="eb438-107">reportRefreshDate</span></span> | <span data-ttu-id="eb438-108">Дата</span><span class="sxs-lookup"><span data-stu-id="eb438-108">Date</span></span>   |
| <span data-ttu-id="eb438-109">Маилформак</span><span class="sxs-lookup"><span data-stu-id="eb438-109">mailForMac</span></span>        | <span data-ttu-id="eb438-110">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-110">Int64</span></span>  |
| <span data-ttu-id="eb438-111">Аутлукформак</span><span class="sxs-lookup"><span data-stu-id="eb438-111">outlookForMac</span></span>     | <span data-ttu-id="eb438-112">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-112">Int64</span></span>  |
| <span data-ttu-id="eb438-113">Аутлукфорвиндовс</span><span class="sxs-lookup"><span data-stu-id="eb438-113">outlookForWindows</span></span> | <span data-ttu-id="eb438-114">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-114">Int64</span></span>  |
| <span data-ttu-id="eb438-115">Аутлукформобиле</span><span class="sxs-lookup"><span data-stu-id="eb438-115">outlookForMobile</span></span>  | <span data-ttu-id="eb438-116">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-116">Int64</span></span>  |
| <span data-ttu-id="eb438-117">Осерформобиле</span><span class="sxs-lookup"><span data-stu-id="eb438-117">otherForMobile</span></span>    | <span data-ttu-id="eb438-118">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-118">Int64</span></span>  |
| <span data-ttu-id="eb438-119">Аутлукфорвеб</span><span class="sxs-lookup"><span data-stu-id="eb438-119">outlookForWeb</span></span>     | <span data-ttu-id="eb438-120">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-120">Int64</span></span>  |
| <span data-ttu-id="eb438-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="eb438-121">pop3App</span></span>           | <span data-ttu-id="eb438-122">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-122">Int64</span></span>  |
| <span data-ttu-id="eb438-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="eb438-123">imap4App</span></span>          | <span data-ttu-id="eb438-124">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-124">Int64</span></span>  |
| <span data-ttu-id="eb438-125">Смтпапп</span><span class="sxs-lookup"><span data-stu-id="eb438-125">smtpApp</span></span>           | <span data-ttu-id="eb438-126">Int64</span><span class="sxs-lookup"><span data-stu-id="eb438-126">Int64</span></span>  |
| <span data-ttu-id="eb438-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="eb438-127">reportPeriod</span></span>      | <span data-ttu-id="eb438-128">String</span><span class="sxs-lookup"><span data-stu-id="eb438-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eb438-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb438-129">JSON representation</span></span>

<span data-ttu-id="eb438-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb438-130">The following is a JSON representation of the resource.</span></span>

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
