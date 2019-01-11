---
title: Тип ресурса oneDriveActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 2f498c7c9507c4210f12f76d57f62729f84da578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820792"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="264a8-103">Тип ресурса oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="264a8-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="264a8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="264a8-104">Properties</span></span>

| <span data-ttu-id="264a8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="264a8-105">Property</span></span>                  | <span data-ttu-id="264a8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="264a8-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="264a8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="264a8-107">reportRefreshDate</span></span>         | <span data-ttu-id="264a8-108">Date</span><span class="sxs-lookup"><span data-stu-id="264a8-108">Date</span></span>              |
| <span data-ttu-id="264a8-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="264a8-109">userPrincipalName</span></span>         | <span data-ttu-id="264a8-110">Строка</span><span class="sxs-lookup"><span data-stu-id="264a8-110">String</span></span>            |
| <span data-ttu-id="264a8-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="264a8-111">isDeleted</span></span>                 | <span data-ttu-id="264a8-112">Логический</span><span class="sxs-lookup"><span data-stu-id="264a8-112">Boolean</span></span>           |
| <span data-ttu-id="264a8-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="264a8-113">deletedDate</span></span>               | <span data-ttu-id="264a8-114">Date</span><span class="sxs-lookup"><span data-stu-id="264a8-114">Date</span></span>              |
| <span data-ttu-id="264a8-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="264a8-115">lastActivityDate</span></span>          | <span data-ttu-id="264a8-116">Date</span><span class="sxs-lookup"><span data-stu-id="264a8-116">Date</span></span>              |
| <span data-ttu-id="264a8-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="264a8-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="264a8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="264a8-118">Int64</span></span>             |
| <span data-ttu-id="264a8-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="264a8-119">syncedFileCount</span></span>           | <span data-ttu-id="264a8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="264a8-120">Int64</span></span>             |
| <span data-ttu-id="264a8-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="264a8-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="264a8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="264a8-122">Int64</span></span>             |
| <span data-ttu-id="264a8-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="264a8-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="264a8-124">Int64</span><span class="sxs-lookup"><span data-stu-id="264a8-124">Int64</span></span>             |
| <span data-ttu-id="264a8-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="264a8-125">assignedProducts</span></span>          | <span data-ttu-id="264a8-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="264a8-126">String collection</span></span> |
| <span data-ttu-id="264a8-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="264a8-127">reportPeriod</span></span>              | <span data-ttu-id="264a8-128">String</span><span class="sxs-lookup"><span data-stu-id="264a8-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="264a8-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="264a8-129">JSON representation</span></span>

<span data-ttu-id="264a8-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="264a8-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
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
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
