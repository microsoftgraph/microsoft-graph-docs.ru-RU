---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bcf75fad8c39a543e69fc378546a2621f24eaeab
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344929"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="79887-103">Тип ресурса Онедривеусажеаккаунтдетаил</span><span class="sxs-lookup"><span data-stu-id="79887-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="79887-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="79887-104">Properties</span></span>

| <span data-ttu-id="79887-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="79887-105">Property</span></span>                | <span data-ttu-id="79887-106">Тип</span><span class="sxs-lookup"><span data-stu-id="79887-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="79887-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="79887-107">reportRefreshDate</span></span>       | <span data-ttu-id="79887-108">Дата</span><span class="sxs-lookup"><span data-stu-id="79887-108">Date</span></span>    |
| <span data-ttu-id="79887-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="79887-109">siteUrl</span></span>                 | <span data-ttu-id="79887-110">String</span><span class="sxs-lookup"><span data-stu-id="79887-110">String</span></span>  |
| <span data-ttu-id="79887-111">Овнердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="79887-111">ownerDisplayName</span></span>        | <span data-ttu-id="79887-112">String</span><span class="sxs-lookup"><span data-stu-id="79887-112">String</span></span>  |
| <span data-ttu-id="79887-113">ОвнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="79887-113">ownerPrincipalName</span></span>      | <span data-ttu-id="79887-114">String</span><span class="sxs-lookup"><span data-stu-id="79887-114">String</span></span>  |
| <span data-ttu-id="79887-115">isDeleted</span><span class="sxs-lookup"><span data-stu-id="79887-115">isDeleted</span></span>               | <span data-ttu-id="79887-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="79887-116">Boolean</span></span> |
| <span data-ttu-id="79887-117">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="79887-117">lastActivityDate</span></span>        | <span data-ttu-id="79887-118">Дата</span><span class="sxs-lookup"><span data-stu-id="79887-118">Date</span></span>    |
| <span data-ttu-id="79887-119">Филекаунт</span><span class="sxs-lookup"><span data-stu-id="79887-119">fileCount</span></span>               | <span data-ttu-id="79887-120">Int64</span><span class="sxs-lookup"><span data-stu-id="79887-120">Int64</span></span>   |
| <span data-ttu-id="79887-121">Активефилекаунт</span><span class="sxs-lookup"><span data-stu-id="79887-121">activeFileCount</span></span>         | <span data-ttu-id="79887-122">Int64</span><span class="sxs-lookup"><span data-stu-id="79887-122">Int64</span></span>   |
| <span data-ttu-id="79887-123">Сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="79887-123">storageUsedInBytes</span></span>      | <span data-ttu-id="79887-124">Int64</span><span class="sxs-lookup"><span data-stu-id="79887-124">Int64</span></span>   |
| <span data-ttu-id="79887-125">Сторажеаллокатединбитес</span><span class="sxs-lookup"><span data-stu-id="79887-125">storageAllocatedInBytes</span></span> | <span data-ttu-id="79887-126">Int64</span><span class="sxs-lookup"><span data-stu-id="79887-126">Int64</span></span>   |
| <span data-ttu-id="79887-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="79887-127">reportPeriod</span></span>            | <span data-ttu-id="79887-128">String</span><span class="sxs-lookup"><span data-stu-id="79887-128">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="79887-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79887-129">JSON representation</span></span>

<span data-ttu-id="79887-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79887-130">The following is a JSON representation of the resource.</span></span>

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
