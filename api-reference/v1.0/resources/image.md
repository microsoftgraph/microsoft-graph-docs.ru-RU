---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 4526b8d475b36521ee08829b50931438999ca249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830417"
---
# <a name="image-resource-type"></a><span data-ttu-id="89552-102">Тип ресурса Image</span><span class="sxs-lookup"><span data-stu-id="89552-102">Image resource type</span></span>

<span data-ttu-id="89552-p101">Ресурс **Image** — это единая структура, объединяющая свойства, связанные с изображением. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **image**, то этот ресурс представляет точечный рисунок.</span><span class="sxs-lookup"><span data-stu-id="89552-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="89552-105">**Примечание.** Если службе не удается определить ширину и высоту изображения, ресурс **Image** может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="89552-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89552-106">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89552-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="89552-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="89552-107">Properties</span></span>

| <span data-ttu-id="89552-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="89552-108">Property</span></span>   | <span data-ttu-id="89552-109">Тип</span><span class="sxs-lookup"><span data-stu-id="89552-109">Type</span></span>  | <span data-ttu-id="89552-110">Описание</span><span class="sxs-lookup"><span data-stu-id="89552-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="89552-111">**height**</span><span class="sxs-lookup"><span data-stu-id="89552-111">**height**</span></span> | <span data-ttu-id="89552-112">Int32</span><span class="sxs-lookup"><span data-stu-id="89552-112">Int32</span></span> | <span data-ttu-id="89552-p102">Необязательный. Высота изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89552-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="89552-116">**width**</span><span class="sxs-lookup"><span data-stu-id="89552-116">**width**</span></span>  | <span data-ttu-id="89552-117">Int32</span><span class="sxs-lookup"><span data-stu-id="89552-117">Int32</span></span> | <span data-ttu-id="89552-p103">Необязательный. Ширина изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89552-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="89552-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="89552-121">Remarks</span></span>

<span data-ttu-id="89552-122">В OneDrive для бизнеса этот ресурс возвращается для элементов, которые должны быть изображениями в соответствии с расширением файла.</span><span class="sxs-lookup"><span data-stu-id="89552-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="89552-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="89552-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
