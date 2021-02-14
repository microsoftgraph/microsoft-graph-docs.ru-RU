---
author: JeremyKelley
ms.date: 09/10/2017
title: Quota
localization_priority: Normal
description: Ресурс quota предоставляет сведения об ограничениях дискового пространства в ресурсе Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 145d145e764128c719e757c213b8d7b2266e0b68
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238899"
---
# <a name="quota-resource-type"></a><span data-ttu-id="1c7a9-103">Тип ресурса quota</span><span class="sxs-lookup"><span data-stu-id="1c7a9-103">Quota resource type</span></span>

<span data-ttu-id="1c7a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c7a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c7a9-105">Ресурс **quota** предоставляет сведения об ограничениях дискового пространства в ресурсе [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="1c7a9-105">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c7a9-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c7a9-106">JSON representation</span></span>

<span data-ttu-id="1c7a9-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1c7a9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c7a9-108">Properties</span></span>

| <span data-ttu-id="1c7a9-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1c7a9-109">Property name</span></span> | <span data-ttu-id="1c7a9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1c7a9-110">Type</span></span>   | <span data-ttu-id="1c7a9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1c7a9-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="1c7a9-112">total</span><span class="sxs-lookup"><span data-stu-id="1c7a9-112">total</span></span>         | <span data-ttu-id="1c7a9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="1c7a9-113">Int64</span></span>  | <span data-ttu-id="1c7a9-p101">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="1c7a9-116">used</span><span class="sxs-lookup"><span data-stu-id="1c7a9-116">used</span></span>          | <span data-ttu-id="1c7a9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="1c7a9-117">Int64</span></span>  | <span data-ttu-id="1c7a9-p102">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="1c7a9-120">remaining</span><span class="sxs-lookup"><span data-stu-id="1c7a9-120">remaining</span></span>     | <span data-ttu-id="1c7a9-121">Int64</span><span class="sxs-lookup"><span data-stu-id="1c7a9-121">Int64</span></span>  | <span data-ttu-id="1c7a9-p103">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="1c7a9-124">deleted</span><span class="sxs-lookup"><span data-stu-id="1c7a9-124">deleted</span></span>       | <span data-ttu-id="1c7a9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="1c7a9-125">Int64</span></span>  | <span data-ttu-id="1c7a9-p104">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="1c7a9-128">состояние</span><span class="sxs-lookup"><span data-stu-id="1c7a9-128">state</span></span>         | <span data-ttu-id="1c7a9-129">string</span><span class="sxs-lookup"><span data-stu-id="1c7a9-129">string</span></span> | <span data-ttu-id="1c7a9-p105">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="1c7a9-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="1c7a9-132">storagePlanInformation</span></span>  | [<span data-ttu-id="1c7a9-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="1c7a9-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="1c7a9-134">Сведения о планах квот дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="1c7a9-135">Только в Личном хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-135">Only in Personal OneDrive.</span></span>|

## <a name="state-enumeration"></a><span data-ttu-id="1c7a9-136">Перечисление state</span><span class="sxs-lookup"><span data-stu-id="1c7a9-136">State Enumeration</span></span>

| <span data-ttu-id="1c7a9-137">Значение</span><span class="sxs-lookup"><span data-stu-id="1c7a9-137">Value</span></span>      | <span data-ttu-id="1c7a9-138">Описание</span><span class="sxs-lookup"><span data-stu-id="1c7a9-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="1c7a9-139">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="1c7a9-140">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="1c7a9-141">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="1c7a9-p107">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="1c7a9-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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

