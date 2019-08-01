---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Назначаем
localization_priority: Normal
description: Ресурс quota предоставляет сведения об ограничениях дискового пространства в ресурсе Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ee93ddfe54e785ea8a8fa245ab3828c548928cc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034960"
---
# <a name="quota-resource-type"></a><span data-ttu-id="7f1bb-103">Тип ресурса quota</span><span class="sxs-lookup"><span data-stu-id="7f1bb-103">Quota resource type</span></span>

<span data-ttu-id="7f1bb-104">Ресурс **quota** предоставляет сведения об ограничениях дискового пространства в ресурсе [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="7f1bb-104">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f1bb-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f1bb-105">JSON representation</span></span>

<span data-ttu-id="7f1bb-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-106">Here is a JSON representation of the resource.</span></span>

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
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="7f1bb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f1bb-107">Properties</span></span>

| <span data-ttu-id="7f1bb-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7f1bb-108">Property name</span></span> | <span data-ttu-id="7f1bb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7f1bb-109">Type</span></span>   | <span data-ttu-id="7f1bb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f1bb-110">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="7f1bb-111">total</span><span class="sxs-lookup"><span data-stu-id="7f1bb-111">total</span></span>         | <span data-ttu-id="7f1bb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7f1bb-112">Int64</span></span>  | <span data-ttu-id="7f1bb-p101">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="7f1bb-115">used</span><span class="sxs-lookup"><span data-stu-id="7f1bb-115">used</span></span>          | <span data-ttu-id="7f1bb-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7f1bb-116">Int64</span></span>  | <span data-ttu-id="7f1bb-p102">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="7f1bb-119">remaining</span><span class="sxs-lookup"><span data-stu-id="7f1bb-119">remaining</span></span>     | <span data-ttu-id="7f1bb-120">Int64</span><span class="sxs-lookup"><span data-stu-id="7f1bb-120">Int64</span></span>  | <span data-ttu-id="7f1bb-p103">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="7f1bb-123">deleted</span><span class="sxs-lookup"><span data-stu-id="7f1bb-123">deleted</span></span>       | <span data-ttu-id="7f1bb-124">Int64</span><span class="sxs-lookup"><span data-stu-id="7f1bb-124">Int64</span></span>  | <span data-ttu-id="7f1bb-p104">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="7f1bb-127">состояние</span><span class="sxs-lookup"><span data-stu-id="7f1bb-127">state</span></span>         | <span data-ttu-id="7f1bb-128">string</span><span class="sxs-lookup"><span data-stu-id="7f1bb-128">string</span></span> | <span data-ttu-id="7f1bb-p105">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="7f1bb-131">Перечисление state</span><span class="sxs-lookup"><span data-stu-id="7f1bb-131">State Enumeration</span></span>

| <span data-ttu-id="7f1bb-132">Значение</span><span class="sxs-lookup"><span data-stu-id="7f1bb-132">Value</span></span>      | <span data-ttu-id="7f1bb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7f1bb-133">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="7f1bb-134">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-134">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="7f1bb-135">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-135">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="7f1bb-136">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-136">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="7f1bb-p106">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="7f1bb-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
