---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: quota
localization_priority: Normal
ms.openlocfilehash: a63b41253569dbb3d666a76b0a7495839ef61b12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882413"
---
# <a name="quota-resource-type"></a><span data-ttu-id="c4d15-102">Тип ресурса квот</span><span class="sxs-lookup"><span data-stu-id="c4d15-102">quota resource type</span></span>

> <span data-ttu-id="c4d15-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c4d15-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4d15-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4d15-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4d15-105">**Квота** ресурсов предоставляет подробные сведения о пространстве ограничивает от ресурса [диска](drive.md) .</span><span class="sxs-lookup"><span data-stu-id="c4d15-105">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4d15-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4d15-106">JSON representation</span></span>

<span data-ttu-id="c4d15-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4d15-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c4d15-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4d15-108">Properties</span></span>

| <span data-ttu-id="c4d15-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c4d15-109">Property name</span></span> | <span data-ttu-id="c4d15-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c4d15-110">Type</span></span>   | <span data-ttu-id="c4d15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c4d15-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="c4d15-112">total</span><span class="sxs-lookup"><span data-stu-id="c4d15-112">total</span></span>         | <span data-ttu-id="c4d15-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c4d15-113">Int64</span></span>  | <span data-ttu-id="c4d15-p102">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4d15-p102">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="c4d15-116">used</span><span class="sxs-lookup"><span data-stu-id="c4d15-116">used</span></span>          | <span data-ttu-id="c4d15-117">Int64</span><span class="sxs-lookup"><span data-stu-id="c4d15-117">Int64</span></span>  | <span data-ttu-id="c4d15-p103">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4d15-p103">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="c4d15-120">remaining</span><span class="sxs-lookup"><span data-stu-id="c4d15-120">remaining</span></span>     | <span data-ttu-id="c4d15-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c4d15-121">Int64</span></span>  | <span data-ttu-id="c4d15-p104">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4d15-p104">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="c4d15-124">deleted</span><span class="sxs-lookup"><span data-stu-id="c4d15-124">deleted</span></span>       | <span data-ttu-id="c4d15-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c4d15-125">Int64</span></span>  | <span data-ttu-id="c4d15-p105">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4d15-p105">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="c4d15-128">state</span><span class="sxs-lookup"><span data-stu-id="c4d15-128">state</span></span>         | <span data-ttu-id="c4d15-129">string</span><span class="sxs-lookup"><span data-stu-id="c4d15-129">string</span></span> | <span data-ttu-id="c4d15-p106">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4d15-p106">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="c4d15-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="c4d15-132">storagePlanInformation</span></span>  | [<span data-ttu-id="c4d15-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="c4d15-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="c4d15-134">Сведения о планах квоты хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="c4d15-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="c4d15-135">Только в личных OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c4d15-135">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="c4d15-136">Значения состояний перечисления</span><span class="sxs-lookup"><span data-stu-id="c4d15-136">State enumeration values</span></span>

| <span data-ttu-id="c4d15-137">Значение</span><span class="sxs-lookup"><span data-stu-id="c4d15-137">Value</span></span>      | <span data-ttu-id="c4d15-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c4d15-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="c4d15-139">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="c4d15-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="c4d15-140">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="c4d15-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="c4d15-141">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="c4d15-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="c4d15-p108">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="c4d15-p108">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota"
} -->
