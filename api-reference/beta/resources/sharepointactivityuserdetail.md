---
title: Тип ресурса sharePointActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7dc324d821dca26ff1083f1e48c258e1955d72f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979945"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="a9638-103">Тип ресурса sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="a9638-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a9638-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9638-104">Properties</span></span>

| <span data-ttu-id="a9638-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9638-105">Property</span></span>                  | <span data-ttu-id="a9638-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a9638-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="a9638-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a9638-107">reportRefreshDate</span></span>         | <span data-ttu-id="a9638-108">Date</span><span class="sxs-lookup"><span data-stu-id="a9638-108">Date</span></span>              |
| <span data-ttu-id="a9638-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9638-109">userPrincipalName</span></span>         | <span data-ttu-id="a9638-110">Строка</span><span class="sxs-lookup"><span data-stu-id="a9638-110">String</span></span>            |
| <span data-ttu-id="a9638-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a9638-111">isDeleted</span></span>                 | <span data-ttu-id="a9638-112">Логический</span><span class="sxs-lookup"><span data-stu-id="a9638-112">Boolean</span></span>           |
| <span data-ttu-id="a9638-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a9638-113">deletedDate</span></span>               | <span data-ttu-id="a9638-114">Date</span><span class="sxs-lookup"><span data-stu-id="a9638-114">Date</span></span>              |
| <span data-ttu-id="a9638-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a9638-115">lastActivityDate</span></span>          | <span data-ttu-id="a9638-116">Date</span><span class="sxs-lookup"><span data-stu-id="a9638-116">Date</span></span>              |
| <span data-ttu-id="a9638-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="a9638-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="a9638-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a9638-118">Int64</span></span>             |
| <span data-ttu-id="a9638-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="a9638-119">syncedFileCount</span></span>           | <span data-ttu-id="a9638-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a9638-120">Int64</span></span>             |
| <span data-ttu-id="a9638-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a9638-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="a9638-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a9638-122">Int64</span></span>             |
| <span data-ttu-id="a9638-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a9638-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="a9638-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a9638-124">Int64</span></span>             |
| <span data-ttu-id="a9638-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="a9638-125">visitedPageCount</span></span>          | <span data-ttu-id="a9638-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a9638-126">Int64</span></span>             |
| <span data-ttu-id="a9638-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="a9638-127">assignedProducts</span></span>          | <span data-ttu-id="a9638-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9638-128">String collection</span></span> |
| <span data-ttu-id="a9638-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a9638-129">reportPeriod</span></span>              | <span data-ttu-id="a9638-130">String</span><span class="sxs-lookup"><span data-stu-id="a9638-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a9638-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9638-131">JSON representation</span></span>

<span data-ttu-id="a9638-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9638-132">The following is a JSON representation of the resource.</span></span>

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
