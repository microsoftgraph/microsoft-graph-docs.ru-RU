---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
ms.openlocfilehash: 0a4af14f08b94f0ba64f33838322fb0210bcda15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027427"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="84b2a-102">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="84b2a-102">GeoCoordinates resource type</span></span>

<span data-ttu-id="84b2a-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="84b2a-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84b2a-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84b2a-105">JSON representation</span></span>

<span data-ttu-id="84b2a-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="84b2a-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="84b2a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="84b2a-107">Properties</span></span>

| <span data-ttu-id="84b2a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="84b2a-108">Property</span></span>  | <span data-ttu-id="84b2a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="84b2a-109">Type</span></span>   | <span data-ttu-id="84b2a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84b2a-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="84b2a-111">altitude</span><span class="sxs-lookup"><span data-stu-id="84b2a-111">altitude</span></span>  | <span data-ttu-id="84b2a-112">Double</span><span class="sxs-lookup"><span data-stu-id="84b2a-112">Double</span></span> | <span data-ttu-id="84b2a-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84b2a-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="84b2a-116">latitude</span><span class="sxs-lookup"><span data-stu-id="84b2a-116">latitude</span></span>  | <span data-ttu-id="84b2a-117">Double</span><span class="sxs-lookup"><span data-stu-id="84b2a-117">Double</span></span> | <span data-ttu-id="84b2a-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84b2a-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="84b2a-121">longitude</span><span class="sxs-lookup"><span data-stu-id="84b2a-121">longitude</span></span> | <span data-ttu-id="84b2a-122">Double</span><span class="sxs-lookup"><span data-stu-id="84b2a-122">Double</span></span> | <span data-ttu-id="84b2a-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84b2a-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="84b2a-126">Заметки</span><span class="sxs-lookup"><span data-stu-id="84b2a-126">Remarks</span></span>

<span data-ttu-id="84b2a-127">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="84b2a-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
