---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 21bc509fd2364365e29d1e35bcbe78d67fdc40c8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522381"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="9ddde-103">Тип ресурса Онедривеусажеаккаунтдетаил</span><span class="sxs-lookup"><span data-stu-id="9ddde-103">oneDriveUsageAccountDetail resource type</span></span>

<span data-ttu-id="9ddde-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ddde-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="9ddde-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ddde-105">Properties</span></span>

| <span data-ttu-id="9ddde-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ddde-106">Property</span></span>                | <span data-ttu-id="9ddde-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9ddde-107">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="9ddde-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="9ddde-108">reportRefreshDate</span></span>       | <span data-ttu-id="9ddde-109">Дата</span><span class="sxs-lookup"><span data-stu-id="9ddde-109">Date</span></span>    |
| <span data-ttu-id="9ddde-110">siteUrl</span><span class="sxs-lookup"><span data-stu-id="9ddde-110">siteUrl</span></span>                 | <span data-ttu-id="9ddde-111">String</span><span class="sxs-lookup"><span data-stu-id="9ddde-111">String</span></span>  |
| <span data-ttu-id="9ddde-112">овнердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="9ddde-112">ownerDisplayName</span></span>        | <span data-ttu-id="9ddde-113">String</span><span class="sxs-lookup"><span data-stu-id="9ddde-113">String</span></span>  |
| <span data-ttu-id="9ddde-114">овнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="9ddde-114">ownerPrincipalName</span></span>      | <span data-ttu-id="9ddde-115">String</span><span class="sxs-lookup"><span data-stu-id="9ddde-115">String</span></span>  |
| <span data-ttu-id="9ddde-116">isDeleted</span><span class="sxs-lookup"><span data-stu-id="9ddde-116">isDeleted</span></span>               | <span data-ttu-id="9ddde-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ddde-117">Boolean</span></span> |
| <span data-ttu-id="9ddde-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="9ddde-118">lastActivityDate</span></span>        | <span data-ttu-id="9ddde-119">Дата</span><span class="sxs-lookup"><span data-stu-id="9ddde-119">Date</span></span>    |
| <span data-ttu-id="9ddde-120">филекаунт</span><span class="sxs-lookup"><span data-stu-id="9ddde-120">fileCount</span></span>               | <span data-ttu-id="9ddde-121">Int64</span><span class="sxs-lookup"><span data-stu-id="9ddde-121">Int64</span></span>   |
| <span data-ttu-id="9ddde-122">активефилекаунт</span><span class="sxs-lookup"><span data-stu-id="9ddde-122">activeFileCount</span></span>         | <span data-ttu-id="9ddde-123">Int64</span><span class="sxs-lookup"><span data-stu-id="9ddde-123">Int64</span></span>   |
| <span data-ttu-id="9ddde-124">сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="9ddde-124">storageUsedInBytes</span></span>      | <span data-ttu-id="9ddde-125">Int64</span><span class="sxs-lookup"><span data-stu-id="9ddde-125">Int64</span></span>   |
| <span data-ttu-id="9ddde-126">сторажеаллокатединбитес</span><span class="sxs-lookup"><span data-stu-id="9ddde-126">storageAllocatedInBytes</span></span> | <span data-ttu-id="9ddde-127">Int64</span><span class="sxs-lookup"><span data-stu-id="9ddde-127">Int64</span></span>   |
| <span data-ttu-id="9ddde-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="9ddde-128">reportPeriod</span></span>            | <span data-ttu-id="9ddde-129">String</span><span class="sxs-lookup"><span data-stu-id="9ddde-129">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9ddde-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ddde-130">JSON representation</span></span>

<span data-ttu-id="9ddde-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ddde-131">The following is a JSON representation of the resource.</span></span>

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
