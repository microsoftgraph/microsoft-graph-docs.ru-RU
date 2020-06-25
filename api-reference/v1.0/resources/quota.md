---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Назначаем
localization_priority: Normal
description: Ресурс quota предоставляет сведения об ограничениях дискового пространства в ресурсе Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 293daf950beb5cdf3cbd791a1e8bf0d4b92a220b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864212"
---
# <a name="quota-resource-type"></a><span data-ttu-id="a9e17-103">Тип ресурса quota</span><span class="sxs-lookup"><span data-stu-id="a9e17-103">Quota resource type</span></span>

<span data-ttu-id="a9e17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9e17-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9e17-105">Ресурс **quota** предоставляет сведения об ограничениях дискового пространства в ресурсе [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="a9e17-105">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9e17-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9e17-106">JSON representation</span></span>

<span data-ttu-id="a9e17-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9e17-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="a9e17-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9e17-108">Properties</span></span>

| <span data-ttu-id="a9e17-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a9e17-109">Property name</span></span> | <span data-ttu-id="a9e17-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a9e17-110">Type</span></span>   | <span data-ttu-id="a9e17-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a9e17-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="a9e17-112">total</span><span class="sxs-lookup"><span data-stu-id="a9e17-112">total</span></span>         | <span data-ttu-id="a9e17-113">Int64</span><span class="sxs-lookup"><span data-stu-id="a9e17-113">Int64</span></span>  | <span data-ttu-id="a9e17-114">Total allowed storage space, in bytes.</span><span class="sxs-lookup"><span data-stu-id="a9e17-114">Total allowed storage space, in bytes.</span></span> <span data-ttu-id="a9e17-115">Read-only.</span><span class="sxs-lookup"><span data-stu-id="a9e17-115">Read-only.</span></span>                           |
| <span data-ttu-id="a9e17-116">used</span><span class="sxs-lookup"><span data-stu-id="a9e17-116">used</span></span>          | <span data-ttu-id="a9e17-117">Int64</span><span class="sxs-lookup"><span data-stu-id="a9e17-117">Int64</span></span>  | <span data-ttu-id="a9e17-118">Total space used, in bytes.</span><span class="sxs-lookup"><span data-stu-id="a9e17-118">Total space used, in bytes.</span></span> <span data-ttu-id="a9e17-119">Read-only.</span><span class="sxs-lookup"><span data-stu-id="a9e17-119">Read-only.</span></span>                                      |
| <span data-ttu-id="a9e17-120">remaining</span><span class="sxs-lookup"><span data-stu-id="a9e17-120">remaining</span></span>     | <span data-ttu-id="a9e17-121">Int64</span><span class="sxs-lookup"><span data-stu-id="a9e17-121">Int64</span></span>  | <span data-ttu-id="a9e17-122">Total space remaining before reaching the quota limit, in bytes.</span><span class="sxs-lookup"><span data-stu-id="a9e17-122">Total space remaining before reaching the quota limit, in bytes.</span></span> <span data-ttu-id="a9e17-123">Read-only.</span><span class="sxs-lookup"><span data-stu-id="a9e17-123">Read-only.</span></span> |
| <span data-ttu-id="a9e17-124">deleted</span><span class="sxs-lookup"><span data-stu-id="a9e17-124">deleted</span></span>       | <span data-ttu-id="a9e17-125">Int64</span><span class="sxs-lookup"><span data-stu-id="a9e17-125">Int64</span></span>  | <span data-ttu-id="a9e17-126">Total space consumed by files in the recycle bin, in bytes.</span><span class="sxs-lookup"><span data-stu-id="a9e17-126">Total space consumed by files in the recycle bin, in bytes.</span></span> <span data-ttu-id="a9e17-127">Read-only.</span><span class="sxs-lookup"><span data-stu-id="a9e17-127">Read-only.</span></span>      |
| <span data-ttu-id="a9e17-128">состояние</span><span class="sxs-lookup"><span data-stu-id="a9e17-128">state</span></span>         | <span data-ttu-id="a9e17-129">string</span><span class="sxs-lookup"><span data-stu-id="a9e17-129">string</span></span> | <span data-ttu-id="a9e17-130">Enumeration value that indicates the state of the storage space.</span><span class="sxs-lookup"><span data-stu-id="a9e17-130">Enumeration value that indicates the state of the storage space.</span></span> <span data-ttu-id="a9e17-131">Read-only.</span><span class="sxs-lookup"><span data-stu-id="a9e17-131">Read-only.</span></span> |
| <span data-ttu-id="a9e17-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="a9e17-132">storagePlanInformation</span></span>  | [<span data-ttu-id="a9e17-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="a9e17-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="a9e17-134">Сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="a9e17-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="a9e17-135">Только в личном хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a9e17-135">Only in Personal OneDrive.</span></span>|

## <a name="state-enumeration"></a><span data-ttu-id="a9e17-136">Перечисление state</span><span class="sxs-lookup"><span data-stu-id="a9e17-136">State Enumeration</span></span>

| <span data-ttu-id="a9e17-137">Значение</span><span class="sxs-lookup"><span data-stu-id="a9e17-137">Value</span></span>      | <span data-ttu-id="a9e17-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a9e17-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="a9e17-139">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="a9e17-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="a9e17-140">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="a9e17-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="a9e17-141">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="a9e17-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="a9e17-142">The used quota has exceeded the total quota.</span><span class="sxs-lookup"><span data-stu-id="a9e17-142">The used quota has exceeded the total quota.</span></span> <span data-ttu-id="a9e17-143">New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span><span class="sxs-lookup"><span data-stu-id="a9e17-143">New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
