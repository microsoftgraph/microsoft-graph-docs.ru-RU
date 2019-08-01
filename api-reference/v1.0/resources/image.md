---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Изображение
localization_priority: Normal
description: Ресурс Image — это единая структура, объединяющая свойства, связанные с изображением.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d8b9f871ed465f3f6f617638a8dba38d575509a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032405"
---
# <a name="image-resource-type"></a><span data-ttu-id="25654-103">Тип ресурса Image</span><span class="sxs-lookup"><span data-stu-id="25654-103">Image resource type</span></span>

<span data-ttu-id="25654-p101">Ресурс **Image** — это единая структура, объединяющая свойства, связанные с изображением. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **image**, то этот ресурс представляет точечный рисунок.</span><span class="sxs-lookup"><span data-stu-id="25654-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="25654-106">**Примечание.** Если службе не удается определить ширину и высоту изображения, ресурс **Image** может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="25654-106">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25654-107">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25654-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="25654-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="25654-108">Properties</span></span>

| <span data-ttu-id="25654-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="25654-109">Property</span></span>   | <span data-ttu-id="25654-110">Тип</span><span class="sxs-lookup"><span data-stu-id="25654-110">Type</span></span>  | <span data-ttu-id="25654-111">Описание</span><span class="sxs-lookup"><span data-stu-id="25654-111">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="25654-112">**height**</span><span class="sxs-lookup"><span data-stu-id="25654-112">**height**</span></span> | <span data-ttu-id="25654-113">Int32</span><span class="sxs-lookup"><span data-stu-id="25654-113">Int32</span></span> | <span data-ttu-id="25654-p102">Необязательный. Высота изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25654-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="25654-117">**width**</span><span class="sxs-lookup"><span data-stu-id="25654-117">**width**</span></span>  | <span data-ttu-id="25654-118">Int32</span><span class="sxs-lookup"><span data-stu-id="25654-118">Int32</span></span> | <span data-ttu-id="25654-p103">Необязательный. Ширина изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25654-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="25654-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="25654-122">Remarks</span></span>

<span data-ttu-id="25654-123">В OneDrive для бизнеса этот ресурс возвращается для элементов, которые должны быть изображениями в соответствии с расширением файла.</span><span class="sxs-lookup"><span data-stu-id="25654-123">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="25654-124">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="25654-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
