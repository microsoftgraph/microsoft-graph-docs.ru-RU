---
author: JeremyKelley
description: Ресурс Quota предоставляет сведения об ограничениях дискового пространства для ресурса Drive.
ms.date: 09/10/2017
title: Назначаем
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 83e842872694a1f708bf37ab800fa73673255647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008798"
---
# <a name="quota-resource-type"></a><span data-ttu-id="cb025-103">Тип ресурса Quota</span><span class="sxs-lookup"><span data-stu-id="cb025-103">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb025-104">Ресурс **Quota** предоставляет сведения об ограничениях дискового пространства для ресурса [Drive](drive.md) .</span><span class="sxs-lookup"><span data-stu-id="cb025-104">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb025-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb025-105">JSON representation</span></span>

<span data-ttu-id="cb025-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb025-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cb025-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb025-107">Properties</span></span>

| <span data-ttu-id="cb025-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="cb025-108">Property name</span></span> | <span data-ttu-id="cb025-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cb025-109">Type</span></span>   | <span data-ttu-id="cb025-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cb025-110">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="cb025-111">total</span><span class="sxs-lookup"><span data-stu-id="cb025-111">total</span></span>         | <span data-ttu-id="cb025-112">Int64</span><span class="sxs-lookup"><span data-stu-id="cb025-112">Int64</span></span>  | <span data-ttu-id="cb025-p101">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb025-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="cb025-115">used</span><span class="sxs-lookup"><span data-stu-id="cb025-115">used</span></span>          | <span data-ttu-id="cb025-116">Int64</span><span class="sxs-lookup"><span data-stu-id="cb025-116">Int64</span></span>  | <span data-ttu-id="cb025-p102">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb025-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="cb025-119">remaining</span><span class="sxs-lookup"><span data-stu-id="cb025-119">remaining</span></span>     | <span data-ttu-id="cb025-120">Int64</span><span class="sxs-lookup"><span data-stu-id="cb025-120">Int64</span></span>  | <span data-ttu-id="cb025-p103">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb025-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="cb025-123">deleted</span><span class="sxs-lookup"><span data-stu-id="cb025-123">deleted</span></span>       | <span data-ttu-id="cb025-124">Int64</span><span class="sxs-lookup"><span data-stu-id="cb025-124">Int64</span></span>  | <span data-ttu-id="cb025-p104">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb025-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="cb025-127">состояние</span><span class="sxs-lookup"><span data-stu-id="cb025-127">state</span></span>         | <span data-ttu-id="cb025-128">string</span><span class="sxs-lookup"><span data-stu-id="cb025-128">string</span></span> | <span data-ttu-id="cb025-p105">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb025-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="cb025-131">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="cb025-131">storagePlanInformation</span></span>  | [<span data-ttu-id="cb025-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="cb025-132">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="cb025-133">Сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="cb025-133">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="cb025-134">Только в личном хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cb025-134">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="cb025-135">Значения перечисления State</span><span class="sxs-lookup"><span data-stu-id="cb025-135">State enumeration values</span></span>

| <span data-ttu-id="cb025-136">Значение</span><span class="sxs-lookup"><span data-stu-id="cb025-136">Value</span></span>      | <span data-ttu-id="cb025-137">Описание</span><span class="sxs-lookup"><span data-stu-id="cb025-137">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="cb025-138">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="cb025-138">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="cb025-139">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="cb025-139">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="cb025-140">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="cb025-140">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="cb025-p107">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="cb025-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": []
}
-->
