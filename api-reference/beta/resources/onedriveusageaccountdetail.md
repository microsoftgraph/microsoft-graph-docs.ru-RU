---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: cc80110a2f8f755ef984b2f993ea660798a86743
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966470"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="c2093-103">Тип ресурса Онедривеусажеаккаунтдетаил</span><span class="sxs-lookup"><span data-stu-id="c2093-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c2093-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2093-104">Properties</span></span>

| <span data-ttu-id="c2093-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2093-105">Property</span></span>                | <span data-ttu-id="c2093-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c2093-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="c2093-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c2093-107">reportRefreshDate</span></span>       | <span data-ttu-id="c2093-108">Дата</span><span class="sxs-lookup"><span data-stu-id="c2093-108">Date</span></span>    |
| <span data-ttu-id="c2093-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="c2093-109">siteUrl</span></span>                 | <span data-ttu-id="c2093-110">String</span><span class="sxs-lookup"><span data-stu-id="c2093-110">String</span></span>  |
| <span data-ttu-id="c2093-111">Овнердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="c2093-111">ownerDisplayName</span></span>        | <span data-ttu-id="c2093-112">String</span><span class="sxs-lookup"><span data-stu-id="c2093-112">String</span></span>  |
| <span data-ttu-id="c2093-113">ОвнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="c2093-113">ownerPrincipalName</span></span>      | <span data-ttu-id="c2093-114">String</span><span class="sxs-lookup"><span data-stu-id="c2093-114">String</span></span>  |
| <span data-ttu-id="c2093-115">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c2093-115">isDeleted</span></span>               | <span data-ttu-id="c2093-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2093-116">Boolean</span></span> |
| <span data-ttu-id="c2093-117">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="c2093-117">lastActivityDate</span></span>        | <span data-ttu-id="c2093-118">Дата</span><span class="sxs-lookup"><span data-stu-id="c2093-118">Date</span></span>    |
| <span data-ttu-id="c2093-119">Филекаунт</span><span class="sxs-lookup"><span data-stu-id="c2093-119">fileCount</span></span>               | <span data-ttu-id="c2093-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c2093-120">Int64</span></span>   |
| <span data-ttu-id="c2093-121">Активефилекаунт</span><span class="sxs-lookup"><span data-stu-id="c2093-121">activeFileCount</span></span>         | <span data-ttu-id="c2093-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c2093-122">Int64</span></span>   |
| <span data-ttu-id="c2093-123">Сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="c2093-123">storageUsedInBytes</span></span>      | <span data-ttu-id="c2093-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c2093-124">Int64</span></span>   |
| <span data-ttu-id="c2093-125">Сторажеаллокатединбитес</span><span class="sxs-lookup"><span data-stu-id="c2093-125">storageAllocatedInBytes</span></span> | <span data-ttu-id="c2093-126">Int64</span><span class="sxs-lookup"><span data-stu-id="c2093-126">Int64</span></span>   |
| <span data-ttu-id="c2093-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="c2093-127">reportPeriod</span></span>            | <span data-ttu-id="c2093-128">String</span><span class="sxs-lookup"><span data-stu-id="c2093-128">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c2093-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2093-129">JSON representation</span></span>

<span data-ttu-id="c2093-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2093-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "ownerPrincipalName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
