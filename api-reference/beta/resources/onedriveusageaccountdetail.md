---
title: Тип ресурса oneDriveUsageAccountDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 4b80ebc24aa45be0368dbb59d6d3e99e7adacc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079699"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="df2e6-103">Тип ресурса oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="df2e6-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="df2e6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="df2e6-104">Properties</span></span>

| <span data-ttu-id="df2e6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="df2e6-105">Property</span></span>                | <span data-ttu-id="df2e6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="df2e6-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="df2e6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="df2e6-107">reportRefreshDate</span></span>       | <span data-ttu-id="df2e6-108">Date</span><span class="sxs-lookup"><span data-stu-id="df2e6-108">Date</span></span>    |
| <span data-ttu-id="df2e6-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="df2e6-109">siteUrl</span></span>                 | <span data-ttu-id="df2e6-110">String</span><span class="sxs-lookup"><span data-stu-id="df2e6-110">String</span></span>  |
| <span data-ttu-id="df2e6-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="df2e6-111">ownerDisplayName</span></span>        | <span data-ttu-id="df2e6-112">String</span><span class="sxs-lookup"><span data-stu-id="df2e6-112">String</span></span>  |
| <span data-ttu-id="df2e6-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="df2e6-113">isDeleted</span></span>               | <span data-ttu-id="df2e6-114">Логический</span><span class="sxs-lookup"><span data-stu-id="df2e6-114">Boolean</span></span> |
| <span data-ttu-id="df2e6-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="df2e6-115">lastActivityDate</span></span>        | <span data-ttu-id="df2e6-116">Date</span><span class="sxs-lookup"><span data-stu-id="df2e6-116">Date</span></span>    |
| <span data-ttu-id="df2e6-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="df2e6-117">fileCount</span></span>               | <span data-ttu-id="df2e6-118">Int64</span><span class="sxs-lookup"><span data-stu-id="df2e6-118">Int64</span></span>   |
| <span data-ttu-id="df2e6-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="df2e6-119">activeFileCount</span></span>         | <span data-ttu-id="df2e6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="df2e6-120">Int64</span></span>   |
| <span data-ttu-id="df2e6-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="df2e6-121">storageUsedInBytes</span></span>      | <span data-ttu-id="df2e6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="df2e6-122">Int64</span></span>   |
| <span data-ttu-id="df2e6-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="df2e6-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="df2e6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="df2e6-124">Int64</span></span>   |
| <span data-ttu-id="df2e6-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="df2e6-125">reportPeriod</span></span>            | <span data-ttu-id="df2e6-126">String</span><span class="sxs-lookup"><span data-stu-id="df2e6-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="df2e6-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df2e6-127">JSON representation</span></span>

<span data-ttu-id="df2e6-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df2e6-128">The following is a JSON representation of the resource.</span></span>

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
