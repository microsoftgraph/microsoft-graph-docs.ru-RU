---
title: Тип ресурса oneDriveActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 679ec9b8452d388fe311e67d88bcfffd6fe73d93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077522"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="f792b-103">Тип ресурса oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f792b-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f792b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f792b-104">Properties</span></span>

| <span data-ttu-id="f792b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f792b-105">Property</span></span>                  | <span data-ttu-id="f792b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f792b-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="f792b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f792b-107">reportRefreshDate</span></span>         | <span data-ttu-id="f792b-108">Date</span><span class="sxs-lookup"><span data-stu-id="f792b-108">Date</span></span>              |
| <span data-ttu-id="f792b-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f792b-109">userPrincipalName</span></span>         | <span data-ttu-id="f792b-110">String</span><span class="sxs-lookup"><span data-stu-id="f792b-110">String</span></span>            |
| <span data-ttu-id="f792b-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f792b-111">isDeleted</span></span>                 | <span data-ttu-id="f792b-112">Логический</span><span class="sxs-lookup"><span data-stu-id="f792b-112">Boolean</span></span>           |
| <span data-ttu-id="f792b-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="f792b-113">deletedDate</span></span>               | <span data-ttu-id="f792b-114">Date</span><span class="sxs-lookup"><span data-stu-id="f792b-114">Date</span></span>              |
| <span data-ttu-id="f792b-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f792b-115">lastActivityDate</span></span>          | <span data-ttu-id="f792b-116">Date</span><span class="sxs-lookup"><span data-stu-id="f792b-116">Date</span></span>              |
| <span data-ttu-id="f792b-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="f792b-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="f792b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f792b-118">Int64</span></span>             |
| <span data-ttu-id="f792b-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="f792b-119">syncedFileCount</span></span>           | <span data-ttu-id="f792b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f792b-120">Int64</span></span>             |
| <span data-ttu-id="f792b-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="f792b-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="f792b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f792b-122">Int64</span></span>             |
| <span data-ttu-id="f792b-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="f792b-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="f792b-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f792b-124">Int64</span></span>             |
| <span data-ttu-id="f792b-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="f792b-125">assignedProducts</span></span>          | <span data-ttu-id="f792b-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f792b-126">String collection</span></span> |
| <span data-ttu-id="f792b-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f792b-127">reportPeriod</span></span>              | <span data-ttu-id="f792b-128">String</span><span class="sxs-lookup"><span data-stu-id="f792b-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="f792b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f792b-129">JSON representation</span></span>

<span data-ttu-id="f792b-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f792b-130">The following is a JSON representation of the resource.</span></span>

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
