---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 594339072c683b053ddeb637b6f401bae2aed322
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812073"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="abe0a-103">Тип ресурса Онедривеусажеаккаунтдетаил</span><span class="sxs-lookup"><span data-stu-id="abe0a-103">oneDriveUsageAccountDetail resource type</span></span>

<span data-ttu-id="abe0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abe0a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="abe0a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="abe0a-105">Properties</span></span>

| <span data-ttu-id="abe0a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="abe0a-106">Property</span></span>                | <span data-ttu-id="abe0a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="abe0a-107">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="abe0a-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="abe0a-108">reportRefreshDate</span></span>       | <span data-ttu-id="abe0a-109">Дата</span><span class="sxs-lookup"><span data-stu-id="abe0a-109">Date</span></span>    |
| <span data-ttu-id="abe0a-110">siteUrl</span><span class="sxs-lookup"><span data-stu-id="abe0a-110">siteUrl</span></span>                 | <span data-ttu-id="abe0a-111">String</span><span class="sxs-lookup"><span data-stu-id="abe0a-111">String</span></span>  |
| <span data-ttu-id="abe0a-112">овнердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="abe0a-112">ownerDisplayName</span></span>        | <span data-ttu-id="abe0a-113">String</span><span class="sxs-lookup"><span data-stu-id="abe0a-113">String</span></span>  |
| <span data-ttu-id="abe0a-114">овнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="abe0a-114">ownerPrincipalName</span></span>      | <span data-ttu-id="abe0a-115">String</span><span class="sxs-lookup"><span data-stu-id="abe0a-115">String</span></span>  |
| <span data-ttu-id="abe0a-116">isDeleted</span><span class="sxs-lookup"><span data-stu-id="abe0a-116">isDeleted</span></span>               | <span data-ttu-id="abe0a-117">Логический</span><span class="sxs-lookup"><span data-stu-id="abe0a-117">Boolean</span></span> |
| <span data-ttu-id="abe0a-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="abe0a-118">lastActivityDate</span></span>        | <span data-ttu-id="abe0a-119">Дата</span><span class="sxs-lookup"><span data-stu-id="abe0a-119">Date</span></span>    |
| <span data-ttu-id="abe0a-120">филекаунт</span><span class="sxs-lookup"><span data-stu-id="abe0a-120">fileCount</span></span>               | <span data-ttu-id="abe0a-121">Int64</span><span class="sxs-lookup"><span data-stu-id="abe0a-121">Int64</span></span>   |
| <span data-ttu-id="abe0a-122">активефилекаунт</span><span class="sxs-lookup"><span data-stu-id="abe0a-122">activeFileCount</span></span>         | <span data-ttu-id="abe0a-123">Int64</span><span class="sxs-lookup"><span data-stu-id="abe0a-123">Int64</span></span>   |
| <span data-ttu-id="abe0a-124">сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="abe0a-124">storageUsedInBytes</span></span>      | <span data-ttu-id="abe0a-125">Int64</span><span class="sxs-lookup"><span data-stu-id="abe0a-125">Int64</span></span>   |
| <span data-ttu-id="abe0a-126">сторажеаллокатединбитес</span><span class="sxs-lookup"><span data-stu-id="abe0a-126">storageAllocatedInBytes</span></span> | <span data-ttu-id="abe0a-127">Int64</span><span class="sxs-lookup"><span data-stu-id="abe0a-127">Int64</span></span>   |
| <span data-ttu-id="abe0a-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="abe0a-128">reportPeriod</span></span>            | <span data-ttu-id="abe0a-129">String</span><span class="sxs-lookup"><span data-stu-id="abe0a-129">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="abe0a-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="abe0a-130">JSON representation</span></span>

<span data-ttu-id="abe0a-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abe0a-131">The following is a JSON representation of the resource.</span></span>

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
