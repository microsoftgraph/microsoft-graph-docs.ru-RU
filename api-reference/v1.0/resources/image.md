---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Изображение
localization_priority: Normal
description: Ресурс Image — это единая структура, объединяющая свойства, связанные с изображением.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e43bf96a34693b19a191d09417623828e1b399be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086664"
---
# <a name="image-resource-type"></a><span data-ttu-id="f9af2-103">Тип ресурса Image</span><span class="sxs-lookup"><span data-stu-id="f9af2-103">Image resource type</span></span>

<span data-ttu-id="f9af2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9af2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9af2-p101">Ресурс **Image** — это единая структура, объединяющая свойства, связанные с изображением. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **image**, то этот ресурс представляет точечный рисунок.</span><span class="sxs-lookup"><span data-stu-id="f9af2-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="f9af2-107">**Примечание.** Если службе не удается определить ширину и высоту изображения, ресурс **Image** может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="f9af2-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9af2-108">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f9af2-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="f9af2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9af2-109">Properties</span></span>

| <span data-ttu-id="f9af2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9af2-110">Property</span></span>   | <span data-ttu-id="f9af2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f9af2-111">Type</span></span>  | <span data-ttu-id="f9af2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f9af2-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="f9af2-113">**height**</span><span class="sxs-lookup"><span data-stu-id="f9af2-113">**height**</span></span> | <span data-ttu-id="f9af2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f9af2-114">Int32</span></span> | <span data-ttu-id="f9af2-p102">Необязательный. Высота изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9af2-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="f9af2-118">**width**</span><span class="sxs-lookup"><span data-stu-id="f9af2-118">**width**</span></span>  | <span data-ttu-id="f9af2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f9af2-119">Int32</span></span> | <span data-ttu-id="f9af2-p103">Необязательный. Ширина изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9af2-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="f9af2-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="f9af2-123">Remarks</span></span>

<span data-ttu-id="f9af2-124">В OneDrive для бизнеса этот ресурс возвращается для элементов, которые должны быть изображениями в соответствии с расширением файла.</span><span class="sxs-lookup"><span data-stu-id="f9af2-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="f9af2-125">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f9af2-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->

