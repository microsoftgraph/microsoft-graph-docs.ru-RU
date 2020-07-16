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
# <a name="quota-resource-type"></a><span data-ttu-id="cc205-103">Тип ресурса quota</span><span class="sxs-lookup"><span data-stu-id="cc205-103">Quota resource type</span></span>

<span data-ttu-id="cc205-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc205-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc205-105">Ресурс **quota** предоставляет сведения об ограничениях дискового пространства в ресурсе [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="cc205-105">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc205-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc205-106">JSON representation</span></span>

<span data-ttu-id="cc205-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc205-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cc205-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc205-108">Properties</span></span>

| <span data-ttu-id="cc205-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="cc205-109">Property name</span></span> | <span data-ttu-id="cc205-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cc205-110">Type</span></span>   | <span data-ttu-id="cc205-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc205-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="cc205-112">total</span><span class="sxs-lookup"><span data-stu-id="cc205-112">total</span></span>         | <span data-ttu-id="cc205-113">Int64</span><span class="sxs-lookup"><span data-stu-id="cc205-113">Int64</span></span>  | <span data-ttu-id="cc205-p101">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc205-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="cc205-116">used</span><span class="sxs-lookup"><span data-stu-id="cc205-116">used</span></span>          | <span data-ttu-id="cc205-117">Int64</span><span class="sxs-lookup"><span data-stu-id="cc205-117">Int64</span></span>  | <span data-ttu-id="cc205-p102">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc205-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="cc205-120">remaining</span><span class="sxs-lookup"><span data-stu-id="cc205-120">remaining</span></span>     | <span data-ttu-id="cc205-121">Int64</span><span class="sxs-lookup"><span data-stu-id="cc205-121">Int64</span></span>  | <span data-ttu-id="cc205-p103">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc205-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="cc205-124">deleted</span><span class="sxs-lookup"><span data-stu-id="cc205-124">deleted</span></span>       | <span data-ttu-id="cc205-125">Int64</span><span class="sxs-lookup"><span data-stu-id="cc205-125">Int64</span></span>  | <span data-ttu-id="cc205-p104">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc205-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="cc205-128">состояние</span><span class="sxs-lookup"><span data-stu-id="cc205-128">state</span></span>         | <span data-ttu-id="cc205-129">string</span><span class="sxs-lookup"><span data-stu-id="cc205-129">string</span></span> | <span data-ttu-id="cc205-p105">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc205-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="cc205-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="cc205-132">storagePlanInformation</span></span>  | [<span data-ttu-id="cc205-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="cc205-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="cc205-134">Сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="cc205-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="cc205-135">Только в личном хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cc205-135">Only in Personal OneDrive.</span></span>|

## <a name="state-enumeration"></a><span data-ttu-id="cc205-136">Перечисление state</span><span class="sxs-lookup"><span data-stu-id="cc205-136">State Enumeration</span></span>

| <span data-ttu-id="cc205-137">Значение</span><span class="sxs-lookup"><span data-stu-id="cc205-137">Value</span></span>      | <span data-ttu-id="cc205-138">Описание</span><span class="sxs-lookup"><span data-stu-id="cc205-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="cc205-139">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="cc205-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="cc205-140">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="cc205-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="cc205-141">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="cc205-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="cc205-p107">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="cc205-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
