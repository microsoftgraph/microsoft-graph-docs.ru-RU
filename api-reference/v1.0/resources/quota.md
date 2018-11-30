---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: quota
ms.openlocfilehash: 54eb88bdc048c6b63bb6f2d0a23fb05023663ca7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025411"
---
# <a name="quota-resource-type"></a><span data-ttu-id="daa14-102">Тип ресурса quota</span><span class="sxs-lookup"><span data-stu-id="daa14-102">Quota resource type</span></span>

<span data-ttu-id="daa14-103">Ресурс **quota** предоставляет сведения об ограничениях дискового пространства в ресурсе [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="daa14-103">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="daa14-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="daa14-104">JSON representation</span></span>

<span data-ttu-id="daa14-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daa14-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="daa14-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="daa14-106">Properties</span></span>

| <span data-ttu-id="daa14-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="daa14-107">Property name</span></span> | <span data-ttu-id="daa14-108">Тип</span><span class="sxs-lookup"><span data-stu-id="daa14-108">Type</span></span>   | <span data-ttu-id="daa14-109">Описание</span><span class="sxs-lookup"><span data-stu-id="daa14-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="daa14-110">total</span><span class="sxs-lookup"><span data-stu-id="daa14-110">total</span></span>         | <span data-ttu-id="daa14-111">Int64</span><span class="sxs-lookup"><span data-stu-id="daa14-111">Int64</span></span>  | <span data-ttu-id="daa14-p101">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daa14-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="daa14-114">used</span><span class="sxs-lookup"><span data-stu-id="daa14-114">used</span></span>          | <span data-ttu-id="daa14-115">Int64</span><span class="sxs-lookup"><span data-stu-id="daa14-115">Int64</span></span>  | <span data-ttu-id="daa14-p102">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daa14-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="daa14-118">remaining</span><span class="sxs-lookup"><span data-stu-id="daa14-118">remaining</span></span>     | <span data-ttu-id="daa14-119">Int64</span><span class="sxs-lookup"><span data-stu-id="daa14-119">Int64</span></span>  | <span data-ttu-id="daa14-p103">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daa14-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="daa14-122">deleted</span><span class="sxs-lookup"><span data-stu-id="daa14-122">deleted</span></span>       | <span data-ttu-id="daa14-123">Int64</span><span class="sxs-lookup"><span data-stu-id="daa14-123">Int64</span></span>  | <span data-ttu-id="daa14-p104">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daa14-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="daa14-126">состояние</span><span class="sxs-lookup"><span data-stu-id="daa14-126">state</span></span>         | <span data-ttu-id="daa14-127">string</span><span class="sxs-lookup"><span data-stu-id="daa14-127">string</span></span> | <span data-ttu-id="daa14-p105">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="daa14-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="daa14-130">Перечисление state</span><span class="sxs-lookup"><span data-stu-id="daa14-130">State Enumeration</span></span>

| <span data-ttu-id="daa14-131">Значение</span><span class="sxs-lookup"><span data-stu-id="daa14-131">Value</span></span>      | <span data-ttu-id="daa14-132">Описание</span><span class="sxs-lookup"><span data-stu-id="daa14-132">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="daa14-133">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="daa14-133">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="daa14-134">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="daa14-134">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="daa14-135">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="daa14-135">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="daa14-p106">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="daa14-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
