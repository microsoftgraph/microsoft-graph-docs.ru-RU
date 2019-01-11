---
title: Тип ресурса sharePointActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 4503739a7b2e13cade72951ae56ab410f22608b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880698"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="1d47c-103">Тип ресурса sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1d47c-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1d47c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d47c-104">Properties</span></span>

| <span data-ttu-id="1d47c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d47c-105">Property</span></span>                  | <span data-ttu-id="1d47c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="1d47c-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="1d47c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1d47c-107">reportRefreshDate</span></span>         | <span data-ttu-id="1d47c-108">Date</span><span class="sxs-lookup"><span data-stu-id="1d47c-108">Date</span></span>              |
| <span data-ttu-id="1d47c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1d47c-109">userPrincipalName</span></span>         | <span data-ttu-id="1d47c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="1d47c-110">String</span></span>            |
| <span data-ttu-id="1d47c-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1d47c-111">isDeleted</span></span>                 | <span data-ttu-id="1d47c-112">Логический</span><span class="sxs-lookup"><span data-stu-id="1d47c-112">Boolean</span></span>           |
| <span data-ttu-id="1d47c-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="1d47c-113">deletedDate</span></span>               | <span data-ttu-id="1d47c-114">Date</span><span class="sxs-lookup"><span data-stu-id="1d47c-114">Date</span></span>              |
| <span data-ttu-id="1d47c-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="1d47c-115">lastActivityDate</span></span>          | <span data-ttu-id="1d47c-116">Date</span><span class="sxs-lookup"><span data-stu-id="1d47c-116">Date</span></span>              |
| <span data-ttu-id="1d47c-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="1d47c-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="1d47c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1d47c-118">Int64</span></span>             |
| <span data-ttu-id="1d47c-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="1d47c-119">syncedFileCount</span></span>           | <span data-ttu-id="1d47c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1d47c-120">Int64</span></span>             |
| <span data-ttu-id="1d47c-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="1d47c-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="1d47c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1d47c-122">Int64</span></span>             |
| <span data-ttu-id="1d47c-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="1d47c-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="1d47c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1d47c-124">Int64</span></span>             |
| <span data-ttu-id="1d47c-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="1d47c-125">visitedPageCount</span></span>          | <span data-ttu-id="1d47c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="1d47c-126">Int64</span></span>             |
| <span data-ttu-id="1d47c-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="1d47c-127">assignedProducts</span></span>          | <span data-ttu-id="1d47c-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1d47c-128">String collection</span></span> |
| <span data-ttu-id="1d47c-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1d47c-129">reportPeriod</span></span>              | <span data-ttu-id="1d47c-130">String</span><span class="sxs-lookup"><span data-stu-id="1d47c-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="1d47c-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d47c-131">JSON representation</span></span>

<span data-ttu-id="1d47c-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d47c-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "visitedPageCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
