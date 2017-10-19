---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: quota
ms.openlocfilehash: f786a2cf84b9553d2f36d0355a9c34a541243d81
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="quota-resource-type"></a><span data-ttu-id="c8f3b-102">Тип ресурса quota</span><span class="sxs-lookup"><span data-stu-id="c8f3b-102">Quota resource type</span></span>

<span data-ttu-id="c8f3b-103">Ресурс **quota** предоставляет сведения об ограничениях дискового пространства в ресурсе [Drive](drive.md).</span><span class="sxs-lookup"><span data-stu-id="c8f3b-103">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8f3b-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8f3b-104">JSON representation</span></span>

<span data-ttu-id="c8f3b-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c8f3b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8f3b-106">Properties</span></span>

| <span data-ttu-id="c8f3b-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c8f3b-107">Property name</span></span> | <span data-ttu-id="c8f3b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c8f3b-108">Type</span></span>   | <span data-ttu-id="c8f3b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c8f3b-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="c8f3b-110">total</span><span class="sxs-lookup"><span data-stu-id="c8f3b-110">total</span></span>         | <span data-ttu-id="c8f3b-111">Int64</span><span class="sxs-lookup"><span data-stu-id="c8f3b-111">Int64</span></span>  | <span data-ttu-id="c8f3b-p101">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="c8f3b-114">used</span><span class="sxs-lookup"><span data-stu-id="c8f3b-114">used</span></span>          | <span data-ttu-id="c8f3b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c8f3b-115">Int64</span></span>  | <span data-ttu-id="c8f3b-p102">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="c8f3b-118">remaining</span><span class="sxs-lookup"><span data-stu-id="c8f3b-118">remaining</span></span>     | <span data-ttu-id="c8f3b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c8f3b-119">Int64</span></span>  | <span data-ttu-id="c8f3b-p103">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="c8f3b-122">deleted</span><span class="sxs-lookup"><span data-stu-id="c8f3b-122">deleted</span></span>       | <span data-ttu-id="c8f3b-123">Int64</span><span class="sxs-lookup"><span data-stu-id="c8f3b-123">Int64</span></span>  | <span data-ttu-id="c8f3b-p104">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="c8f3b-126">состояние</span><span class="sxs-lookup"><span data-stu-id="c8f3b-126">state</span></span>         | <span data-ttu-id="c8f3b-127">string</span><span class="sxs-lookup"><span data-stu-id="c8f3b-127">string</span></span> | <span data-ttu-id="c8f3b-p105">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="c8f3b-130">Перечисление state</span><span class="sxs-lookup"><span data-stu-id="c8f3b-130">State Enumeration</span></span>

| <span data-ttu-id="c8f3b-131">Значение</span><span class="sxs-lookup"><span data-stu-id="c8f3b-131">Value</span></span>      | <span data-ttu-id="c8f3b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8f3b-132">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="c8f3b-133">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-133">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="c8f3b-134">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-134">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="c8f3b-135">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-135">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="c8f3b-p106">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="c8f3b-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota"
} -->
