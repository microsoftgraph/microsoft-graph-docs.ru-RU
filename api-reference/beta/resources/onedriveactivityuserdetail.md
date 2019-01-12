---
title: Тип ресурса oneDriveActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948249"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="9e9d2-103">Тип ресурса oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9e9d2-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9e9d2-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e9d2-104">Properties</span></span>

| <span data-ttu-id="9e9d2-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e9d2-105">Property</span></span>                  | <span data-ttu-id="9e9d2-106">Тип</span><span class="sxs-lookup"><span data-stu-id="9e9d2-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="9e9d2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9e9d2-107">reportRefreshDate</span></span>         | <span data-ttu-id="9e9d2-108">Date</span><span class="sxs-lookup"><span data-stu-id="9e9d2-108">Date</span></span>              |
| <span data-ttu-id="9e9d2-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9e9d2-109">userPrincipalName</span></span>         | <span data-ttu-id="9e9d2-110">Строка</span><span class="sxs-lookup"><span data-stu-id="9e9d2-110">String</span></span>            |
| <span data-ttu-id="9e9d2-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9e9d2-111">isDeleted</span></span>                 | <span data-ttu-id="9e9d2-112">Логический</span><span class="sxs-lookup"><span data-stu-id="9e9d2-112">Boolean</span></span>           |
| <span data-ttu-id="9e9d2-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="9e9d2-113">deletedDate</span></span>               | <span data-ttu-id="9e9d2-114">Date</span><span class="sxs-lookup"><span data-stu-id="9e9d2-114">Date</span></span>              |
| <span data-ttu-id="9e9d2-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="9e9d2-115">lastActivityDate</span></span>          | <span data-ttu-id="9e9d2-116">Date</span><span class="sxs-lookup"><span data-stu-id="9e9d2-116">Date</span></span>              |
| <span data-ttu-id="9e9d2-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="9e9d2-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="9e9d2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9e9d2-118">Int64</span></span>             |
| <span data-ttu-id="9e9d2-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="9e9d2-119">syncedFileCount</span></span>           | <span data-ttu-id="9e9d2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="9e9d2-120">Int64</span></span>             |
| <span data-ttu-id="9e9d2-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="9e9d2-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="9e9d2-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9e9d2-122">Int64</span></span>             |
| <span data-ttu-id="9e9d2-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="9e9d2-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="9e9d2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="9e9d2-124">Int64</span></span>             |
| <span data-ttu-id="9e9d2-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="9e9d2-125">assignedProducts</span></span>          | <span data-ttu-id="9e9d2-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9e9d2-126">String collection</span></span> |
| <span data-ttu-id="9e9d2-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9e9d2-127">reportPeriod</span></span>              | <span data-ttu-id="9e9d2-128">String</span><span class="sxs-lookup"><span data-stu-id="9e9d2-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="9e9d2-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e9d2-129">JSON representation</span></span>

<span data-ttu-id="9e9d2-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e9d2-130">The following is a JSON representation of the resource.</span></span>

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
