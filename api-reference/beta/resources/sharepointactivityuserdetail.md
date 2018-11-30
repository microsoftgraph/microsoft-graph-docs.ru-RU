---
title: Тип ресурса sharePointActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: a5b6de8a4a9b82d9e6d34a2ae289f0c7589798ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075477"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="171fb-103">Тип ресурса sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="171fb-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="171fb-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="171fb-104">Properties</span></span>

| <span data-ttu-id="171fb-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="171fb-105">Property</span></span>                  | <span data-ttu-id="171fb-106">Тип</span><span class="sxs-lookup"><span data-stu-id="171fb-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="171fb-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="171fb-107">reportRefreshDate</span></span>         | <span data-ttu-id="171fb-108">Date</span><span class="sxs-lookup"><span data-stu-id="171fb-108">Date</span></span>              |
| <span data-ttu-id="171fb-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="171fb-109">userPrincipalName</span></span>         | <span data-ttu-id="171fb-110">String</span><span class="sxs-lookup"><span data-stu-id="171fb-110">String</span></span>            |
| <span data-ttu-id="171fb-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="171fb-111">isDeleted</span></span>                 | <span data-ttu-id="171fb-112">Логический</span><span class="sxs-lookup"><span data-stu-id="171fb-112">Boolean</span></span>           |
| <span data-ttu-id="171fb-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="171fb-113">deletedDate</span></span>               | <span data-ttu-id="171fb-114">Date</span><span class="sxs-lookup"><span data-stu-id="171fb-114">Date</span></span>              |
| <span data-ttu-id="171fb-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="171fb-115">lastActivityDate</span></span>          | <span data-ttu-id="171fb-116">Date</span><span class="sxs-lookup"><span data-stu-id="171fb-116">Date</span></span>              |
| <span data-ttu-id="171fb-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="171fb-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="171fb-118">Int64</span><span class="sxs-lookup"><span data-stu-id="171fb-118">Int64</span></span>             |
| <span data-ttu-id="171fb-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="171fb-119">syncedFileCount</span></span>           | <span data-ttu-id="171fb-120">Int64</span><span class="sxs-lookup"><span data-stu-id="171fb-120">Int64</span></span>             |
| <span data-ttu-id="171fb-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="171fb-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="171fb-122">Int64</span><span class="sxs-lookup"><span data-stu-id="171fb-122">Int64</span></span>             |
| <span data-ttu-id="171fb-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="171fb-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="171fb-124">Int64</span><span class="sxs-lookup"><span data-stu-id="171fb-124">Int64</span></span>             |
| <span data-ttu-id="171fb-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="171fb-125">visitedPageCount</span></span>          | <span data-ttu-id="171fb-126">Int64</span><span class="sxs-lookup"><span data-stu-id="171fb-126">Int64</span></span>             |
| <span data-ttu-id="171fb-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="171fb-127">assignedProducts</span></span>          | <span data-ttu-id="171fb-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="171fb-128">String collection</span></span> |
| <span data-ttu-id="171fb-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="171fb-129">reportPeriod</span></span>              | <span data-ttu-id="171fb-130">String</span><span class="sxs-lookup"><span data-stu-id="171fb-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="171fb-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="171fb-131">JSON representation</span></span>

<span data-ttu-id="171fb-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="171fb-132">The following is a JSON representation of the resource.</span></span>

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
