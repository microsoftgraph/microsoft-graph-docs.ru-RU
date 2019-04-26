---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Назначаем
localization_priority: Normal
ms.openlocfilehash: 7cafff3162c7cdc4435df1cde522b42998398693
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563376"
---
# <a name="quota-resource-type"></a><span data-ttu-id="44a8f-102">Тип ресурса Quota</span><span class="sxs-lookup"><span data-stu-id="44a8f-102">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44a8f-103">Ресурс **Quota** предоставляет сведения об ограничениях дискового пространства для ресурса [Drive](drive.md) .</span><span class="sxs-lookup"><span data-stu-id="44a8f-103">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44a8f-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44a8f-104">JSON representation</span></span>

<span data-ttu-id="44a8f-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44a8f-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="44a8f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="44a8f-106">Properties</span></span>

| <span data-ttu-id="44a8f-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="44a8f-107">Property name</span></span> | <span data-ttu-id="44a8f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="44a8f-108">Type</span></span>   | <span data-ttu-id="44a8f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="44a8f-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="44a8f-110">total</span><span class="sxs-lookup"><span data-stu-id="44a8f-110">total</span></span>         | <span data-ttu-id="44a8f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="44a8f-111">Int64</span></span>  | <span data-ttu-id="44a8f-p101">Общий объем разрешенного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44a8f-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="44a8f-114">used</span><span class="sxs-lookup"><span data-stu-id="44a8f-114">used</span></span>          | <span data-ttu-id="44a8f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="44a8f-115">Int64</span></span>  | <span data-ttu-id="44a8f-p102">Общий объем использованного дискового пространства в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44a8f-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="44a8f-118">remaining</span><span class="sxs-lookup"><span data-stu-id="44a8f-118">remaining</span></span>     | <span data-ttu-id="44a8f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="44a8f-119">Int64</span></span>  | <span data-ttu-id="44a8f-p103">Общий объем дискового пространства, оставшегося до достижения максимальной квоты, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44a8f-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="44a8f-122">deleted</span><span class="sxs-lookup"><span data-stu-id="44a8f-122">deleted</span></span>       | <span data-ttu-id="44a8f-123">Int64</span><span class="sxs-lookup"><span data-stu-id="44a8f-123">Int64</span></span>  | <span data-ttu-id="44a8f-p104">Общий объем дискового пространства, занятого файлами в корзине, в байтах. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44a8f-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="44a8f-126">состояние</span><span class="sxs-lookup"><span data-stu-id="44a8f-126">state</span></span>         | <span data-ttu-id="44a8f-127">string</span><span class="sxs-lookup"><span data-stu-id="44a8f-127">string</span></span> | <span data-ttu-id="44a8f-p105">Значение перечисления, указывающее состояние дискового пространства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44a8f-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="44a8f-130">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="44a8f-130">storagePlanInformation</span></span>  | [<span data-ttu-id="44a8f-131">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="44a8f-131">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="44a8f-132">Сведения о планах квот хранилища диска.</span><span class="sxs-lookup"><span data-stu-id="44a8f-132">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="44a8f-133">Только в личном хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="44a8f-133">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="44a8f-134">Значения перечисления State</span><span class="sxs-lookup"><span data-stu-id="44a8f-134">State enumeration values</span></span>

| <span data-ttu-id="44a8f-135">Значение</span><span class="sxs-lookup"><span data-stu-id="44a8f-135">Value</span></span>      | <span data-ttu-id="44a8f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="44a8f-136">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="44a8f-137">На диске еще много свободного дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="44a8f-137">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="44a8f-138">Объем свободного дискового пространства менее 10 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="44a8f-138">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="44a8f-139">Объем свободного дискового пространства менее 1 % общего объема дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="44a8f-139">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="44a8f-p107">Объем использованного дискового пространства превышает максимально допустимый объем дискового пространства. Вам не удастся добавлять новые файлы или папки на диск, пока объем использованного дискового пространства не станет меньше общего объема дискового пространства или пока вы не приобретете дополнительное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="44a8f-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": [
    "Error: /api-reference/beta/resources/quota.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
