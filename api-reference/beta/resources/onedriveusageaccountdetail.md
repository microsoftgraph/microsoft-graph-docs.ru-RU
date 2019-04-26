---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563548"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="25317-103">Тип ресурса Онедривеусажеаккаунтдетаил</span><span class="sxs-lookup"><span data-stu-id="25317-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="25317-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="25317-104">Properties</span></span>

| <span data-ttu-id="25317-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="25317-105">Property</span></span>                | <span data-ttu-id="25317-106">Тип</span><span class="sxs-lookup"><span data-stu-id="25317-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="25317-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="25317-107">reportRefreshDate</span></span>       | <span data-ttu-id="25317-108">Дата</span><span class="sxs-lookup"><span data-stu-id="25317-108">Date</span></span>    |
| <span data-ttu-id="25317-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="25317-109">siteUrl</span></span>                 | <span data-ttu-id="25317-110">String</span><span class="sxs-lookup"><span data-stu-id="25317-110">String</span></span>  |
| <span data-ttu-id="25317-111">Овнердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="25317-111">ownerDisplayName</span></span>        | <span data-ttu-id="25317-112">String</span><span class="sxs-lookup"><span data-stu-id="25317-112">String</span></span>  |
| <span data-ttu-id="25317-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="25317-113">isDeleted</span></span>               | <span data-ttu-id="25317-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="25317-114">Boolean</span></span> |
| <span data-ttu-id="25317-115">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="25317-115">lastActivityDate</span></span>        | <span data-ttu-id="25317-116">Дата</span><span class="sxs-lookup"><span data-stu-id="25317-116">Date</span></span>    |
| <span data-ttu-id="25317-117">Филекаунт</span><span class="sxs-lookup"><span data-stu-id="25317-117">fileCount</span></span>               | <span data-ttu-id="25317-118">Int64</span><span class="sxs-lookup"><span data-stu-id="25317-118">Int64</span></span>   |
| <span data-ttu-id="25317-119">Активефилекаунт</span><span class="sxs-lookup"><span data-stu-id="25317-119">activeFileCount</span></span>         | <span data-ttu-id="25317-120">Int64</span><span class="sxs-lookup"><span data-stu-id="25317-120">Int64</span></span>   |
| <span data-ttu-id="25317-121">Сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="25317-121">storageUsedInBytes</span></span>      | <span data-ttu-id="25317-122">Int64</span><span class="sxs-lookup"><span data-stu-id="25317-122">Int64</span></span>   |
| <span data-ttu-id="25317-123">Сторажеаллокатединбитес</span><span class="sxs-lookup"><span data-stu-id="25317-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="25317-124">Int64</span><span class="sxs-lookup"><span data-stu-id="25317-124">Int64</span></span>   |
| <span data-ttu-id="25317-125">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="25317-125">reportPeriod</span></span>            | <span data-ttu-id="25317-126">String</span><span class="sxs-lookup"><span data-stu-id="25317-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="25317-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25317-127">JSON representation</span></span>

<span data-ttu-id="25317-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25317-128">The following is a JSON representation of the resource.</span></span>

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
