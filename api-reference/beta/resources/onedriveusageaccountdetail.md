---
title: Тип ресурса oneDriveUsageAccountDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957398"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="00aa0-103">Тип ресурса oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="00aa0-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="00aa0-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="00aa0-104">Properties</span></span>

| <span data-ttu-id="00aa0-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="00aa0-105">Property</span></span>                | <span data-ttu-id="00aa0-106">Тип</span><span class="sxs-lookup"><span data-stu-id="00aa0-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="00aa0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="00aa0-107">reportRefreshDate</span></span>       | <span data-ttu-id="00aa0-108">Date</span><span class="sxs-lookup"><span data-stu-id="00aa0-108">Date</span></span>    |
| <span data-ttu-id="00aa0-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="00aa0-109">siteUrl</span></span>                 | <span data-ttu-id="00aa0-110">String</span><span class="sxs-lookup"><span data-stu-id="00aa0-110">String</span></span>  |
| <span data-ttu-id="00aa0-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="00aa0-111">ownerDisplayName</span></span>        | <span data-ttu-id="00aa0-112">String</span><span class="sxs-lookup"><span data-stu-id="00aa0-112">String</span></span>  |
| <span data-ttu-id="00aa0-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="00aa0-113">isDeleted</span></span>               | <span data-ttu-id="00aa0-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="00aa0-114">Boolean</span></span> |
| <span data-ttu-id="00aa0-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="00aa0-115">lastActivityDate</span></span>        | <span data-ttu-id="00aa0-116">Date</span><span class="sxs-lookup"><span data-stu-id="00aa0-116">Date</span></span>    |
| <span data-ttu-id="00aa0-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="00aa0-117">fileCount</span></span>               | <span data-ttu-id="00aa0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="00aa0-118">Int64</span></span>   |
| <span data-ttu-id="00aa0-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="00aa0-119">activeFileCount</span></span>         | <span data-ttu-id="00aa0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="00aa0-120">Int64</span></span>   |
| <span data-ttu-id="00aa0-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="00aa0-121">storageUsedInBytes</span></span>      | <span data-ttu-id="00aa0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="00aa0-122">Int64</span></span>   |
| <span data-ttu-id="00aa0-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="00aa0-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="00aa0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="00aa0-124">Int64</span></span>   |
| <span data-ttu-id="00aa0-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="00aa0-125">reportPeriod</span></span>            | <span data-ttu-id="00aa0-126">String</span><span class="sxs-lookup"><span data-stu-id="00aa0-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="00aa0-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00aa0-127">JSON representation</span></span>

<span data-ttu-id="00aa0-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00aa0-128">The following is a JSON representation of the resource.</span></span>

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
