---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Изображение
localization_priority: Normal
ms.openlocfilehash: b9b8e65442b268e58f920d9b08b60ae8de35df35
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506341"
---
# <a name="image-resource-type"></a><span data-ttu-id="e0ab4-102">Тип ресурса Image</span><span class="sxs-lookup"><span data-stu-id="e0ab4-102">Image resource type</span></span>

<span data-ttu-id="e0ab4-p101">Ресурс **Image** — это единая структура, объединяющая свойства, связанные с изображением. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **image**, то этот ресурс представляет точечный рисунок.</span><span class="sxs-lookup"><span data-stu-id="e0ab4-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="e0ab4-105">**Примечание.** Если службе не удается определить ширину и высоту изображения, ресурс **Image** может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="e0ab4-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0ab4-106">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e0ab4-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="e0ab4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0ab4-107">Properties</span></span>

| <span data-ttu-id="e0ab4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0ab4-108">Property</span></span>   | <span data-ttu-id="e0ab4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e0ab4-109">Type</span></span>  | <span data-ttu-id="e0ab4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e0ab4-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="e0ab4-111">**height**</span><span class="sxs-lookup"><span data-stu-id="e0ab4-111">**height**</span></span> | <span data-ttu-id="e0ab4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ab4-112">Int32</span></span> | <span data-ttu-id="e0ab4-p102">Необязательный. Высота изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0ab4-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="e0ab4-116">**width**</span><span class="sxs-lookup"><span data-stu-id="e0ab4-116">**width**</span></span>  | <span data-ttu-id="e0ab4-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ab4-117">Int32</span></span> | <span data-ttu-id="e0ab4-p103">Необязательный. Ширина изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0ab4-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="e0ab4-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="e0ab4-121">Remarks</span></span>

<span data-ttu-id="e0ab4-122">В OneDrive для бизнеса этот ресурс возвращается для элементов, которые должны быть изображениями в соответствии с расширением файла.</span><span class="sxs-lookup"><span data-stu-id="e0ab4-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="e0ab4-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e0ab4-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
