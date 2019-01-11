---
title: Тип ресурса oneDriveUsageAccountDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 92695f509302ede4b3ce64320e8f4ed42418f7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842611"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="bec5c-103">Тип ресурса oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="bec5c-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bec5c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="bec5c-104">Properties</span></span>

| <span data-ttu-id="bec5c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="bec5c-105">Property</span></span>                | <span data-ttu-id="bec5c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="bec5c-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="bec5c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bec5c-107">reportRefreshDate</span></span>       | <span data-ttu-id="bec5c-108">Date</span><span class="sxs-lookup"><span data-stu-id="bec5c-108">Date</span></span>    |
| <span data-ttu-id="bec5c-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="bec5c-109">siteUrl</span></span>                 | <span data-ttu-id="bec5c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="bec5c-110">String</span></span>  |
| <span data-ttu-id="bec5c-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="bec5c-111">ownerDisplayName</span></span>        | <span data-ttu-id="bec5c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="bec5c-112">String</span></span>  |
| <span data-ttu-id="bec5c-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bec5c-113">isDeleted</span></span>               | <span data-ttu-id="bec5c-114">Логический</span><span class="sxs-lookup"><span data-stu-id="bec5c-114">Boolean</span></span> |
| <span data-ttu-id="bec5c-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bec5c-115">lastActivityDate</span></span>        | <span data-ttu-id="bec5c-116">Date</span><span class="sxs-lookup"><span data-stu-id="bec5c-116">Date</span></span>    |
| <span data-ttu-id="bec5c-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="bec5c-117">fileCount</span></span>               | <span data-ttu-id="bec5c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="bec5c-118">Int64</span></span>   |
| <span data-ttu-id="bec5c-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="bec5c-119">activeFileCount</span></span>         | <span data-ttu-id="bec5c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="bec5c-120">Int64</span></span>   |
| <span data-ttu-id="bec5c-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="bec5c-121">storageUsedInBytes</span></span>      | <span data-ttu-id="bec5c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="bec5c-122">Int64</span></span>   |
| <span data-ttu-id="bec5c-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="bec5c-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="bec5c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="bec5c-124">Int64</span></span>   |
| <span data-ttu-id="bec5c-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bec5c-125">reportPeriod</span></span>            | <span data-ttu-id="bec5c-126">String</span><span class="sxs-lookup"><span data-stu-id="bec5c-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="bec5c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bec5c-127">JSON representation</span></span>

<span data-ttu-id="bec5c-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bec5c-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
