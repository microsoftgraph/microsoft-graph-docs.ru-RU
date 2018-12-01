---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
ms.openlocfilehash: c9e647ef630e8822d835aec1bd72b9f3c18f2e3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079865"
---
# <a name="image-resource-type"></a><span data-ttu-id="ba428-102">Тип ресурса Image</span><span class="sxs-lookup"><span data-stu-id="ba428-102">Image resource type</span></span>

> <span data-ttu-id="ba428-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba428-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba428-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba428-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba428-p102">Ресурс **Image** — это единая структура, объединяющая свойства, связанные с изображением. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **image**, то этот ресурс представляет точечный рисунок.</span><span class="sxs-lookup"><span data-stu-id="ba428-p102">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="ba428-107">**Примечание.** Если службе не удается определить ширину и высоту изображения, ресурс **Image** может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="ba428-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba428-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba428-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="ba428-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba428-109">Properties</span></span>

| <span data-ttu-id="ba428-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba428-110">Property</span></span>   | <span data-ttu-id="ba428-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ba428-111">Type</span></span>  | <span data-ttu-id="ba428-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ba428-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="ba428-113">**height**</span><span class="sxs-lookup"><span data-stu-id="ba428-113">**height**</span></span> | <span data-ttu-id="ba428-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ba428-114">Int32</span></span> | <span data-ttu-id="ba428-p103">Необязательный. Высота изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba428-p103">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="ba428-118">**width**</span><span class="sxs-lookup"><span data-stu-id="ba428-118">**width**</span></span>  | <span data-ttu-id="ba428-119">Int32</span><span class="sxs-lookup"><span data-stu-id="ba428-119">Int32</span></span> | <span data-ttu-id="ba428-p104">Необязательный. Ширина изображения в пикселях. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba428-p104">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="ba428-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="ba428-123">Remarks</span></span>

<span data-ttu-id="ba428-124">В OneDrive для бизнеса этот ресурс возвращается для элементов, которые должны быть изображениями в соответствии с расширением файла.</span><span class="sxs-lookup"><span data-stu-id="ba428-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="ba428-125">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ba428-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
