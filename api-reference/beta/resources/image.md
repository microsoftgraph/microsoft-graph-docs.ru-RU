---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 588f5185cba3012ce3dce77a9707aa23be2bf0cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513930"
---
# <a name="image-resource-type"></a><span data-ttu-id="e45d9-102">Тип ресурса Image</span><span class="sxs-lookup"><span data-stu-id="e45d9-102">Image resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e45d9-p101">Ресурс **Image** — это единая структура, объединяющая свойства, связанные с изображением. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **image**, то этот ресурс представляет точечный рисунок.</span><span class="sxs-lookup"><span data-stu-id="e45d9-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="e45d9-105">**Примечание.** Если службе не удается определить ширину и высоту изображения, ресурс **Image** может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="e45d9-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e45d9-106">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e45d9-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="e45d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e45d9-107">Properties</span></span>

| <span data-ttu-id="e45d9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e45d9-108">Property</span></span>   | <span data-ttu-id="e45d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e45d9-109">Type</span></span>  | <span data-ttu-id="e45d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e45d9-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="e45d9-111">**height**</span><span class="sxs-lookup"><span data-stu-id="e45d9-111">**height**</span></span> | <span data-ttu-id="e45d9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e45d9-112">Int32</span></span> | <span data-ttu-id="e45d9-p102">Необязательный. Высота изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e45d9-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="e45d9-116">**width**</span><span class="sxs-lookup"><span data-stu-id="e45d9-116">**width**</span></span>  | <span data-ttu-id="e45d9-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e45d9-117">Int32</span></span> | <span data-ttu-id="e45d9-p103">Необязательный. Ширина изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e45d9-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="e45d9-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="e45d9-121">Remarks</span></span>

<span data-ttu-id="e45d9-122">В OneDrive для бизнеса этот ресурс возвращается для элементов, которые должны быть изображениями в соответствии с расширением файла.</span><span class="sxs-lookup"><span data-stu-id="e45d9-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="e45d9-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e45d9-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image",
  "suppressions": [
    "Error: /api-reference/beta/resources/image.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
